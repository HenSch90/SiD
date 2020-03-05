

F2_6
====

tc:

vn: ainfasia; ainflandosia; ainfortosia; ainfbmsia; ainfbjsia; ainfdausia

qt: Dropdown und offene Angabe

hl:

in:

q: Sie befinden sich zurzeit im Ausland: Bitte beschreiben Sie diesen Auslandaufenthalt näher.

is:

it:

st:


ao:[Dropdown, Art des Aufenthalts]

aox (ainfasia): 0: Art des Auslandsaufenthalts 

ao1 (ainfasia): 1: Auslandsstudium mit angestrebtem Abschluss im Ausland

ao2 (ainfasia): 2: Auslandsstudium/-semester ohne angestrebten Abschluss

ao3 (ainfasia): 3: Praktikum/Praxisphase

ao4 (ainfasia): 4: Sprachkurs

ao5 (ainfasia): 5: Studienreise

ao6 (ainfasia): 6: Projektarbeit

ao7 (ainfasia): 7: Summer School

ao8 (ainfasia): 8: sonstiger Aufenthalt



ao9 (ainflandosia): Präfix: Land: [string, 100 Zeichen]

ao10 (ainfortosia): Präfix: Stadt/Hochschule: [string, 100 Zeichen]



[Nebeneinander angeordnete Dropdowns (Monat, Jahr)]

[Dropdown, Start des Auslandsaufenthalts]

ao11 (ainfbmsia): : Monat: (Monat \ Januar \| … \| Dezember)

ao12 (ainfbjsia): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2009 \| vor 2009)



[Dropdown, Dauer des Aufenthalts]

ao13: (ainfdausia): Dauer: (Dauer \| 1 Monat \| 2 Monate \| ... \| 12 Monate \| mehr als 12 Monate)

mv:

ka:(ao11 To ao12) Start des Aufenthalts

vc: SHOW ao9 AND ao10 if hsstandbl=17 AND hsstandlao=MISSING AND hsstandhsao=MISSING

av:

kh:

fv:

hv:

fo:

tr: GOTO F2_8

hi: @ZOFAR ich bin mir nicht sicher, ob deutlich wird, dass die Dropdowns für Monat und Jahr nebeneinander stehen sollen, während das Dropdown "Dauer des Aufenthalts" unter den beiden zuvor genannten stehen soll.

\--------------------------------

F2_8
====

tc:

vn: bdequasia; bdefamssia; bdeoeksia; bdefinsia; bdesprsia; bdearbsia; bdekensia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Warum haben Sie sich für dieses Land entschieden?

is: **Ich habe mich für ein Studium in diesem Land entschieden, …**

it1: (bdequasia): aufgrund der hohen Lebensqualität.

it2: (bdefamssia): weil bereits Freund\*innen/Verwandte in diesem Land studiert haben.

it3: (bdeoeksia): aufgrund der wirtschaftlichen Lage.

it4: (bdefinsia): weil dies meinen finanziellen Möglichkeiten entspricht.

it5: (bdesprsia): um meine Sprachkenntnisse zu vertiefen.

it6: (bdearbsia): um nach Studienabschluss in diesem Land zu arbeiten.

it7: (bdekensia): um dieses Land kennenzulernen.

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

hi:

\--------------------------------

F2_9
====

tc:

vn: sabsabssia

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Planen Sie im Ausland einen Hochschulabschluss zu erwerben?

is: Bitte beziehen Sie sich auf Ihren aktuellen Studiengang.

it:

st:

ao1: 1: nein

ao2: 2: Ja, ich plane einen Studienabschluss im Ausland (z. B. Bachelor, Master, Promotion).

ao3: 3: Ja, ich plane einen Doppelabschluss (Deutschland und anderes Land).

ao4: -12: weiß ich noch nicht

mv: ao4

ka:

vc:

av:

kh:

fv:

hv:

fo: ao4 absetzen

tr:

GOTO F2_10

hi:

\--------------------------------

F2_10
=====

tc:

vn: ainfcpsia

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wird Ihr gegenwärtiger Auslandsaufenthalt auf Ihr Studium in Deutschland angerechnet?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, teilweise

ao3: 3: ja, vollständig

ao4: 4: ist nicht vorgesehen

ao5: -12: weiß ich nicht

mv: ao5

ka:

vc:

av:

kh:

fv:

hv:

fo: ao5 absetzen

tr:

GOTO F2_11

hi:

\--------------------------------

F2_11
==

tc:

vn: apronosia; aproerassia; aprodaadsia; aprohhssia; aprogahssia; aproanprsia

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Findet Ihr Auslandsaufenthalt im Rahmen eines Austauschprogramms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (apronosia): nein (Exklusivkategorie)

ao2: (aproerassia): … ERASMUS+

ao3: (aprodaadsia): … DAAD-Programm

ao4: (aprohhssia): … Programm meiner Heimathochschule

ao5: (aprogahssia): … Programm der Gasthochschule in Deutschland

ao6: (aproanprsia): … anderes Programm

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

vn: afinelt; afinpar; afinbaf; afinjobv; afinjobw; afinstip; afinkre; afinand

qt: Mehrfachauswahl

hl:

in:

q: Wie finanzieren Sie Ihren studienbezogenen Auslandsaufenthalt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (afinelt): Eltern

ao2: (afinpar): Parnter\*in

ao3: (afinbaf): BAföG

ao4: (afinjobv): Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5: (afinjobw): Verdienst aus Tätigkeiten während des Auslandsaufenthalt

ao6: (afinstip): Stipendium

ao7: (afinkre): Bildungskredit

ao8: (afinand): andere Finanzierungsquelle

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

vn: akontgastsia; akonteinheimsia; akontdeustsia; akontintstsia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig unterhalten Sie sich mit…

is:

it1: (akontgastsia): … Studierenden des Gastlandes?

it2: (akonteinheimsia): … anderen Einheimischen?

it3: (akontdeustsia): … deutschen Studierenden?

it4: (akontintstsia): … anderen internationalen Studierenden?

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte eine Leerzeile zwischen Frage und Antwortitems. Im Pretest waren diese sehr nah beieinander.

tr:

GOTO F2_14

hi:

\--------------------------------

F2_14
=====

tc:

vn: asprachgaslsia; asprachheimlsia; asprachandsia; asprachandsiao

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig sprechen Sie während Ihres Auslandsaufenthalts die folgenden Sprachen?

is:

it1: (asprachgaslsia): Landessprache des Gastlandes

it2: (asprachheimlsia): Deutsch

it3: (asprachandsia): andere Sprache, und zwar: [50 Zeichen, (asprachandsiao)]

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

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

vn: azuflernerfsia; azufinsgsia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: In Bezug auf Ihren Auslandsaufenthalt: Wie zufrieden sind Sie mit …

is:

it1: (azuflernerfsia): … den im Ausland gewonnenen fachlichen Kenntnissen?

it2: (azufinsgsia): … Ihrem Auslandsaufenthalt insgesamt?

st:

ao1: 1: überhaupt nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr zufrieden

mv:

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

vn: azuforgaufwsia; azuffinanzaufwsia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und wie beurteilen Sie …

is:

it1: (azuforgaufwsia): … den organisatorischen Aufwand Ihres Aufenthaltes?

it2: (azuffinanzaufwsia): … den finanziellen Aufwand Ihres Aufenthaltes?

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

qt: Einfachauswahl mit horizontalen ao

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen: Würden Sie Ihren Freund\*innen/Bekannten empfehlen, im Ausland zu studieren?

is:

it:

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

GOTO F2_18

hi:

\--------------------------------


F2_19 
======

tc: 

vn: intpsydeusia; intpsyzeitasia; intpsydauasia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsydeusia): in Deutschland

it2: (intpsyzeitasia): zeitweise im Ausland

it3: (intpsydauasia): dauerhaft im Ausland

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

tc:

vn: intling1sia; intling2sia; intling3sia

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie zu?

is:

it1: (intling1sia): Ich kann in der Sprache meines Gastlandes über vertraute Themen sprechen und meine persönliche Meinung äußern.

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
