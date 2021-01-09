# Mana Link

**Table of Contents**
- [Konzept](#konzept)
  - [Was ist Mana Link?](#was-ist-mana-link?)
  - [Effect](#effect)
  - [Namen](#namen)
  - [Domain](#domain)
  - [User Story](#User-Story)
  - [Prozessablauf](#Prozessablauf)
  - [Finanz-Ökosystem](#Finanz-Ökosystem)
- [Development](#Developing)
  - [Hosting](#hosting)
  - [Technologien](#technologien)

![alt text](/mana.link-logo.png "Mana Link Coin Logo")

## Konzept

### Was ist Mana Link?
Es ist die Währung einer Pflanze die man bei sich in der Wohnung stehen hat. 
Die Pflanze ist der Token, also der Wert. Die Schenkung des Setzlinges an weitere Personen, die Transaktion des Wertes.
Je älter der Token, umso höher die verschenkten Generationen wodurch der Wert des Genesis Token der Pflanze sich erhöht.

### Effect
Schneball System welches mit der Wertigkeit der Plfanze und deren Werdegang, den Erhalt der Natur gewährleistet.

### Namen
- ManaLink
- Plana
- Plantana

### Domain
- [mana.link](https://mana.link)

### User Story
Ich gehe in den Laden "Mana Shop" und kaufe mir dort eine Pflanze. Diese Pflanze stelle ich in meine Wohnung und pflege diese sehr gut. Der Plfanze geht es so gut, dass sie sich vermehrt.
Sie bekommt Setzlinge. Diese Setzlinge nehmen Platz im Topf weg und müssen somit raus und im besten Fall werden diese verschenkt und leben weiter in der nächsten Generation.

### Prozessablauf
Der Genesis-QR-Code öffnet eine Webseite (mana.link/{QR-Code ID} auf der die Plfanze mit Ihrer Geschichte präsentiert wird. 
Dort zu sehen und nur durch den QR-Code berechtigt, erscheint ein Formular, indem man seine persönlichen Daten einträgt und sich somit mit dieser Pflanzer vekrnüpft. 
Nach Abschluss erhält man die Möglichkeit, weitere QR-Codes der 2. Generation zu erzeugen, da die Pflanze Setzlinge bildete, die man umtopfen kann und somit an andere weiterverschenkt. 
Bevor man die Pflanze verschenkt, legt man dem Setzling den QR-Code der 2. Generation bei, sodass sich der Beschenkende der Pflanze, sich auf der URL des neuen Codes wiederum auf mana.link mit dieser Generation als Besitzer verknüpft.
Somit generiert sich nach Weilen eine Verankerungskette, die den Weg der Pflanze durch die Menscheit und der Epochen verknüpft.

Durch diesen Prozess kann man in Zukunft herausfinden, wer hatte alles diese Pflanze, woher kam sie. Es könnte passieren, dass ich meine Pflanze verschenke und diese irgendwann als Geschenk bei einer bekannten Person landet. Bspw. Angelar Merkel.

### Finanz-Ökosystem
Man kauft sich mit der Währung ManaL im Laden "Mana Shop", die Pflanze . Durch die Bezahlung in ManaL darf der Käuft sich auf mana.link für den Genesis Block registrieren.

Jeder neue Eintrag eines Setzlings der weiteren Generationen darf nur durch den Tausch von ManaL sein Besitzestum in der Chain eintragen und somit Teil der Kette werden.

Der Benefit dieser Kette ist die Auszahlung der anteiligen Berürungen beim erzeugen und erhalt des Netzwerkes (Chain), sobald die eigene Pflanze stirbt. Somit verkauft man seine Token und aktualisiert den allgemeinen Bestand.

## Developing

### Hosting
Die Webseite wird über das IPFS auf der Domain mana.link ausgeliefert. IPFS ist das dezentrale Speicher-Netzwerk. Beim export der Webseite wird durch den Service https://pinata.cloud/ mittels API Key die gerenderte Webseite ins IPFS gespeichert.

### Technologien
- [IPFS Hosting](https://pinata.cloud/)
- [NextJS](https://nextjs.org/)
- [ReactJS](https://reactjs.org/)
- StyledComponents
- [Polkadot{js}](https://polkadot.js.org/) zum verknüpfen des Wallets
- [Substrate](https://substrate.dev/) zum erzeugen der eigenen Blockchain auf basis von Polkadot

### Pflanzenerkennung per AI
Beim scannen der Pflanze, zum verknüpfen des Besitzers, verwenden wir eine AI zum identifizieren der Pflanze. 
- Service: https://web.plant.id/plant-identification-api/

### Foto Upload
Fotos von den Pflanzen werden im IPFS abgespeichert und erhalten eine CID zur Wiedererkennung.

### Verknüpfung
Beim schreiben in die Blockchain werden die Wallet-Adresse des neuen Besitzer, die CID

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
const recieverBalance(recieverWallet.getBalance() < manaCost) {
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

*archiv*
Dieses System erzeugt eine finanzielle Einbahnstraße und erzeugt einen Pot für eine Wertigkeit
Der Token ist nicht limitiert von der Menge, sondern wird pro Genesis-Plfanze neu erzeugt und bei Einträgen zweiter Generation usw.usw. Somit ergibt sich eine incrementierende Währung mit Verknüpfung an die Anzahl der verangegangenen Pflanzen und Bestehender Pflanzenanzahl.

Bei Tod der Pflanz, darf man seinen Token, der jeweiligen Generation auszahlen lassen und erhält, anteilig an den, nach mir erzeugten Pflanzen 

