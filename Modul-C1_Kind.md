
\--------------------------------

C1_1
====

tc: IF dkinja = 2

vn: dkinanz

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wie viele Kinder haben Sie?

is:

it:

st:

ao1: 1: eins

ao2: 2: zwei

ao3: 3: drei

ao4: 4: vier oder mehr

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO C1_2

hi:

\--------------------------------

C1_2
====

tc: IF dkinja = 2

vn: dkinage (dkinagej / dkinage1 / dkinage2 / dkinage3 / dkinage4 / dkinage5)

qt: offene Angaben mit vertikaler Eingabespalte/-feldern

hl:

in:

q1: Wie alt ist Ihr jüngstes Kind?

q2: Wie alt ist Ihr Kind?

q3: Wie alt sind Ihre Kinder?

is: Mit “1. Kind” meinen wir Ihr ältestes Kind.

it1: (dkinagej) [infield = Alter jüngstes Kind]

it2: (dkinage1): [infield = Alter Ihres Kindes]

it3: (dkinage2): [infield = Alter 1. Kind]

it4: (dkinage3): [infield = Alter 2. Kind]

it5: (dkinage4): [infield = Alter 3. Kind]

it6: (dkinage5): [infield = Alter 4. Kind]

st:

ao1: (dkinagej): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao2: (dkinage1): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao3: (dkinage2): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao4: (dkinage3): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao5: (dkinage4): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao6: (dkinage5): 4-stellig: 0 TO 99, number, Suffix: Jahre

mv:

ka:

vc1: SHOW dkinagej IF dkinanz = k. A.

vc2: SHOW dkinage1 IF dkinanz = 1

vc3: SHOW dkinage2 IF dkinanz >= 2

vc4: SHOW dkinage3 IF dkinanz >= 2

vc5: SHOW dkinage4 IF dkinanz >= 3

vc6: SHOW dkinage5 IF dkinanz >= 4

vc7: SHOW is IF dkinanz >= 2

vc8: SHOW q1 IF dkinanz = k. A.

vc9: SHOW q2 IF dkinanz = 1

vc10: SHOW q3 IF dkinanz >= 2

av: 

kh: Bitte geben Sie das Lebensalter Ihres Kindes an (0 bis 99).

fv:

hv:

fo:

tr:

GOTO C1_4

hi: Dezimalstellen zulassen.

\--------------------------------

C1_3
====

tc: IF dkinja=2

vn: dkinro (dkinrono / dkinrofr / dkinrokom / dkinroges / dkinroelt / dkinrover)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Kannten Sie jemanden, der bereits vor Ihnen mit Kind studiert hat?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dkinrono): nein, niemanden [EK] 

ao2: (dkinrofr): Freund\*innen, Bekannte

ao3: (dkinrokom): Kommiliton\*innen

ao4: (dkinroges): Geschwister

ao5: (dkinroelt): Eltern

ao6: (dkinrover): andere Verwandte

mv:

ka: (ao2 TO ao6): ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: "ja, und zwar:" zwischen ao1 und ao2 setzen.

tr:

GOTO C1_6

hi:

\--------------------------------

C1_4
====

tc: IF dkinja = 2

vn: dkinanzhh

qt: offene Angabe

hl:

in:

q: Wie viele Kinder leben in Ihrem Haushalt?

is:

it:

st:

ao: (dkinanzhh):  [infield = "Anzahl Kinder"; number, 1-stellig: 0 TO 9]

mv:

ka:

vc:

av:

kh: Bitte geben Sie die Anzahl an Kindern in Ihrem Haushalt an (0 bis 9).

fv:

hv:

fo:

tr: GOTO C1_5

hi:

\--------------------------------

C1_5
====

tc: IF dkinja = 2

vn: dkinalo

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Sind Sie alleinerziehend?

is: Darunter fallen Personen, die allein mit minderjährigen Kindern zusammenleben und 
hauptverantwortlich für deren Erziehung sorgen.

it:

st:

ao1: 1: ja

ao2: 2: nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_3

hi:

\--------------------------------

C1_7
====

tc: IF dkinja = 2

vn: dkinbe (dkinbehs / dkinbekit / dkinbekig / dkinbeho / dkinbehts / dkinbehtsn / dkinbegts / dkinbek)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q1: Nutzen Sie die folgenden Einrichtungen/Angebote zur Betreuung Ihres Kindes/Ihrer Kinder?

q2: Nutzen Sie die folgenden Einrichtungen/Angebote zur Betreuung Ihres Kindes?

q3: Nutzen Sie die folgenden Einrichtungen/Angebote zur Betreuung Ihrer Kinder?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dkinbehs): Betreuungsangebote an der Hochschule

ao2: (dkinbekit): Krippe/Kita/Tagesmutter (0-3 Jahre)

ao3: (dkinbekig): Kindergarten (3-6 Jahre)

ao4: (dkinbeho): Hort 

ao5: (dkinbehts): Halbtagsschule

ao6: (dkinbehtsn): Halbtagsschule mit Nachmittagsangeboten

ao7: (dkinbegts): Ganztagsschule

ao8: (dkinbek): keine der genannten Einrichtungen [EK]

mv:

ka:

vc1: SHOW q1 IF dkinanz = k.A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \>1

av:

kh:

fv:

hv:

fo: ao8 bitte etwas absetzen.

tr: GOTO C1_9

hi:

\--------------------------------

C1_6
====

tc: IF dkinja = 2

vn: dkinbe (dkinbesel / dkinbepar / dkinbeelt / dkinbegelt / dkinbefr / dkinbesit / dkinbealo)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie häufig betreuen die folgenden Personen Ihr(e) Kind(er)?

q2: Wie häufig betreuen die folgenden Personen Ihr Kind?

q3: Wie häufig betreuen die folgenden Personen Ihre Kinder?

is:

it1: (dkinbesel): ich selbst

it2: (dkinbepar): Partner\*in

it3: (dkinbeelt): anderer Elternteil (falls nicht Partner\*in)

it4: (dkinbegelt): Großeltern oder andere Verwandte

it5: (dkinbefr): Freund\*innen, Bekannte

it6: (dkinbesit): bezahlte Babysitter\*innen

it7: (dkinbealo): Das Kind bleibt/Die Kinder bleiben alleine.

it8: (dkinbealo): Das Kind bleibt alleine.

it9: (dkinbealo): Die Kinder bleiben alleine.

st:

ao1: 1: nie

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: sehr häufig

mv:

ka:

vc1: SHOW q1 IF dkinanz = k.A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \>1

vc4: SHOW it7 IF dkinanz = k.A.

vc5: SHOW it8 IF dkinanz = 1

vc6: SHOW it9 IF dkinanz \>1

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_7

hi:

\--------------------------------

C1_9
====

tc: IF dkinja = 2

vn: dkinsu (dkinsuwist / dkinsuekr / dkinsuspz / dkinsubers / dkinsuberf / dkinsubar / dkinsuspr / dkinsuwoh / dkinsukber)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Gibt es an Ihrem Hochschulstandort folgende Unterstützungsmöglichkeiten bzw. Angebote für Studierende mit Kind?

is:

it1: (dkinsuwist): Wickel-/Stillräume

it2: (dkinsuekr): Eltern-Kind-Räume

it3: (dkinsuspm): Spielmöglichkeiten

it4: (dkinsubers): Studienberatung, Familienservice/-büro

it5: (dkinsuberf) Sozial-/Finanzberatung

it6: (dkinsubar): barrierefreie Zugänge für Kinderwagen

it7: (dkinsuspr): Gesprächskreise für Eltern

it8: (dkinsuwoh): Wohnangebote für Studierende mit Kind

it9: (dkinsukber): Angebote zur flexiblen Kurzzeitbetreuung von Kindern


st:

ao1: 0: nein 

ao2: 1: ja 

mv: -12: weiß ich nicht 

ka:

vc:

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" etwas absetzen.

tr: GOTO C1_10

hi:

\--------------------------------

C1_10
=====

tc: IF dkinja = 2

vn: dkinver (dkinverlver / dkinverreg / dkinveratm)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium mit Kind(ern) zu?

q2: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium mit Kind zu?

q3: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium mit Kindern zu?

is:


it1: (dkinverlver): Die Lehrenden meines Studiengangs haben Verständnis für die besondere Situation von Studierenden mit Kind(ern).

it2: (dkinverlver): Die Lehrenden meines Studiengangs haben Verständnis für die besondere Situation von Studierenden mit Kind.

it3: (dkinverlver): Die Lehrenden meines Studiengangs haben Verständnis für die besondere Situation von Studierenden mit Kindern.

it4: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kind(ern).

it5: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kind.

it6: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kindern.

it7: (dkinveratm): In meinem Studiengang herrscht eine kinderfreundliche Atmosphäre.


st:

ao1: 1: trifft gar nicht zu

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc1: SHOW q1 IF dkinanz = k.A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \>1

vc4: SHOW it1, it4 IF dkinanz = k.A.

vc5: SHOW it2, it5 IF dkinanz = 1

vc6: SHOW it3, it6 IF dkinanz \>1

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_12

hi: 

\--------------------------------

C1_12
=====

tc: IF dkinja = 2

vn: dkin (dkinwistu / dkinentstu)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr stimmen Sie den folgenden Aussagen zu?

is:

it1: (dkinwistu): Mir ist es wichtig, dass mein Kind später einmal studiert/meine Kinder später einmal studieren.

it2: (dkinwistu): Mir ist es wichtig, dass mein Kind später einmal studiert.

it3: (dkinwistu): Mir ist es wichtig, dass meine Kinder später einmal studieren.

it4: (dkinentstu): Wenn mein Kind nicht studiert/meine Kinder nicht studieren, wäre ich enttäuscht.

it5: (dkinentstu): Wenn mein Kind nicht studiert, wäre ich enttäuscht.

it6: (dkinentstu): Wenn meine Kinder nicht studieren, wäre ich enttäuscht.


st:

ao1: 1: gar nicht

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: voll und ganz

mv:

ka:

vc1: SHOW it1, it4 IF dkinanz = k. A.

vc2: SHOW it2, it5 IF dkinanz = 1

vc3: SHOW it3, it6 IF dkinanz \> 1

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_14

hi:

\--------------------------------

C1_14
=====

tc: IF dkinja = 2

vn: dkinsturev

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Was würden Sie künftigen Studienanfänger\*innen empfehlen

is:

it:

st:

ao1: 1: erst studieren, wenn die Kinder älter sind

ao2: 2: während des Studiums Kinder bekommen

ao3: 3: erst das Studium beenden und dann Kinder bekommen

ao4: 4: gar keine Kinder bekommen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_13

hi:
