
F2_6
====

tc:

vn: ainfasia; ainfbmsia; ainfbjsia; ainfemsia; ainfejsia

qt: Tableau-Abfrage Drop-Down-Menü

hl:

in:

q: Sie befinden sich zurzeit im Ausland: Bitte beschreiben Sie Ihren aktuellen studienbezogenen 
Auslandsaufenthalt näher.

is:

it:

st:

Art des Auslandsaufenthalts: 
Drop-Down-Menü

aox (ainfasia): 0: Art des Auslandsaufenthalts 

ao1 (ainfasia): 1: Auslandsstudium mit angestrebtem Abschluss im Ausland

ao2 (ainfasia): 2: Auslandsstudium/-semester ohne angestrebten Abschluss

ao3 (ainfasia): 3: Praktikum/Praxisphase

ao4 (ainfasia): 4: Sprachkurs

ao5 (ainfasia): 5: Studienreise

ao6 (ainfasia): 6: Projektarbeit

ao7 (ainfasia): 7: Summer School

ao8 (ainfasia): 8: sonstiger Aufenthalt


Untereinander angeordnete Drop-Down-Menüs

Start des Auslandsaufenthalts

ao9 (ainfbmsia): : Monat: (Monat \ Januar \| … \| Dezember)

ao10 (ainfbjsai): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2009 \| vor 2009)


Untereinander angeordnete Drop-Down-Menüs

voraussichtliches Ende des Auslandsaufenthalts

ao11 (ainfemsia): : Monat: (Monat \ Januar \| … \| Dezember)

ao12 (ainfejsia): Jahr: (Jahr \ 2018 \| 2019 \| … \| 2030)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

<zofar:transition target="F2_7" condition="(zofar.asNumber(ainfasia) ge 3 or zofar.asNumber(ainfasia) le 8) or      ((zofar.asNumber(ainfasia)==1 or zofar.asNumber(ainfasia)==2) and (!hsstand_2.value or (zofar.asNumber(hsstandbl) ge 1 and zofar.asNumber(hsstandbl) le 16)))"/>
            <zofar:transition target="F2_7" condition="(zofar.asNumber(ainfasia)==1 or zofar.asNumber(ainfasia)==2) and zofar.isMissing(hsstandlao)"/>
            <zofar:transition target="F2_8"/>

hi:

\--------------------------------

F2_7
====

tc:

vn: hsstandlao; hsstandsto; hsstandhso

qt: offene Angabe

hl:

in:

q: Bitte tragen Sie das Land, den Ort sowie ggf. die Hochschule ein, an der Sie aktuell im Ausland studieren.

is:

it:

st:

ao1: 70 Stellen, Präfix (hsstandlao), Suffix: [Land]

ao2: 70 Stellen, Präfix (hsstandsto), Suffix: [Ort]

ao1: 70 Stellen, Präfix (hsstandhso), Suffix: [Hochschule]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_8

hi:


\--------------------------------

F2_8
====

tc:

vn: bdefinsia; bdekensia; bdesprsia; bdefamssia; bdefamlsia; bdetecsia;
bdeoeksia; bdepolsia; bdequasia; bdearbsia; fehlt; fehlto

qt: Einfachauswahlmatrix mit offener Angabe

hl:

in:

q: Warum haben Sie sich für dieses Land entschieden?

is:

Überschrift: Ich habe mich für ein Studium in diesem Land entschieden, …

it1: (bdefinsia): …weil ein Studium in diesem Land meinen finanziellen
Möglichkeiten entspricht.

it2: (bdekensia): …um dieses Land kennenzulernen/weil mich die Geschichte und
Kultur des Landes interessiert.

it3: (bdesprsia): …um meine Sprachkenntnisse zu vertiefen.

it4: (bdefamssia): …weil Freunde/Verwandte in diesem Land studieren/studiert
haben.

it5: (bdefamlsia): …weil Freunde/Verwandte in diesem Land leben/gelebt haben.

it6: (bdetecsia): …weil dieses Land ein hochtechnisiertes Land ist.

