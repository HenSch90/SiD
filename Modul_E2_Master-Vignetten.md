Master-Vignetten 

\--------------------------------

KSM-ma01
========

tc:

vn: 

qt: Einfachauswahl mit vertikalen Antwortoptionen

hl: Fragen zu Masterstudium und Beruf

in: Sie sind momentan im fortgeschrittenen Bachelorstudium und überlegen, ob Sie sich  für ein Masterstudium bewerben.

Nachfolgend bitten wir Sie, für vier hypothetische Masterstudiengänge mit unterschiedlichen Eigenschaften einzuschätzen, wie wahrscheinlich Sie sich bewerben würden. Die Merkmale der Studiengänge sind jeweils in kurzen Texten dargestellt. 

Es handelt sich um einen Studiengang an einer !!staatlichen oder privaten!! Hochschule, der auf Ihrem angestrebten Bachelorabschluss !!fachlich aufbaut!!. !!Wohnkosten und Freizeitmöglichkeiten!! entsprechen in etwa Ihrem !!jetzigen Studienort!!.

q: 

is:

it:

st:

ao1:

ao2:

ao3:

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO mvig[deck]_1 if IF h_deck==[deck]

hi:


\--------------------------------

mvig[deck]_1
=================

tc: 

vn: mabew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl: Attraktivität eines Masterstudiums

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q4: Wie wahrscheinlich würden Sie sich auf diesen Masterstudiengang bewerben?

is:

it:

st:

ao1: 0: sehr unwahrscheinlich

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: mvig[deck]_2

hi: vig1, vig2 und vig3 sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert: [Master-Vignetten](https://github.com/dzhw/SiD/blob/master/Vignetten_Master.xls)

\--------------------------------

mvig[deck]_2
=================

tc: 

vn: mabew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl: Attraktivität eines Masterstudiums

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q4: Wie wahrscheinlich würden Sie sich auf diesen Masterstudiengang bewerben?

is:

it:

st:

ao1: 0: sehr unwahrscheinlich

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: mvig[deck]_3

hi: vig1, vig2 und vig3 sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert: [Master-Vignetten](https://github.com/dzhw/SiD/blob/master/Vignetten_Master.xls)

\--------------------------------

mvig[deck]_3
=================

tc: 

vn: mabew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl: Attraktivität eines Masterstudiums

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q4: Wie wahrscheinlich würden Sie sich auf diesen Masterstudiengang bewerben?

is:

it:

st:

ao1: 0: sehr unwahrscheinlich

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: mvig[deck]_4

hi: vig1, vig2 und vig3 sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert: [Master-Vignetten](https://github.com/dzhw/SiD/blob/master/Vignetten_Master.xls)

\--------------------------------

mvig[deck]_4
=================

tc: 

vn: mabew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl: Attraktivität eines Masterstudiums

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q4: Wie wahrscheinlich würden Sie sich auf diesen Masterstudiengang bewerben?

is:

it:

st:

ao1: 0: sehr unwahrscheinlich

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma02

hi: vig1, vig2 und vig3 sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert: [Master-Vignetten](https://github.com/dzhw/SiD/blob/master/Vignetten_Master.xls)

\--------------------------------


KSM-ma02
========

tc:

vn: maber

qt: Einfachauswahl mit vertikalen Antwortoptionen

hl:

in:

q: Wissen Sie schon, welchen Beruf Sie ergreifen möchten?

is:

it:

st:

ao1: 1: nein, noch offen

ao2: 2: ja, mit einiger Sicherheit

ao3: 3: ja, mit großer Sicherheit

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma03 if maber= 2 OR maber= 3

GOTO KSM-ma04 if maber= 1
GOTO KSM-ma04 if maber= SYSMISS

hi:

\--------------------------------

KSM-ma03
========

tc:

vn: berufswahl

qt: offene Frage

hl:

in:

q: Bitte nennen Sie die genaue Berufsbezeichnung:

is:

it:

st:

ao: (berufswahl): [90 pt, einzeilig, 255 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma04

hi:

\--------------------------------

KSM-ma04
========

tc: (alle)

vn: bervorb

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in:

q: Wie gut fühlen Sie sich durch das Studium für die Ausübung eines Berufs
vorbereitet?

is:

it:

st:

ao1: 1: überhaupt nicht vorbereitet

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut vorbereitet

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma05

hi:

\--------------------------------

KSM-ma05
========

tc:

vn: jobfach; jobabsch; joblohn; joberfue

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern erwarten Sie Schwierigkeiten nach Ihrem Bachelorabschluss, eine
Stelle zu finden, die …

is:

it1: (jobfach): … Ihren fachlichen Fähigkeiten entspricht?

it2: (jobabsch): … Ihrem Hochschulabschluss entspricht?

it3: (joblohn): … Ihren Lohnansprüchen genügt?

it4: (joberfue): … Sie wirklich erfüllt?

st:

ao1: 1: keine Schwierigkeiten

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: große Schwierigkeiten

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma07 IF (sabsan = 6 OR sabsan = 7 OR sabsan = 8 OR sabsan = 9) OR (sabsan = 5 AND sabslaja <>1)
GOTO KSM-ma06 IF ELSE

hi: 


\--------------------------------

KSM-ma06
========

tc:

vn: einkberufb; einkbab; einkmab; einkdrb

qt: Einfachauswahl mit vertikalen ao/Spaltenformat

hl:

in:

q: Was denken Sie: Wie hoch ist schätzungsweise das durchschnittliche monatliche Nettoeinkommen in Ihrem Berufsfeld mit …

is: Bitte schätzen Sie das Netto-Gehalt ungefähr ein, d. h. Einkommen abzüglich Steuer.

it1: (einkberufb): … Berufsausbildung?

it2: (einkbab): … Bachelorabschluss?

it3: (einkmab): … Masterabschluss?

it4: (einkdrb): … Promotion (Dr., PhD)?

st:

ao1: 1: unter 1.000 €

ao2: 2: 1.000 € bis unter 1.500 €

ao3: 3: 1.500 € bis unter 2.000 €

ao4: 4: 2.000 € bis unter 2.500 €

ao5: 5: 2.500 € bis unter 3.000 €

ao6: 6: 3.000 € bis unter 3.500 €

ao7: 7: 3.500 € bis unter 4.000 €

ao8: 8: 4.000 € bis unter 5.000 €

ao9: 9: 5.000 € bis unter 10.000 €

ao10: 10: 10.000 € und mehr

mv: -12:, weiß ich nicht/trifft nicht zu

ka:

vc:

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" absetzen

tr: GOTO KSM-ma07

hi:

\--------------------------------

KSM-ma07
========

tc: 

vn: mastergrund1- mastergrund13; mastergrund13o

qt: Einfachauswahlmatrix mit offener Angabe

hl:

in:

q: Es gibt Gründe, die für oder gegen ein Masterstudium sprechen. Bitte geben Sie an, inwiefern die folgenden Aussagen auf Sie persönlich zutreffen.

is:

it1: (mastergrund1): Nur mit einem Master kann ich meinen Berufswunsch erfüllen.

it2: (mastergrund2): Ein Master verbessert meine Berufsaussichten.

it3: (mastergrund3): Ein Master sichert mir ein höheres Einkommen.

it4: (mastergrund4): Ein Master besitzt ein höheres soziales Ansehen.

it5: (mastergrund5): Im Masterstudium kann ich mich persönlich entfalten.

it6: (mastergrund6): Durch ein Masterstudium kann ich den Berufseinstieg hinausschieben.

it7: (mastergrund7): Ein Masterstudium dauert mir zu lange.

it8: (mastergrund8): Ich kann mir ein Masterstudium finanziell nicht leisten. 

it9: (mastergrund9): Ein Masterstudium ist viel zu theoretisch.

it10: (mastergrund10): Ein Master ist für den Berufseinstieg unnötig. 

it11: (mastergrund11): Das Anforderungsniveau des Masters ist zu hoch.

it12: (mastergrund12): Ich will mich nicht so stark spezialisieren.

it13: (mastergrund13): Sonstiges, und zwar... [(mastergrund13o), offene Angabe, 250 Zeichen]

st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma08

hi: Reihenfolge Itemliste bitte randomisieren.


\--------------------------------

KSM-ma08
========

tc:

vn: bawert1; bawert2; bawert3

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stehen Sie zu den folgenden Aussagen bezüglich des Bachelorabschlusses?

Ein Bachelorabschluss …

is:

it1: (bawert1): … ist kein vollwertiger Hochschulabschluss, sondern vergleichbar mit
der beruflichen Ausbildung.

it2: (bawert2): … ist nur ein Zwischenschritt zu einem Masterstudium.

it3: (bawert3): … wird von Arbeitgeber*/innen als Hochschulabschluss voll anerkannt.

st:

ao1: 1: stimme überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: stimme voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO Abschlussseite

hi:
