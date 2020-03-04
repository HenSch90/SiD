
F3_6
=====

tc:

vn: azufmob

qt: Einfachauswahl mit horizontalen aos

hl:

in:

q1: Trauen Sie sich zu, ein Studium im Ausland zu absolvieren?

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

GOTO F3_7 IF ainfaus>1
GOTO F3_16 IF ainfaus=1 AND auslandint=4
GOTO F3_16 IF ainfaus=MISSING AND auslandint=4
GOTO F3_21 IF ainfaus=1 AND auslandint=1 | 2 | 3
GOTO F3_21 IF ainfaus=MISSING AND auslandint=1 | 2 | 3
GOTO F3_21 IF ainfaus=MISSING AND auslandint=MISSING
hi:

\--------------------------------

F3_7 
=====

tc: 

vn: ainfa1; ainflando1; ainforto1; ainfbm1; ainfbj1, ainfdau1
    ainfa2; ainflando2; ainforto2; ainfbm2; ainfbj2, ainfdau2
    ainfa3; ainflando3; ainforto3; ainfbm3; ainfbj3, ainfdau3

qt: Dropdown und offene Angabe

hl:

in:

q1: Bitte beschreiben Sie Ihren studienbezogenen Auslandsaufenthalt näher.

q2: Bitte beschreiben Sie Ihre beiden studienbezogenen Auslandsaufenthalte näher.

q3: Bitte beschreiben Sie Ihre drei studienbezogenen Auslandsaufenthalte näher.

is1: Bitte beginnen Sie mit Ihrem letzten studienbezogenen Auslandsaufenthalt.

is2: Bitte beginnen Sie mit Ihrem letzten studienbezogenen Auslandsaufenthalt. Sollten Sie bereits häufiger als dreimal studienbezogen im Ausland gewesen sein, dann geben Sie bitte nur die drei letzten Aufenthalte an.



it1: (ainfa1): [Dropdown, Art des Aufenthalts]

aox (ainfa1): 0: Art des Auslandsaufenthalts

ao1 (ainfa1): 1: Auslandsstudium mit angestrebtem Abschluss im Ausland

ao2 (ainfa1): 2: Auslandsstudium/-semester ohne angestrebten Abschluss

ao3 (ainfa1): 3: Praktikum/Praxisphase

ao4 (ainfa1): 4: Sprachkurs

ao5 (ainfa1): 5: Studienreise

ao6 (ainfa1): 6: Projektarbeit

ao7 (ainfa1): 7: Summer School

ao8 (ainfa1): 8: sonstiger Aufenthalt


it2: (ainflando1): Präfix: Land: [string, 100 Zeichen]

it3: (ainforto1): Präfix: Stadt/Hochschule: [string, 100 Zeichen]


[Nebeneinander angeordnete Dropdowns (Monat, Jahr)]

it4: (ainfbm1): : Monat: (Monat \ Januar \| … \| Dezember)

it5: (ainfbj1): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2009 \| vor 2009)


[Dropdown, Dauer des Aufenthalts]

it6: (ainfdau1): Dauer: (Dauer \| 1 Monat \| 2 Monate \| ... \| 12 Monate \| mehr als 12 Monate)



it7: (ainfa2): [Dropdown, Art des Aufenthalts]

aox (ainfa2): 0: Art des Auslandsaufenthalts

ao9 (ainfa2): 1: Auslandsstudium mit angestrebtem Abschluss im Ausland

ao10 (ainfa2): 2: Auslandsstudium/-semester ohne angestrebten Abschluss

ao11 (ainfa2): 3: Praktikum/Praxisphase

ao12 (ainfa2): 4: Sprachkurs

ao13 (ainfa2): 5: Studienreise

ao14 (ainfa2): 6: Projektarbeit

ao15 (ainfa2): 7: Summer School

ao16 (ainfa2): 8: sonstiger Aufenthalt


it8: (ainflando2): Präfix: Land: [string, 100 Zeichen]

it9: (ainforto2): Präfix: Stadt/Hochschule: [string, 100 Zeichen]


[Nebeneinander angeordnete Dropdowns (Monat, Jahr)]

it10: (ainfbm2): : Monat: (Monat \ Januar \| … \| Dezember)

it11: (ainfbj2): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2009 \| vor 2009)


[Dropdown, Dauer des Aufenthalts]

it12: (ainfdau2): Dauer: (Dauer \| 1 Monat \| 2 Monate \| ... \| 12 Monate \| mehr als 12 Monate)



it13: (ainfa3): [Dropdown, Art des Aufenthalts]

aox (ainfa3): 0: Art des Auslandsaufenthalts

