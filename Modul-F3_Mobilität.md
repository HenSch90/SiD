
F3_6
=====

tc:

vn: azufmob

qt: Einfachauswahl mit horizontal abgetragenen Antwortoptionen

hl:

in:

q1: Inwieweit trauen Sie es sich zu, im Ausland zu studieren?

q2: Inwieweit trauen Sie es sich zu, ein weiteres Mal im Ausland zu studieren?

is:

it:

st:

ao1: 1: 1: gar nicht

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: voll und ganz

mv:

ka:

vc:

SHOW q2 IF ainfaus ge 2

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_7 IF ainfaus>1
GOTO F3_16 IF ainfaus=1 AND auslandint=4
GOTO F3_16 IF ainfaus=MISSING AND auslandint=4
GOTO F3_21 IF ainfaus=1 AND auslandint=1,2,3
GOTO F3_21 IF ainfaus=MISSING AND auslandint=1,2,3

hi:

\--------------------------------

F3_7 
=====

tc: IF ainfaus \> 1 \| kA

vn: 
ainfa1 / ainflo1 / ainfsto1 / ainfhso1 / ainfbm1 / ainfbj1 / ainfem1 / ainfej1 / 
ainfa2 / ainflo2 / ainfsto2 / ainfhso2 / ainfbm2 / ainfbj2 / ainfem2 / ainfej2 / 
ainfa3 / ainflo3 / ainfsto3 / ainfhso3 / ainfbm3 / ainfbj3 / ainfem3 / ainfej3

qt: Tableau-Abfrage Drop-Down-Menüs, offene Angabe

hl:

in:

q1: Bitte beschreiben Sie Ihren studienbezogenen Auslandsaufenthalt näher.

q2: Bitte beschreiben Sie Ihre beiden studienbezogenen Auslandsaufenthalte näher

q3: Bitte beschreiben Sie Ihre drei studienbezogenen Auslandsaufenthalte näher.

is1: Bitte beginnen Sie mit Ihrem zuletzt durchgeführten Aufenthalt.

is2: Bitte beginnen Sie mit Ihrem zuletzt durchgeführten Aufenthalt. Sollten Sie
mehr als drei Aufenthalte haben, dann geben sie bitte den drittletzten
Aufenthalt an.

it1: (ainfa1): Art des Auslandsaufenthalts: [Drop-Down-Menü1]

it2: Land: [ainflo1] [Eingabefeld; 100 Zeichen]

it3: Stadt/Hochschule: [ainfsto1] [Eingabefeld; 100 Zeichen]

it4: ggf. Hochschule: [ainfhso1] [Eingabefeld; 100 Zeichen]

it5: (ainfbm1): Monat: [Drop-Down-Menü2]

it6: (ainfbj1): Jahr: [Drop-Down-Menü3]

it7: (ainfem1): Monat: [Drop-Down-Menü2]

it8: (ainfej1): Jahr: [Drop-Down-Menü5]

it9: (ainfa2): Art des Auslandsaufenthalts: [Drop-Down-Menü1]

it10: Land: [ainflo2] [Eingabefeld; 100 Zeichen]

it11: Stadt/Hochschule: [ainfsto2] [Eingabefeld; 100 Zeichen]

it12: ggf. Hochschule: [ainfhso2] [Eingabefeld; 100 Zeichen]

it13: (ainfbm2): Monat: [Drop-Down-Menü2]

it14: (ainfbj2): Jahr: [Drop-Down-Menü3]

it15: (ainfem2): Monat: [Drop-Down-Menü2]

it16: (ainfej2): Jahr: [Drop-Down-Menü5]

it17: (ainfa3): Art des Auslandsaufenthalts: [Drop-Down-Menü1]

it18: Land: [ainflo3] [Eingabefeld; 100 Zeichen]

it19: Stadt/Hochschule: [ainfsto3] [Eingabefeld; 100 Zeichen]

it20: ggf. Hochschule: [ainfhso3] [Eingabefeld; 100 Zeichen]

it21: (ainfbm3): Monat: [Drop-Down-Menü2]

it22: (ainfbj3): Jahr: [Drop-Down-Menü3]

it23: (ainfem3): Monat: [Drop-Down-Menü2]

it24: (ainfej3): Jahr: [Drop-Down-Menü5]

it

st:

ao:

Drop-Down-Menü1

Drop-Down-Menü2

Drop-Down-Menü3

Drop-Down-Menü4

Drop-Down-Menü5

mv:

ka1 (it2 TO it3): Land, Stadt, Hochschule des Auslandsaufenthalts:

ka2 (it4 TO it6): Start des Auslandsaufenthalts:

ka3 (it7 TO it8): Ende des Auslandsaufenthalts:

ka4 (it10 TO it11): Land, Stadt, Hochschule des Auslandsaufenthalts:

ka5 (it12 TO it14): Start des Auslandsaufenthalts:

ka6 (it15 TO it16): Ende des Auslandsaufenthalts:

ka7 (it18 TO it19): Land, Stadt, Hochschule des Auslandsaufenthalts:

ka8 (it20 TO it22): Start des Auslandsaufenthalts:

ka9 (it23 TO it24): Ende des Auslandsaufenthalts:

vc:

SHOW q1 AND it1 TO it8 AND ka1 TO ka3 IF ainfaus = 2 \| kA

SHOW q2 AND is1 AND it1 TO it13 AND it16 AND ka1 TO ka6 IF ainfaus = 3

SHOW q3 AND is2 AND it1 TO it24 AND ka1 TO ka9 IF ainfaus = 4

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_8

hi:

\--------------------------------

F3_8
====

tc: IF ainfaus \> 1 \| kA

vn: aproselb1 / aproeras1 / aproapeu1 / aprodaad1 / apropad1 / apropromos1 /
aprodths1 / aprogahs1 / aproanpr1 / aproselb2 / aproeras2 / aproapeu2 /
aprodaad2 / apropad2 / apropromos2 / aprodths2 / aprogahs2 / aproanpr2 /
aproselb3 / aproeras3 / aproapeu3 / aprodaad3 / apropad3 / apropromos3 /
aprodths3 / aprogahs3 / aproanpr3

qt: Mehrfachnennung, Akkordeon je Aufenthalt

hl:

in:

q1: Fand Ihr Auslandsaufenthalt im Rahmen eines Programms statt?

q2: Fanden Ihre Auslandsaufenthalte im Rahmen eines Programms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aproselb1): Nein, ich habe den Aufenthalt selbst organisiert. [EK]

ao2: (aproeras1): ja, ERASMUS+, ERASMUS

ao3: (aproapeu1): ja, anderes EU-Programm

ao4: (aprodaad1): ja, DAAD-Programm

ao5: (apropad1): ja, Pädagogischer Austauschdient (PAD)/COMENIUS

ao6: (apropromos1): ja, PROMOS-Stipendium

ao7: (aprodths1): ja, Programm meiner Hochschule in Deutschland

ao8: (aprogahs1): ja, Programm meiner Gasthochschule im Ausland

ao9: (aproanpr1): ja, anderes Programm, und zwar [Eingabefeld; 100 Stellen]

ao10: (aproselb2): Nein, ich habe den Aufenthalt selbst organisiert. [EK]

ao11: (aproeras2): ja, ERASMUS+, ERASMUS

ao12: (aproapeu2): ja, anderes EU-Programm

ao13: (aprodaad2): ja, DAAD-Programm

ao14: (apropad2): ja, Pädagogischer Austauschdient (PAD)/COMENIUS

ao15: (apropromos2): ja, PROMOS-Stipendium

ao16: (aprodths2): ja, Programm meiner Hochschule in Deutschland

ao17: (aprogahs2): ja, Programm meiner Gasthochschule im Ausland

ao18: (aproanpr2): ja, anderes Programm, und zwar [Eingabefeld; 100 Stellen]

ao19: (aproselb3): Nein, ich habe den Aufenthalt selbst organisiert. [EK]

ao20: (aproeras3): ja, ERASMUS+, ERASMUS

ao21: (aproapeu3): ja, anderes EU-Programm

ao22: (aprodaad3): ja, DAAD-Programm

ao23: (apropad3): ja, Pädagogischer Austauschdient (PAD)/COMENIUS

ao24: (apropromos3): ja, PROMOS-Stipendium

ao25: (aprodths3): ja, Programm meiner Hochschule in Deutschland

ao26: (aprogahs3): ja, Programm meiner Gasthochschule im Ausland

ao27: (aproanpr3): ja, anderes Programm, und zwar [Eingabefeld; 100 Stellen]

mv:

ka1 (ao1 TO ao9): Aufenthalt A: [Art Aufenthalt, Land, Beginn]

ka2 (ao10 TO ao18): Aufenthalt B: [Art Aufenthalt, Land, Beginn]

ka3 (ao19 TO ao27): Aufenthalt C: [Art Aufenthalt, Land, Beginn]

vc:

SHOW q1 AND ao1 TO ao9 AND ka1 IF 1 Aufenthalt

SHOW q2 AND ao1 TO ao18 AND ka1 TO ka2 IF 2 Aufenthalte

SHOW q2 AND ao1 TO ao27 AND ka1 TO ka3 IF 3 Aufenthalte

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_9

hi:

\--------------------------------

F3_9 
=====

tc: IF ainfaus \> 1 \| kA

vn: ainfcp / ainfcpteilo / ainfcpvollo

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Wurde Ihr letzter Auslandsaufenthalt auf Ihr Studium angerechnet, z. B. in
Form von ECTS-Punkten?

is:

it:

st:

ao1: 1: : Nein

ao2: 2: : ja, teilweise: [ainfcpteilo] [Eingabefeld; 2 Stellen] ECTS-Punkte

ao3: 3: : ja, vollständig: [ainfcpvollo] [Eingabefeld; 2 Stellen] ECTS-Punkte

ao4: -12: : weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F3_10

hi:

\--------------------------------

F3_10
=====

tc: IF ainfaus \> 1 \| k.A.

vn: 
afinelt1 / afinpar1 / afinbaf1 / afinjobv1 / afinjobw1 / afinstip1 / afinand1 / 
afinelt2 / afinpar2 / afinbaf2 / afinjobv2 / afinjobw2 / afinstip2 / afinand2 / 
afinelt3 / afinpar3 / afinbaf3 / afinjobv3 / afinjobw3 / afinstip3 / afinand3

qt: Mehrfachnennung, Akkordeon

hl:

in:

q1: Wie haben Sie ihren Auslandsaufenthalt finanziert?

q2: Wie haben Sie ihre Auslandsaufenthalte finanziert?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (afinelt1): Eltern

ao2 (afinpar1): Partner(in)

ao3 (afinbaf1): BAföG

ao4 (afinjobv1): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5 (afinjobw1): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao6 (afinstip1): Stipendium

ao7 (afinand1): andere Finanzierungsquelle

ao8 (afinelt2): Eltern

ao9 (afinpar2): Partner(in)

ao10 (afinbaf2): BAföG

ao11 (afinjobv2): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao12 (afinjobw2): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao13 (afinstip2): Stipendium

ao14 (afinand2): andere Finanzierungsquelle

ao15 (afinelt3): Eltern

ao16 (afinpar3): Partner(in)

ao17 (afinbaf3): BAföG

ao18 (afinjobv3): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao19 (afinjobw3): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao20 (afinstip3): Stipendium

ao21 (afinand3): andere Finanzierungsquelle

mv:

ka1 (ao1 TO ao7) : Aufenthalt A: [Art Aufenthalt, Land, Beginn]

ka2 (ao8 TO ao14): Aufenthalt B: [Art Aufenthalt, Land, Beginn]

ka3 (ao15 TO ao21): Aufenthalt C: [Art Aufenthalt, Land, Beginn]

vc:

SHOW q1 AND ao1 TO ao7 AND ka1 IF 1 Aufenthalt

SHOW q2 AND ao1 TO ao14 AND ka1 TO ka2 IF 2 Aufenthalte

SHOW q2 AND ao1 TO ao21 AND ka1 TO ka3 IF 3 Aufenthalte

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_11

hi:

\--------------------------------

F3_11 
======

tc: IF ainfaus \> 1 \| k.A.

vn: akontdeust / akontgast / akonteinheim / akontintst

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q1: Wie häufig hatten Sie während Ihres studienbezogenen Auslandsaufenthalts
Kontakt …

q2: Wie häufig hatten Sie während Ihres letzten studienbezogenen
Auslandsaufenthalts Kontakt mit…

is:

it1: (akontdeust): … Studierenden aus Deutschland?

it2: (akontgast): … Studierenden des Gastlandes?

it3: (akonteinheim): … anderen Einheimischen?

it4: (akontintst): … anderen internationalen Studierenden (nicht aus
Deutschland)?

st:

ao1: 1: : nie

ao2: 2: : selten

ao3: 3: : manchmal

ao4: 4: : häufig

ao5: 5: : sehr häufig

mv:

ka:

vc:

SHOW q1 IF ainfaus = 2 \| kA

SHOW q2 IF ainfaus \> 2

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_12

hi:

\--------------------------------

F3_12 
======

tc: IF ainfaus \> 1 \| k.A.

vn: asprachland / asprachdeut / asprachand / asprachando

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q1: Wie häufig haben Sie während Ihres Auslandsaufenthalts die folgenden
Sprachen gesprochen?

q2: Wie häufig haben Sie während Ihres letzten Auslandsaufenthalts die folgenden
Sprachen gesprochen?

is:

it1: (asprachland): Landessprache

it2: (asprachdeut): Deutsch

it3: (asprachand): Andere Sprache, und zwar [asprachando] [Eingabefeld, 50 Stellen]

st:

ao1: 1: : nie

ao2: 2: : selten

ao3: 3: : manchmal

ao4: 4: : häufig

ao5: 5: : sehr häufig

mv:

ka:

vc:

SHOW q1 IF ainfaus = 2 \| kA

SHOW q2 IF ainfaus \> 2

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_13

hi:

\--------------------------------

F3_13 
======

tc: IF ainfaus \> 1 \| kA

vn: azufskein / azufskstu / azufsklehr / azuflernerf / azufinsg

qt: Akkordeon

hl:

in:

q: Wie zufrieden sind Sie in Bezug auf Ihren letzten studienbezogenen
Auslandsaufenthalt mit …

is:

it1: (azufskein): … dem Kontakt zu Einheimischen?

it2: (azufskstu): … dem Kontakt zu Studierenden?

it3: (azufsklehr): … dem Kontakt zu Lehrenden?

it4: (azuflernerf): … den gewonnen fachlichen Kenntnissen?

it5: (azufinsg): … dem Auslandsaufenthalt insgesamt?

st:

ao1: 1: 1: überhaupt nicht zufrieden

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr zufrieden

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_14

hi:

\--------------------------------

F3_14 
======

tc: IF ainfaus \> 1 \| kA

vn: azufleistanf / azuforgaufw / azuffinanzaufw

qt: Akkordeon

hl:

in:

q: In Bezug auf Ihren letzten studienbezogenen Auslandsaufenthalt: Wie
beurteilen Sie…

is:

it1: (azufleistanf): … die Leistungsanforderungen?

it2: (azuforgaufw): … den organisatorischen Aufwand?

it3: (azuffinanzaufw): … den finanziellen Aufwand?

st:

ao1: 1: 1: sehr niedrig

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr hoch

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_15

hi:

\--------------------------------

F3_15
=====

tc:

vn: aeempf

qt: Einfachauswahl vertikale ao

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen:

Würden Sie einen studienbezogenen Auslandsaufenthalt empfehlen?

is:

it:

st:

ao1: 1: 1: nein überhaupt nicht

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: ja, unbedingt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_22

hi:

\-------------------------------- 

F3_16
=====

tc: Die Frage erhalten ausschließlich Studierende, die beabsichtigen einen
(weiteren) Auslandsaufenthalt durchzuführen (s. Grundprogramm).

vn: aplanstg / aplantst / aplanpra / aplanspk / aplanstureis / aplanprojekt /
aplansumschoo / aplanson / aplanwnn

qt: Mehrfachnennung

hl:

in:

q: Sie haben angegeben, dass sie einen (weiteren) studienbezogenen
Auslandsaufenthalt künftig beabsichtigen durchzuführen:

Welche Art von Aufenthalt planen Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (aplanstg): Auslandsstudium mit Erwerb eines Abschlusses im Ausland (z. B.
Masterstudium)

ao2 (aplantst): Teilstudium im Ausland (Auslandssemester)

ao3 (aplanpra): Auslandspraktikum

ao4 (aplanspk): Sprachkurs im Ausland

ao5 (aplanstureis): Studienreise

ao6 (aplanprojekt): Projektarbeit

ao7 (aplansumschoo): Summerschool

ao8 (aplanson): sonstiger Auslandsaufenthalt

ao9 (aplanwnn): weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_17

hi:

\--------------------------------

F3_17
=====

tc: Die Frage erhalten ausschließlich Studierende, die beabsichtigen einen
(weiteren) Auslandsaufenthalt durchzuführen.

vn: aplanlasta / aplanlao / aplanstao

qt: Einfachauswahl, offene Angabe

hl:

in:

q: In welchem Land und in welcher Stadt/Hochschule planen Sie den
Auslandsaufenthalt durchzuführen?

is:

it:

st:

ao1: 100 Stellen; Präfix: Land:

ao2: 100 Stellen; Präfix: Stadt/Hochschule:

ao3: -12: : weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_19

hi:

\--------------------------------

F3_19
=====

tc: Die Frage erhalten ausschließlich Studierende, die beabsichtigen einen
(weiteren) Auslandsaufenthalt durchzuführen.

vn: aplanföpro; aplanföproo

qt: Einfachauswahl

hl:

in:

q: Auf welche Weise planen Sie Ihren künftigen Auslandsaufenthalt zu
organisieren?

is:

it:

st:

ao1: 1: : … ja, ERASMUS+, ERASMUS

ao2: 2: : … ja, anderes EU-Programm

ao3: 3: : … ja, DAAD-Programm

ao4: 4: : … ja, Pädagogischer Austauschdient (PAD)/COMENIUS

ao5: 5: : … ja, PROMOS-Stipendium

ao6: 6: : … ja, Programm meiner Hochschule in Deutschland

ao7: 7: : … ja, Programm meiner Gasthochschule im Ausland

ao8: 8: : … ja, anderes Programm, und zwar [aplanföproo] [Eingabefeld; 100 Stellen]

[Leerzeile]

ao9: 9: : nein, werde Aufenthalt selbst organisieren [EK]

mv:

ka (ao1 TO ao8) : Der Aufenthalt findet im Rahmen eines Austauschprogramms statt

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_20

hi: ao9 bitte optisch von restlicher Itemliste absetzen

\--------------------------------

F3_20
=====

tc: Die Frage erhalten ausschließlich Studierende, die beabsichtigen einen
(weiteren) Auslandsaufenthalt durchzuführen.

vn: aplfinelt / aplfinpar / aplfinbaf / aplfinjobv / aplfinjobw / aplfinstip /
aplfinand

qt: Mehrfachnennung

hl:

in:

q: Wie werden Sie Ihren studienbezogenen Auslandsaufenthalt voraussichtlich
finanzieren?

is:

it:

st:

ao1 (aplfinelt): Eltern

ao2 (aplfinpar): Partner*in

ao3 (aplfinbaf): BAföG

ao4 (aplfinjobv): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5 (aplfinjobw): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao6 (aplfinstip): Stipendium

ao7 (aplfinand): andere Finanzierungsquelle

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_22

hi:

\--------------------------------

F3_21
=====

tc: Die Frage erhalten ausschließlich Studierende, die nicht studienbezogen im
Ausland waren und auch nicht beabsichtigen einen Auslandsaufenthalt
durchzuführen

vn: aplanbedi; aplanbedio

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Gibt es Umstände, unter denen ein Auslandsstudium für Sie doch in Frage
kommen würde?

is:

it:

st:

ao1: 1: : nein

ao2: 2: : ja, und zwar wenn … [aplanbedio] [Eingabefeld; 200 Stellen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_22

hi:

\--------------------------------

F3_22
=====

tc:

vn: akontdeust; akonteust; akontneust

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q: Wie häufig unterhalten Sie sich mit…

is:

it1: (akontdeust): … Studierenden aus Deutschland

it2: (akonteust): … Studierenden aus anderen Ländern Europas

it3: (akontneust): … Studierenden aus Ländern außerhalb Europas

st:

ao1: 1: 1: sehr selten

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_23

hi:

\--------------------------------

F3_23
=====

tc:

vn: wohnemin / wohnemino

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Wie viel Zeit benötigen Sie für den einfachen Weg von Ihrer Wohnung zur
Hochschule?

is: Bitte geben Sie die Dauer des Weges „von Tür zu Tür“ an.

it:

st:

ao1: 3 Stellen; Präfix: Dauer:; Suffix: Minuten

ao2: -12: : weiß ich nicht [EK]

mv:

ka:

vc:

av: number : \<= dreistellig : 1 TO 999

kh: Bitte geben Sie die Dauer des einfachen Weges von Ihrer Wohnung zu Ihrer
Hochschule an (1 bis 999).

fv:

hv:

fo:

tr:

GOTO F3_24

hi:

\--------------------------------

F3_24
=====

tc:

vn: mobregmittel

qt: Einfachauswahl

hl:

in:

q: Welches Verkehrsmittel nutzen Sie überwiegend um an Ihre Hochschule zu
gelangen?

is: Bei kombinierter Nutzung geben Sie bitte das Verkehrsmittel an, mit dem Sie
die längste Wegstrecke zurücklegen.

it:

st:

ao1: 1: : ich gehe zu Fuß

ao2: 2: : Fahrrad

ao3: 3: : öffentliche Verkehrsmittel

ao4: 4: : PKW (allein fahrend)

ao5: 5: : PKW (in Fahrgemeinschaft)

ao6: 6: : anderes

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_25

hi:

\--------------------------------

F3_25
=====

tc:

vn: intpsydeu / intpsyzeit / intpsyandl

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsydeu): In Deutschland

it2: (intpsyzeitl): Zeitweise im Ausland

it3: (intpsyandl): Dauerhaft im Ausland

st:

ao1: 1: 1: auf keinen Fall

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: auf jeden Fall

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_56

hi:
