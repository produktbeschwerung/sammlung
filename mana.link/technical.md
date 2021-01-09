# ⌨️ Developing

## Source-Code Hosting
- [Gitlab]

## Hosting
Die Webseite wird über das IPFS auf der Domain mana.link ausgeliefert. IPFS ist das dezentrale Speicher-Netzwerk. Beim export der Webseite wird durch den Service https://pinata.cloud/ mittels API Key die gerenderte Webseite ins IPFS gespeichert.

- IPFS for decentalized hosting
- [IPFS Service](https://pinata.cloud/)

## Web
- [NextJS](https://nextjs.org/)
- [ReactJS](https://reactjs.org/)
- StyledComponents
- [Polkadot{js}](https://polkadot.js.org/) zum verknüpfen des Wallets

## Blockchain
- [Substrate](https://substrate.dev/) zum erzeugen der eigenen Blockchain auf basis von Polkadot
- [Setup Substrate Blockchain](https://medium.com/@wilfried.kopp/your-very-own-local-polkadot-substrate-network-in-less-than-30s-1dd466f7f22b)
- [Awesome Substrate](https://github.com/substrate-developer-hub/awesome-substrate)

## Deployment
- [Gitlab]
Das Repository wird durch eine Pipeline in GitLab deployed. Nachdem NextJS exportiert wurde, wird der `out` Ordner mittels folgendem Code auf dem IPFS deployed

```jsx
const sourcePath = `${__dirname}/web/out`;
const options = {
    pinataMetadata: {
        name: 'Mana.Link',
        keyvalues: {
            customKey: 'customValue',
            customKey2: 'customValue2'
        }
    },
    pinataOptions: {
        cidVersion: 0
    }
};

const result = await pinata.pinFromFS(sourcePath, options)
```

### Pflanzenerkennung per AI
Beim scannen der Pflanze, zum verknüpfen des Besitzers, verwenden wir eine AI zum identifizieren der Pflanze. 
- Service: https://web.plant.id/plant-identification-api/

### Foto Upload
Fotos von den Pflanzen werden im IPFS abgespeichert und erhalten eine CID zur Wiedererkennung.

### Transaktion
im folgenden Code ist der logische Ablauf einer Transaktion beschrieben.

```jsx

const previousTransactionBlock = Polkadot.getTransactionBlockFromHash(hash)

// User
const senderWallet = previousTransactionBlock.getRecieverAdress()
const recieverWallet = LocalWallet.getRecieverWalletAdress()

// Object
const picture = getPictureFromCamera()

// ObjectData
const pictureCID = uploadPictureToIPFS(picture)
const aiResult = recognitePlantFromAI(picture)

const manaCost = 5;

// Abort on insufficient balance
if (recieverWallet.getBalance() < manaCost) {
  new Error('insuffiecent balance')
}

// build new Transaction
const Transaktion = new Polkadot.newTransaction()

Transaktion.setSender(senderWallet.getAdress())
Transaktion.setReciever(senderWallet.getAdress())
Transaktion.setManaAmount(manaCost)

Transaktion.setObject({
  type: 'plant',
  name: aiResult.name,
  picture: pictureCID
})

Transaktion.execute()

```

### Transaktions Block Beispiel
```jsx

const Block = {
  owners: {
    sender: senderWallet.getAdress(),
    reciever: recieverWallet.getAdress()
  },
  object: {
    type: 'plant',
    name: aiResult.name,
    picture: pictureCID
  }
}
```