it7: (bdeoeksia): …wegen der wirtschaftlichen Lage in diesem Land.

it8: (bdepolsia): …wegen der politischen Lage in diesem Land.

it9: (bdequasia): …wegen der Lebensqualität in diesem Land.

it10: (bdearbsia): …aufgrund der Möglichkeiten, nach Studienabschluss in diesem
Land zu arbeiten.

it11: (fehlt): …anderer Grund und zwar: [fehlto, 100 Zeichen]

st:

ao1: 1: trifft gar nicht zu

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

tr:

GOTO F2_9

hi: Items bitte zufällig rotieren.

\--------------------------------

F2_9
====

tc:

vn: ainfastsia

qt: Einfachauswahl

hl:

in:

q: Beabsichtigen Sie im Ausland einen Abschluss zu erwerben?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, sowohl an der ausländischen als auch der deutschen Hochschule

ao3: 3: ja, nur an der ausländischen Hochschule

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_10

hi:

\--------------------------------

F2_10
=====

tc:

vn: ainfcpsia; ainfcp1osia; ainfcp2osia

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Wird Ihr gegenwärtiger Auslandsaufenthalt auf Ihr Studium in Deutschland angerechnet?

is:

it:

st:

ao1: 1: nein

ao2: 2: offene Angabe: 2 Stellen Präfix: ja, teilweise [ainfcp1osia], Suffix: ECTS-Punkte

ao3: 3: offene Angabe: 2 Stellen Präfix: ja, vollständig [ainfcp2osia], Suffix: ECTS-Punkte

ao1: 4: weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_11

hi:

\--------------------------------

F2_11
==

tc:

vn: aproselbsia; aproerassia; aproapeusia; aprodaadsia; apropadsia;
apropromossia; aprodthssia; aprogahssia; aproanprsia; aproanprosia

qt: Mehrfachnennung mit Exklusivkategorie

hl:

in:

q: Findet Ihr Auslandsaufenthalt im Rahmen eines Austauschprogramms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aproselbsia): nein, habe Aufenthalt selbst organisiert (Exklusivkategorie)

ao2: (aproerassia): ja, ERASMUS+, ERASMUS

ao3: (aproapeusia): ja, anderes EU-Programm

ao4: (aprodaadsia): ja, DAAD-Programm

ao5: (apropadsia): ja, Pädagogischer Austauschdienst (PAD)/COMENIUS

ao6: (apropromossia): ja, PROMOS-Stipendium

ao7: (aprodthssia): ja, Programm meiner Hochschule in Deutschland

ao8: (aprogahssia): ja, Programm meiner Gasthochschule im Ausland

ao9: (aproanprsia): ja, anderes Programm und zwar: offene Angabe: 100 Stellen, Präfix
[aproanprosia], Suffix

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_12

hi:

\--------------------------------

F2_12
=====

tc:

vn: afinelt; afinpar; afinbaf; afinjobv; afinjobw; afinstip; afinand

qt: Mehrfachnennung

hl:

in:

q: Wie finanzieren Sie Ihren studienbezogenen Auslandsaufenthalt?

is: Bitte alles Zutreffende auswählen

it:

st:

ao1: (afinelt): Eltern

ao2: (afinpar): Parnter\*In

ao3: (afinbaf): BAföG

ao4: (afinjobv): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5: (afinjobw): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao6: (afinstip): Stipendium

ao7: (afinand): andere Finanzierungsquelle

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_13

hi:

\--------------------------------

F2_13
=====

tc:

vn: akontdeustsia; akontgastsia; akonteinheimsia; akontintstsia

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig haben Sie während Ihres Auslandsaufenthalts Kontakt mit…

is:

it1: (akontdeustsia): … Studierenden aus Deutschland?

it2: (akontgastsia): … Studierenden des Gastlandes?

it3: (akonteinheimsia): … anderen Einheimischen?

it4: (akontintstsia): … anderen internationalen Studierenden (nicht aus
Deutschland)?

st:

ao1: 1: nie

ao2: 2: selten

ao3: 3: manchmal

ao4: 4: häufig

ao5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_14

hi:

\--------------------------------

F2_14
=====

tc:

vn: asprachlandsia; asprachdeutsia; asprachandsia; asprachandosia

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig sprechen Sie während Ihres Auslandsaufenthalts die folgenden Sprachen?

is:

it1: (asprachlandsia): Landessprache des Gastlandes

it2: (asprachdeutsia): Deutsch

it3: (asprachandsia): Andere Sprache, und zwar (offene Angabe: 50 Stellen, Präfix
[asprachandosia], Suffix

st:

ao1: 1: nie

ao2: 2: selten

ao3: 3: manchmal

ao4: 4: häufig

ao5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_15

hi:

\--------------------------------

F2_15
=====

tc:

vn: azufskein; azufskstu; azufsklehr; azuflernerf; azufinsg

qt: Einfachauswahlmatrix

hl:

in:

q: In Bezug auf Ihren Auslandsaufenthalt: Wie zufrieden sind Sie mit …

is:

it1: (azufskein): … dem Kontakt zu Einheimischen?

it2: (azufskstu): … dem Kontakt zu Studierenden?

it3: (azufsklehr): … dem Kontakt zu Lehrenden?

it4: (azuflernerf): … den gewonnenen fachlichen Kenntnissen?

it5: (azufinsg): … dem Auslandsaufenthalt insgesamt?

st:

ao1: 1: überhaupt nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr zufrieden

ao6: 6: trifft nicht zu

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_16

hi:

\--------------------------------

F2_16
=====

tc:

vn: azufleistanf; azuforgaufw; azuffinanzaufw

qt: Einfachauswahlmatrix (Akkordeon)

hl:

in:

q: Und wie beurteilen Sie …

is:

it1: (azufleistanf): … die Leistungsanforderungen an Ihrer Hochschule?

it2: (azuforgaufw): … den organisatorischen Aufwand Ihres Aufenthaltes?

it3: (azuffinanzaufw): … den finanziellen Aufwand Ihres Aufenthaltes?

st:

ao1: 1: sehr niedrig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr hoch

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_17

hi:

\--------------------------------

F2_17
=====

tc:

vn: aeempfsia

qt: Einfachauswahl mit horizontalen aos

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen:
Würden Sie einen studienbezogenen Auslandsaufenthalt empfehlen?

is:

it:

st:

ao1: 1: nein, überhaupt nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: ja, unbedingt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_18

hi:

\--------------------------------

F2_18
=====

tc:

vn: bdedarlosia; bdedarhsosia 

qt: Einfachauswahl, offene Angabe

hl:

in:

q:  Wenn Sie die freie Wahl hätten, wo würden Sie am liebsten studieren?
is:

it:

st:

ao1:  Land: (offene Angabe, Präfix [bdedarlosia]),
Suffix:

ao2: Ort/Hochschule: (offene Angabe, Präfix [bdedarhsosia]), 
Suffix:


mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_19

hi:

\--------------------------------

F2_19 
======

tc: IF (nur für Studierende, die sich aktuell studienbezogen im Ausland
befinden)

vn: intpsydeu; intpsyzeitl; intpsyandl

qt: Einfachauswahlmatrix

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsydeu): in Deutschland

it2: (intpsyzeitl): zeitweise im Ausland

it3: (intpsyandl): dauerhaft im Ausland

st:

ao1: 1: auf keinen Fall

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: auf jeden Fall

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F2_20

hi:

\--------------------------------

F2_20
=====

tc: IF (nur für Studierende, die sich aktuell studienbezogen im Ausland
befinden)

vn: intling1sia; intling2sia; intling3sia

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie zu?

is:

it1: (intling1sia): Ich kann in der Sprache meines Gastlandes über vertraute Themen sprechen
und meine persönliche Meinung äußern.

it2: (intling2sia): Ich verstehe die wichtigsten Punkte in den einheimischen Radio- und Fernsehprogrammen.

it3: (intling3sia): Ich kann einheimische Zeitungsartikel lesen und verstehen.

st:

ao1: 1: trifft gar nicht zu

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

tr:

GOTO A_56
hi:
