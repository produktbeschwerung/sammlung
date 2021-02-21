# KYC basierte ELO Rating- & Matching-Blockchain

## Einleitung
Ein ELO-Rating ist das Einordnen von mehreren Teilnehmern in einem Wettbewerb.
Dieser Wettbewerb findet als reale Sportart oder innerhalb von Computer-Spielen statt.

Die Einordnung der Teilnehmer durch ein ELO-System gewährt ein faires und ausgeglichenes Pairing zwischen mehreren Parteien (1vs1 / 5vs5).
Weitere Informationen zum ELO-System gibt es [hier](https://en.wikipedia.org/wiki/Elo_rating_system).

## Pain
Ein ELO System ist derzeit intransparent und gehört nur dem Spiele-Entwickler.
Somit sind keine Einsichten in:

- Der Verlinkung zwischen Spiele-Account und der Person.
- Die Bildung von Matches gegen andere Spieler. 
- Die Berechnung der Position innerhalb des ELO-Systems.
- Verstöße beim den oberen Punkte.

## Wer spielt?
Die unique Verlinkung einer echten Person und einem Spiele-Account ist derzeit nicht gegeben. 
Durch die Erstellung so genannter Smurf-Accounts kann eine Person dem ELO-System des Spiele-Entwicklers öfters beitreten.

Hier bietete die Blockchain die Möglichkeit eines KYC (Know Your Customer)

Ein Blockchain basiertes ELO-System ist Spiele-Entwickler unabhängig.

## Matchmaking
Personen in einem Wettbewerb können einem Smart-Contract beitreten. 
Somit sind diese innerhalb des Systems als Bereit markiert und werden bei Erfüllung folgender Paramter gematched:

- Spieler Anzahl erfüllt
- Spieler mit gleicher ELO gefunden
  - Nein: Elo Range wird prozentual erhöht
  - Ja: Spieler erhalten Server zum joinen
  
## Match Abschluss
Nachdem ein Match beendet wurde, werden die Ergebnisse der Begegnung als Transaction in die Blockchain gespeichert

## Transaction

```js

const calculatePool = (counterparties, mates) => {
  let sum = 0
  for (let player of counterparties) {
    sum += player.wallet.amount
  }
  
  for (let player of mates) {
    sum += player.wallet.amount
  }
  sum 
  return 
}

const Transaction = {
  counterparties: [walletID],
  mates: [walletID],
  amountOfPoints: calculatePool()
}
````