ao17 (ainfa3): 1: Auslandsstudium mit angestrebtem Abschluss im Ausland

ao18 (ainfa3): 2: Auslandsstudium/-semester ohne angestrebten Abschluss

ao19 (ainfa3): 3: Praktikum/Praxisphase

ao20 (ainfa3): 4: Sprachkurs

ao21 (ainfa3): 5: Studienreise

ao22 (ainfa3): 6: Projektarbeit

ao23 (ainfa3): 7: Summer School

ao24 (ainfa3): 8: sonstiger Aufenthalt


it14: (ainflando3): Präfix: Land: [string, 100 Zeichen]

it15: (ainforto3): Präfix: Stadt/Hochschule: [string, 100 Zeichen]


[Nebeneinander angeordnete Dropdowns (Monat, Jahr)]

it16: (ainfbm3): : Monat: (Monat \ Januar \| … \| Dezember)

it17: (ainfbj3): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2009 \| vor 2009)


[Dropdown, Dauer des Aufenthalts]

it18: (ainfdau3): Dauer: (Dauer \| 1 Monat \| 2 Monate \| ... \| 12 Monate \| mehr als 12 Monate)

st:

ao:

mv:

ka1 (it1 TO it6): letzter studienbezogener Auslandsaufenthalt

ka2 (it4 TO it6): Start und Dauer des Auslandsaufenthalts:

ka3 (it7 TO it12): Vorletzter studienbezogener Auslandsaufenthalt

ka4 (it10 TO it12): Start und Dauer des Auslandsaufenthalts:

ka5 (it13 TO it18): Drittletzter studienbezogener Auslandsaufenthalt

ka6 (it16 TO it18): Start und Dauer des Auslandsaufenthalts:


vc:

SHOW q1 AND it1 TO it6 AND ka1 TO ka2 IF ainfaus = 2 \| kA

SHOW q2 AND is1 AND it1 TO it12 AND ka1 TO ka4 IF ainfaus = 3

SHOW q3 AND is2 AND it1 TO it18 AND ka1 TO ka6 IF ainfaus = 4

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_8

\--------------------------------

F3_8
====

tc: 

vn: aprono1; aproeras1; aprodaad1; aprohhs1; aprogahs1; aproanpr1
    aprono2; aproeras2; aprodaad2; aprohhs2; aprogahs2; aproanpr2
    aprono3; aproeras3; aprodaad3; aprohhs3; aprogahs3; aproanpr3

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q1: Fand Ihr Auslandsaufenthalt im Rahmen eines Programms statt?

q2: Fanden Ihre Auslandsaufenthalte im Rahmen eines Programms statt?

is: Bitte beginnen Sie mit Ihrem zuletzt durchgeführten Aufenthalt. Sollten Sie mehr als drei Aufenthalte haben, dann geben sie bitte den drittletzten Aufenthalt an.

it:

st:

ao1: (aprono1): nein (Exklusivkategorie)

ao2: (aproeras1): ERASMUS+, ERASMUS

ao3: (aprodaad1): DAAD-Programm

ao4: (aprohhs1): Programm meiner Heimathochschule

ao5: (aprogahs1): Programm der Gasthochschule in Deutschland

ao6: (aproanpr1): anderes Programm


ao7: (aprono2): nein (Exklusivkategorie)

ao8: (aproeras2): ERASMUS+, ERASMUS

ao9: (aprodaad2): DAAD-Programm

ao10: (aprohhs2): Programm meiner Heimathochschule

ao11: (aprogahs2): Programm der Gasthochschule in Deutschland

ao12: (aproanpr2): anderes Programm


ao13: (aprono3): nein (Exklusivkategorie)

ao14: (aproeras3): ERASMUS+, ERASMUS

ao15: (aprodaad3): DAAD-Programm

ao16 (aprohhs3): Programm meiner Heimathochschule

ao17: (aprogahs3): Programm der Gasthochschule in Deutschland

ao18: (aproanpr3): anderes Programm

mv:

ka1 (ao1 TO ao6): Letzter studienbezogener Auslandsaufenthalt

ka2 (ao7 TO ao12): Vorletzter studienbezogener Auslandsaufenthalt

ka3 (ao13 TO ao18): Drittletzter studienbezogener Auslandsaufenthalt

vc:

SHOW q1 AND ao1 TO ao6 AND ka1 IF 1 Aufenthalt (ainfaus > 1)

SHOW q2 AND ao1 TO ao16 AND ka1 TO ka2 IF 2 Aufenthalte (ainfaus > 2)

SHOW q2 AND is AND ao1 TO ao18 AND ka1 TO ka3 IF 3 Aufenthalte (ainfaus > 3)

