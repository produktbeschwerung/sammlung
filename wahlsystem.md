# Restrukturierung von Wahl und Parteien

## Einleitung

Die derzeitigen Themen auf den Wahl-Programmen der Parteien sind Versprechungen, die nicht an messbaren Werten gekoppelt sind. 

Oft sind diese Themen grobe Richtungen mit emotionaler Stimmungsmache gegen andere Parteien. siehe ([Wahlprogramm CDU / CSU 2017](https://www.cdu.de/system/tdf/media/dokumente/170703regierungsprogramm2017.pdf?file=1)) 


**Teilauschnitt**
```
Die rot-grüne Koalition hat im Jahr 2005 über 5 Millionen
Arbeitslose hinterlassen. In der Regierungszeit von Bundeskanzlerin Angela Merkel
und der Union ist es uns gelungen, die Arbeitslosigkeit zu halbieren. Im Juni dieses 
Jahres lag die Arbeitslosigkeit unter 2,5 Millionen, das entspricht einer
Arbeitslosenquote von nur noch 5,5 Prozent. Dies ist eine großartige Bestätigung
für unsere Politik.
```

Viele Themen, die in diesen Wahl-Programmen angesprochen werden, sind eben nur angesprochen und nicht schon mit fest definierten Aufgaben und Lösungen verankert.

```
Unser Land braucht geeignete und qualifizierte Fachkräfte in großer Zahl.
Deshalb werden wir unsere Anstrengungen in den Bereichen Bildung, Ausbildung und Weiterbildung erheblich verstärken. Wir wollen mehr Frauen
ermöglichen sozialversicherungspflichtig zu arbeiten. Zudem wollen wir gerade junge Menschen zwischen 25 und 35 ohne Abschluss nachqualifizieren,
um ihnen das dauerhafte Erarbeiten des eigenen Lebensunterhalts zu
ermöglichen. So schöpfen wir das Arbeitskräftepotenzial in unserem Land
besser aus, schaffen neues Wachstum und verringern die Arbeitslosigkeit
weiter. Kein Arbeitsplatz soll unbesetzt bleiben, weil es an Fachkräften fehlt.
```
Nach Ablauf der Legislatur-Periode möchte man als Wähler wissen, ob dieses Thema erfolgreich angegangen wurde, jetzt stellen sich folgende Fragen:

- In welchem Bereich fehlten denn diese Fachkräfte? 
- Welche Maßnahmen wurden im Bereich der Bildung unternommen?
- Wieviele Menschen gab es vorher ohne Abschluss?

Durch die schwamminge Beschreibung ergibt sich ein großer Spielraum, den die Partei so nutzen und auslegen kann, dass es am Ende als erfolgreich umgesetzt gilt. 

```
Interpretations-Spielräume dürfen nicht existieren.
```

Wie agile Software-Entwicklung als Vorbild zur Definierung und Umsetzung von Themen innerhalb einer Regierung die Transparenz erhöht und die Beziehung zwischen Volk und Politik stärkt und schütz.

## Parteien

**Aufgaben und Pflichten beim Erstellen des Wahl-Programmes:**
- Ein Wahl-Programm ist die Todo-Liste der Partei.
- Ein Todo ist ein Thema auf dem Wahl-Programm welches anhand von konkreten Zielen abgeschlossen werden kann
- Ein Todo hat ein Ziel, welches sich durch einen Ist-Zustand und Soll Zustand definiert
- Einn Ist oder Soll Zustand ist durch einen Messbaren Wert verankert.
- Ein Messbarer Wert definiert sich über eine parteien unabhängige Quelle (API).

**Problem**

Die Ausarbeitung eines solchen Wahl-Programmes gestaltet sich aufwändiger und benötigt mehr Zeit. 

**Lösung**

Eine Partei wird in zwei equivalente in sich funktionierende Teams unterteilt.
Diese Teams sind jeweils mit allen relevanten Personalien und Kompetenzen für die Ausübung als regierende Partei besetzt.
Diese Teams arbeiten parallel in zwei verschiedenen Phasen.

#### Definierung des Programmes
In dieser Phase erarbeitet das Team ein Wahl-Programm mit allen nötigen Informationen.

#### Ausführung als Regierung
Die Partei ist dazu verpflichtet die Themen auf dem Wahl-Programm bis zum ende der Legislatur-Periode umzusetzen.

### Phasen-Wechsel
Nach Ablauf der Legislatur-Periode tauschen die Teams.

Team A von Definierung zur Auführung
Team-B von Ausführung zur Definierung

**Begründung**
Durch die Aufteilung in zweier parallel arbeitenden Teams, erhalten diese Teams jeweils 4 Jahre Zeit zur Ausarbeitung des Wahl-Programmes. 

**Das Versprechen vor der Wahl**
Jedes einzelne Thema einer Partei, welches als Punkt im Wahlprogramm aufgenommen ist, besitzt messbare klar definierte Werte, die zur
Bestimmung des erfolgreichen abschließen dienen.

#### Beispiel Themen
- Wir als Partei haben die Armutsgrenze um x Prozentpunkte gesenkt.
- Wir als Partei haben das Gesetz zum Upload-Filter in unserem Gesetzbuch X verankert.
- Jede Schule in Deutschland besitzt einen Glasfaser-Zugang zum Internet.
- Wir als Partei haben 15 Milliarden Euro in den Erhalt und die Förderung der Kultur folgender Einrichtungen / Orte entrichtet:
  - Museum X bekommt Summe Y
  - Zeche-Zoll-Verein erhält Betrag X
- Die Taktfrequenzen von Zügen auf den Strecken X,Y,Z wurden von 3 Zügen pro Stunde auf 4 Züge erhöht.

#### Bildung und Aufbau eines Themas

**Wahl-Ergebnis**
Nach erfolgreich abgeschlossener Wahl, wird die Partei mit den höchsten Abstimmungswerten (tbd), für den nächsten Sprint in die Regierung gewählt.

**Zyklus**
Die regierende Partei hat einen Zyklus Zeit Ihre Wahlversprechen zu erfüllen.

**Wahlversprechen Erfüllt**
Erfüllt die Partei mind. 75% aller Versprechen, wird diese für die darauf folgende Wahl, wieder zugelassen.

**Wahlversprechen nicht erfüllt**
Erfüllt die Partei nicht das abschließen von mind. 75% aller Versprechen, wird diese für einen Zyklus ausgesetzt.

**Bann Grund**

#### Archiv

(Durch ein 2-Team Fail-Over wird bei Misserfolg die Abschließung von unfertigen Themen durch die Fachkompetenz des zweiten Teams gewährleistet und iterativ verbessert)

**Ablauf**
wird jede antretende Partei in zwei Teams mit jeweils ausgeglichener Kompetenzen aufgeteilt. Dies hat zur Folge, dass Parteien bei Wiederwahl durch das zweite Team für diese legislatur Periode vertreten wird.

Somit wählt der Bürger nicht nur die Partei, sondern direkte Themen, die nach Ablauf der Legislatur-Periode erfüllt sein müssen.
Erfüllt das Team der regierenden Partei nicht innerhalb der Legislatur-Periode mind. 75% aller Punkte Ihres Wahlprogrammes, wird diese Partei für eine Legislatur-Periode gesperrt, damit diese Zeit hat, personelle / strukturelle Probleme innerhalb der Teams zu beheben,
damit die Neu-Aufstellung mit ihrem Wahlprogramm, um den darauf folgenden Regierungs-Sprint zu bewerben.

Ein Wahlprogramm ist ein

