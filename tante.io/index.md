# Whitepaper - tante.io

## Leitsatz
Finde was du brauchst, wenn du es brauchst bei dir um der Ecke. 

Nachhaltiger Micro Delivery Service in deiner Umgebung

## Einleitung

Das Synonym für das Projekt, tante.io, möchte ein großen Pain angehen. tante.io versucht die Transparenz in Bereichen, die sich bisher der Digitalisierung entzogen, auf die neuesten Standards hieven.
tante.io versucht durch Community Driven Data Collecting, ein selbst auffrischendes System zu etablieren, wobei der Besitzer eines POI jederzeit die Kontrolle über seine Daten übernehmen kann diese aktualisieren.
tante.io erfasst in fleißarbeit, alle zum Launch relevanten und benötigten Daten aller Kiosks innerhalb der unten aufgelisteten Locations:

Köln
Münster

## Konkurrenz
https://www.marktfee.app/

## User-Flow

Der Besucher löst Anhand seiner aktuellen Position, eine Umkreissuche aus, in der alle Kiosk, die sich innerhalb des Suchradius befinden, und den Filterkriterien, wie z.b. Öffnungzeiten o. Paketrückgabe, angezeigt werden.

## Milestone One

Kiosk
Fragen

- Bezahlmethoden
  - Bar, Karte, PayPal, Bitcoin
- Kann man an diesem Kiosk DHL Pakete abholen / hinbringen?
  - Hermes		
  - DHL
  - UPS
  - usw.
- Kann man hier Sim Karten aufladen?
- Kann man hier Mund-Nasen-Schutz Masken kaufen?
- Kann man hier drucken?
- Gibt es hier kostenloses WLAN?
- Kann man sich hier an den PC setzen?
- Gibt es hier im Kiosk Sitzgelegenheiten?
- ist das Kiosk barrierefrei erreichbar?
- Kann man hier Bahntickets kaufen?
- Kann man hier Gutscheine kaufen?
- Gibt es hier Zigaretten Liquids?
- Gibt es hier Shisha Tabak?
- Gibt es hier Lebensmittel?
- Gibt es belegte oder trockene Brötchen?
- Kann man hier Kaffee trinken?
- Bekomme ich hier meine Zeitung / Zeitschrift?
- Ist ein Briefkasten hier in der nähe?
- Kann man hier Briefmarken kaufen
- Gibt es hier Schreibwaren?
- Gibt es hier Hygieneartikel?
- Gibt es hier CBD
- Kann man hier sein Smartphone laden?
- Wo kann ich verpackungsfrei einkaufen?
- Wo kann ich was reparieren lassen?
- Wo kann ich mein Geschenk einpacken lassen?

## Mögliche Szenarien

**Kiosk von Seite entfernen**
Der Kiosk Besitze möchte nicht, dass das Kiosk auf der Seite ist. Hierfür wird es einen melden Button geben.

Kioskbesitzer möchte selber die Daten angeben

**Suchkriterien**
Der Kunde möchte in Ehrenfeld ein Kiosk finden, indem man sein DHL Paket abgeben kann.

Dazu gibt es auf der Kartenansicht die Möglichkeit nach DHL Stores zu filtern, sodass mir auf der karte nur noch Kioske in der Umgebung angezeigt werden, die eine DHL Paket-Abgabe ermöglichen.

## Features

**Werbeflächen**
Jedes Kiosk hat die Möglichkeit für eine Servicegebühr einen Werbeplatz an prominenten Stellen auf der Webseite zu reservieren, um dort Werbung für sein eigenes Kiosk zu machen.

**Label Zertifiziertes Kiosk**
Als Kioskbetreiber kann ich mein Kiosk auf der Seite verifizieren, dass ich der Eigentümer bin und alle dort eingetragen Daten korrekt sind. Damit erhält das Kiosk ein spezielles Zertifiziert Label

**Favoriten Liste**
Ich habe mein favorisiertes Kiosk und möchte direkt sehen, ob mein Wunschprodukt dort gerade verfügbar ist. Dafür möchte ich das Kiosk mit einem Klick auf de Button (Zu Favoriten hinzufügen) das Kiosk zu meiner Favoritenliste hinzuzufügen, sodass ich schnell mit einem Klick auf der Startseite, auf die Detailseite des Kiosk gelangen.

**24 Stunden Service**
Ein Kiosk mit einem 24 Stunden Öffnungsservice, erhalten auf tante.io ein auffäliges erkennungsmerkmal.

## Marketing

**Sticker mit QR Code**
Sticker an den Kiosken platzieren mit “frag die tante.io” und einem QR Code der auf tante.io leitet

Sticker überall hinlegen z.b. an die Kiosk Kasse

**Blog**
Einen Blog starten, auf dem man das geplante Image von der Tante vertritt und zeitgemäße und interessante Themen behandelt, sodass große socials interesse entstehen kann.

## Technische Umsetzung

Die Applikation wird mit NextJS und Strapi als Datenbank und API umgesetzt. Das Design ist fertig und kann innerhalb der technischen Umsetzung umgesetzt werden. Die Domain tante.io routet auf den Server, auf der die die Applikation läuft.

**Dependency List**
- Docker
- Node Image
- Auth0
- GraphDB
- NextJS
- GraphQL
- Styled-Components
- Typescript
- GitLab

### Seitentypen

- Startseite (Suche)
- Ergebnisse der Suche
- Filtermöglichkeiten erlauben das schnelle finden meines Anliegens
- Kiosk Detailansicht
  - Adresse
  - Bezahlmethoden
  - usw.
- Formular zum eintragen weiterer Daten in Bezug auf gewähltes Kiosk
- Hilfe Center
- Feedback Formular
- Impressum
- Datenschutz
- Allgemeine Geschäftsbedingungen
- Über Uns und unsere Intention
- Blog
  - Übersichtsseite
  - Beitragsseite


## Milestone Two
Integration von Services und Lieferanten.

### Weitere Services
Hier eine Liste mit zukünftig möglichen Services, die auf tante.io angeboten werden könnten.

Für den Start und Abschluss der Phase zwei entscheiden wir uns dafür den Service Wertstoffe-Entsorgung und Pfand Rückgabe an die bestehende Kiosk Datenbank anzuschließen, um so den Usern, weitere Services zu bieten.

**Wertstoffe-Entsorgung und Pfand Rückgabe**
Die Möglichkeit Alt-Glas, Pfand, Altkleider, Pappe oder speziell zu entsorgende Werkstoffe, gegen eine Gebühr von 1-6 EURO abholen zu lassen, damit diese entsorgt werden.

**Street Disposal**
Zusätzlich wird angegeben, dass Leute die Müll auf der Straße sehen, den melden können und direkt gegen eine kleine Gebühr entsorgt wird.

**Briefabholung**
Ich möchte einen Brief verschicken, habe weder Ahnung wo der Briefkasten ist, geschweige denn eine Briefmarke. Jemand kommt bei mir zuhause vorbei mit einem frankierten Briefumschlag und nimmt diesen Brief mit und wirft ihn in den Briefkasten.

Lieferanten

Bewerbung für Services
Privat Personen können sich auf der tante.io registrieren um einen bestimmten Service auszuüben. Dies kann z.b. Briefe abolen sein. Der Lieferant erhält die komplette Servicegebühr Summe abzüglich der Kosten in Höhe von 10% vom Gesamtbetrag bei tante.io anfallen.

Daten über den Lieferanten
Foto
Alter
Geschlecht
Bewertungen

Statistiken
Jeder Lieferant sieht übersichtlich seine erledigten Jobs und den dazugehörigen monatlichen Konto-Stand.

Bewertung
Jeder Lieferant kann für seinen Job, den er erledigt hat, bewertet werden. In einer Skala 0-5, sodass jeder Kunde, sofort sieht, wie zuverlässig der Lieferant ist. Die Darstellung könnten Sterne sein, wie auch ein Kopf von tante.io

Belohnungssystem
Jeder lieferant der fleißig der tante.io hilft, erhält nach verschieden erreichten aufgaben von der tante.io eine kleine Belohnung, damit der haussegen nicht schief hängt.
Diese Belohnung sind mit dem Account des Lieferanten verankert und setzen sich nicht zurück. Diese könne erspielt werden in einer Zeitleiste. Verschiedene Beispiele
Profilfoto hinzugefügt + TanteTonken

Supporter
Supporter sind Leute, die den Kunden und den Lieferanten bei technischen Fragen oder allgemeinen Fragen zu den Services entstehen, dabei helfen, diese zu beantworten.

Service Workflows

Pfand-Rückgabe

Kunde bucht Service Pfand-Rückgabe für 3 EUR
Geldsumme wird auf der tante.io als TanteToken zwischen gespeichert.
Job muss von Lieferant angenommen.
Bei Fehler oder Fehlvermittlung erhält der Kunde den vollen Betrag + 2% Entschuldigungs Bonus erstattet.
Lieferant fährt zu Kunde mit Lastenrad und bestätigt Ankunft.
Kunde übergibt die Behältnisse mit Pfand dem Lieferanten.
Lieferant bestätigt in App, den erhalt des Pfands.
Lieferant bringt Pfand zurück und erhält Pfand-Gutschein-Bon mit Code.
Lieferant übermittelt ein Foto von diesem Bon an den Kunden und bestätigt den Abschluss des Jobs.
Der Kunde bestätigt den Erhalt des Bons
Gespeicherte TanteToken werden auf das Konto des Lieferanten transferiert.
Lieferant kann sich die TanteToken zum aktuellen Tauschpreis in FIAT umwandeln.


Briefabholung
Kunde bucht Service Briefabholung für 3 EUR
Geldsumme wir auf der tante.io zwischen abgelegt.
Job muss von Lieferant angenommen.
Bei Fehler oder Fehlvermittlung erhält der Kunde den vollen Betrag + 2% Entschuldigungs Bonus erstattet.
Lieferant fährt zu Kunde mit Lastenrad und bestätigt ankunft.
Foto von Brief wird vom Kunden angefertigt, Brief wird übergeben. Lieferant bestätigt die Annahm des Pakets.
Brief wird eingeworfen mit Beweisfoto (ähnlich wie E-Scooter) und über tante.io der Auftrag als abgeschlossen markiert.
Der Auftraggeber, prüft das Foto und bestätigt den erfolgreichen Abschlusses des Jobs.
Geldsumme wird sofort vom zwischengespeicherten Konto, abzüglich der 10% Service Gebühr an tante.io an den Lieferant transferiert.


Unternehmen

Rechtsform
tante.io ist bei start des Projektes eine GBR Schauf
Bei Abschluss von Service Phase 2, der integration von Services und Lieferanten, wird das Unternehmen den Crypto-Token, TanteToken in einer festgelegten Summer generiert.

Das Finanz-Ökosystem TanteToken
Der TanteToken ist ein ERC-20 Standard Token, der über die Ethereum Blockchain, anhand eines Smart-Contracts in einer fest angelegten Summe an TanteToken generierte Crypto-Währung. Dieser Token wird in allen internen Unternehmensprozessen, als Träger von Gefallen und Verpflichtungen für die Transferierung zwischen einzelnen Parteien wie Lieferant, Kunde und Mitarbeiter verwendet. Mitarbeiter, Kunden, Lieferanten und Investoren sind alle ein Teil dieses Ökosystems welches nicht zwischen unterschiedlichen Gewichtungen unterscheidet, sondern ganz allein die Anzahl an TanteToken, die jemand in seinem Besitz hat. Somit befindet sich durch die direkte Umwandlung der Fiat Währung in den TanteToken, das komplette Kapital, der komplette Umsatz und alle anderen Werte sich zu jederzeit, solange es noch nicht das Unternehmen verlassen darf, innerhalb dieses Finanz-Öko System von tante.io befindet. Jeder Lieferant oder Mitarbeiter der im Besitz von TanteToken ist, erhält das Recht auf Abstimmungen innerhalb des Unternehmens. Der Token-Besitzer, setzt für Anzahl Token seine Beteiligung an der Abstimmung. Je höher der Einsatz, umso mehr Gewichtung erhält deine Entscheidung.

Jeder erfolgreich abgeschlossen job innerhalb tante.io wird mit der Transferierung des vorab geleisteten Betrags des Kunden, an das Konto des Lieferanten überwiesen. Den TanteToken, kann der Lieferant sich zum aktuellsten Tauschpreis zwischen TanteToken und FIAT tauschen, ohne das der Lieferant diese Umwandlung überhaupt bemerkt.

Die Gewinnung von TanteToken können nur über Leistungen innerhalb des Ökosystems verdient werden. Es gibt keinen direkten Umtausch von EUR in TanteToken

Das Team
Das Unternehmen wird durch Tante Emma repräsentiert. Die Tante Emma hat Bekannte wie Tante Sara, Tante, Molly und Onkel Holger
Archiv

Sperrmüll
Ich wohne in Köln und möchte meine alten Möbel entsorgen. Wo finde ich die Möglichkeit diesen Sperrmüll abholen zu lassen.

Ich möchte Second Hand klamotten kaufen, dafür definiere ich eine Zeit bei mir zuhause vor der Tür, damit dann dort ein Fahrrad Second Hand Shop vor fährt und ich mir direkt vor der haustüre Kleine aussuchen und kaufen kann.

Ein neues Kiosk eröffnet und möchte auf der Karte eingetragen werden.

Änderungsantrag Öffnungszeiten
Das Kiosk hat seine Öffnungszeite

Fotos von Kiosk sollen angezeigt werden können, hierfür sollte es einen Upload geben, sodass jeder ein Foto des Kiosk veröffentlichen kann.

Social Media

Tante.io Instagram Account
Die Tante ist natürlich auch auf Instagram vertreten, wir wollen euch doch nicht unsere Top Favoriten vorenhalten. (Sara)