av:

kh:

fv:

hv:

fo: ao1, ao7 und ao13 jeweils von den nachstehenden ao absetzen

tr:

GOTO F3_9



\--------------------------------

F3_9 
=====

tc: 

vn: ainfcp

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wurde Ihr letzter Auslandsaufenthalt auf Ihr Studium angerechnet?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, teilweise

ao3: 3: ja, vollständig

ao4: 4: Ich habe keine Leistungen erbracht.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: ao4 absetzen

tr: GOTO F3_10

hi:

\--------------------------------

F3_10
=====

tc: 

vn: afinelt1; afinpar1; afinbaf1; afinjobv1; afinjobw1, afinstip1; afinkre1; afinand1;
    afinelt2; afinpar2; afinbaf2; afinjobv2; afinjobw2; afinstip2; afinkre2; afinand2;
    afinelt3; afinpar3; afinbaf3; afinjobv3; afinjobw3; afinstip3; afinkre3; afinand3

qt: Mehrfachauswahl

hl:

in:

q1: Wie haben Sie ihren Auslandsaufenthalt finanziert?

q2: Wie haben Sie ihre Auslandsaufenthalte finanziert?

is1: Bitte alles Zutreffende auswählen.

is2: Bitte beginnen Sie mit Ihrem letzten studienbezogenen Auslandsaufenthalt. Bitte alles Zutreffende auswählen.

it:

st:

ao1: (afinelt1): Eltern

ao2: (afinpar1): Partner\*in

ao3: (afinbaf1): BAföG

ao4: (afinjobv1): Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5: (afinjobw1): Verdienst aus Tätigkeiten während des Auslandsaufenthalts

ao6: (afinstip1): Stipendium

ao7: (afinkre1): Bildungskredit

ao8: (afinand1): andere Finanzierungsquelle



ao9: (afinelt2): Eltern

ao10: (afinpar2): Partner\*in

ao11: (afinbaf2): BAföG

ao12: (afinjobv2): Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao13: (afinjobw2): Verdienst aus Tätigkeiten während des Auslandsaufenthalts

ao14: (afinstip2): Stipendium

ao15: (afinkre2): Bildungskredit

ao16: (afinand2): andere Finanzierungsquelle



ao17: (afinelt3): Eltern

ao18: (afinpar3): Partner\*in

ao19: (afinbaf3): BAföG

ao20: (afinjobv3): Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao21: (afinjobw3): Verdienst aus Tätigkeiten während des Auslandsaufenthalts

ao22: (afinstip3): Stipendium

ao23: (afinkre3): Bildungskredit 

ao24: (afinand3): andere Finanzierungsquelle

mv:

ka1 (ao1 TO ao8): Letzter studienbezogener Auslandsaufenthalt

ka2 (ao9 TO ao16): Vorletzter studienbezogener Auslandsaufenthalt

ka3 (ao17 TO ao24): Drittletzter studienbezogener Auslandsaufenthalt

vc:

SHOW q1 AND is1 AND ao1 TO ao8 AND ka1 IF ainfaus==2 OR ainfaus==MISSING

SHOW q2 AND is2 AND ao1 TO ao16 AND ka1 TO ka2 IF ainfaus==3

SHOW q2 AND is2 ao1 TO ao24 AND ka1 TO ka3 IF ainfaus==4

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

tc:

vn: akontdeust / akontgast / akonteinheim / akontintst

qt: Einfachauswahlmatrix mit horizontalen aos

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

qt: Einfachauswahlmatrix mit horizontalen aos

hl:

in:

q1: Wie häufig haben Sie während Ihres Auslandsaufenthalts die folgenden
Sprachen gesprochen?

q2: Wie häufig haben Sie während Ihres letzten Auslandsaufenthalts die folgenden
Sprachen gesprochen?

is:

it1: (asprachland): Landessprache

it2: (asprachdeut): Deutsch

it3: (asprachand): Andere Sprache, und zwar [asprachando] [Eingabefeld]

st:

ao1: 1: nie

ao2: 2: selten

ao3: 3: manchmal

ao4: 4: häufig

ao5: 5: sehr häufig

mv:

ka:

vc:

SHOW q1 IF ainfaus = 2 \| MISSING

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

GOTO F3_14

hi:

\--------------------------------

F3_14 
======

tc: IF ainfaus \> 1 \| kA

vn: azufleistanf / azuforgaufw / azuffinanzaufw

qt: Einfachauswahlmatrix mit horizontalen aos

hl:

in:

q: In Bezug auf Ihren letzten studienbezogenen Auslandsaufenthalt: Wie
beurteilen Sie…

is:

it1: (azufleistanf): … die Leistungsanforderungen?

it2: (azuforgaufw): … den organisatorischen Aufwand?

it3: (azuffinanzaufw): … den finanziellen Aufwand?

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

GOTO F3_15

hi:

\--------------------------------

F3_15
=====

tc:

vn: aeempf

qt: Einfachauswahl mit vertikalen aos

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen:

Würden Sie einen studienbezogenen Auslandsaufenthalt empfehlen?

is:

it:

st:

ao1: 1: nein überhaupt nicht

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

GOTO F3_22

hi:

\-------------------------------- 

F3_16
=====

tc: 
(ainfaus=1 AND auslandint==4) OR
(ainfaus=MISSING AND auslandint==4)

vn: aplanstg / aplantst / aplanpra / aplanspk / aplanstureis / aplanprojekt /
aplansumschoo / aplanson / aplanwnn

qt: Mehrfachnennung

hl:

in:

q: Sie haben angegeben, dass sie einen (weiteren) studienbezogenen
Auslandsaufenthalt planen:
Welche Art von Aufenthalt planen Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aplanstg): Auslandsstudium mit Erwerb eines Abschlusses im Ausland (z. B.
Masterstudium)

ao2: (aplantst): Teilstudium im Ausland (Auslandssemester)

ao3: (aplanpra): Auslandspraktikum

ao4: (aplanspk): Sprachkurs im Ausland

ao5: (aplanstureis): Studienreise

ao6: (aplanprojekt): Projektarbeit

ao7: (aplansumschoo): Summer School

ao8: (aplanson): sonstiger Auslandsaufenthalt

ao9: (aplanwnn): weiß ich noch nicht

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

tc: 
(ainfaus=1 AND auslandint==4) OR
(ainfaus=MISSING AND auslandint==4)

vn: aplanföpro; aplanföproo

qt: Einfachauswahl mit offener Angabe

hl:

q: Auf welche Weise planen Sie Ihren künftigen Auslandsaufenthalt zu
organisieren?

in: Der Aufenthalt findet im Rahmen eines Austauschprogramms statt…

it:

st:

ao1: 1: … ja, ERASMUS+, ERASMUS

ao2: 2: … ja, anderes EU-Programm

ao3: 3: … ja, DAAD-Programm

ao4: 4: … ja, Pädagogischer Austauschdient (PAD)/COMENIUS

ao5: 5: … ja, PROMOS-Stipendium

ao6: 6: … ja, Programm meiner Hochschule in Deutschland

ao7: 7: … ja, Programm meiner Gasthochschule im Ausland

ao8: 8: … ja, anderes Programm, und zwar [aplanföproo] [Eingabefeld; 100 Zeichen]

ao9: 9: … nein, werde Aufenthalt selbst organisieren.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F3_20

hi:

\--------------------------------

F3_20
=====

tc: 
(ainfaus=1 AND auslandint==4) OR
(ainfaus=MISSING AND auslandint==4)

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

ao1: (aplfinelt): Eltern

ao2: (aplfinpar): Partner\*in

ao3: (aplfinbaf): BAföG

ao4: (aplfinjobv): eigener Verdienst aus Tätigkeiten vor dem Auslandsaufenthalt

ao5: (aplfinjobw): eigener Verdienst aus Tätigkeiten während des
Auslandsaufenthalts

ao6: (aplfinstip): Stipendium

ao7: (aplfinand): andere Finanzierungsquelle

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

ao1: 1: nein

ao2: 2: ja, und zwar wenn … (offene Angabe; 200 Zeichen; [aplanbedio])

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

qt: Einfachauswahlmatrix mit horizontalen aos

hl:

in:

q: Wie häufig unterhalten Sie sich mit…

is:

it1: (akontdeust): … Studierenden aus Deutschland?

it2: (akonteust): … Studierenden aus anderen Ländern Europas?

it3: (akontneust): … Studierenden aus Ländern außerhalb Europas?

st:

ao1: 1: sehr selten

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

ao1: 1: Präfix: Dauer: (offene Angabe; 3 Zeichen; [wohnemino]); Suffix: Minuten

ao2: -12: weiß ich nicht

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

ao1: 1: ich gehe zu Fuß

ao2: 2: Fahrrad

ao3: 3: öffentliche Verkehrsmittel

ao4: 4: PKW (allein fahrend)

ao5: 5: PKW (in Fahrgemeinschaft)

ao6: 6: anderes

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

qt: Einfachauswahlmatrix mit horizontalen aos

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

tr: GOTO A_56

hi:
