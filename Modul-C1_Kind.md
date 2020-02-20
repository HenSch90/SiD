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

qt: offene Einzelfragen mit vertikaler Eingabespalte/-feldern

hl:

in:

q1: Wie alt ist Ihr jüngstes Kind?

q2: Wie alt ist Ihr Kind?

q3: Wie alt sind Ihre Kinder?

is: Mit der Bezeichnung “1. Kind” meinen wir Ihr ältestes Kind.

it1: (dkinagej) 

it2: (dkinage1): [infield = Alter Ihres Kindes]

it3: (dkinage2): [infield = Alter Ihres 1. Kindes]

it4: (dkinage3): [infield = Alter Ihres 2. Kindes]

it5: (dkinage4): [infield = Alter Ihres 3. Kindes]

it6: (dkinage5): [infield = Alter Ihres 4. Kindes]

st:

ao1: (dkinagej): 2-stellig, 0-99, [number] Suffix: Jahre

ao2: (dkinage1): 4-stellig, 0-99, [number] Suffix: Jahre

ao3: (dkinage2): 4-stellig, 0-99, [number] Suffix: Jahre

ao4: (dkinage3): 4-stellig, 0-99, [number] Suffix: Jahre

ao5: (dkinage4): 4-stellig, 0-99, [number] Suffix: Jahre

ao6: (dkinage5): 4-stellig, 0-99, [number] Suffix: Jahre

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

av: Bitte geben Sie das Lebensalter Ihres Kindes an (0 bis 99).

kh:

fv:

hv:

fo:

tr:

GOTO C1_4

hi: Eingabefelder auf XXXX-Format setzen; Wertebereich = 0 bis 99; Dezimalstellen zulassen.

\--------------------------------

C1_3
====

tc: IF dkinja=2

vn: dkinro (dkinrono / dkinroelt / dkinroges / dkinrover / dkinrokom / dkinrofr / dkinroan / dkinroano)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Kannten Sie jemanden, der bereits vor Ihnen mit Kind(ern) studiert hat?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dkinrono): nein, niemanden [EK] 

ao2: (dkinroelt): Eltern

ao3: (dkinroges): Geschwister

ao4: (dkinrover): andere Verwandte

ao5: (dkinrokom): Kommiliton\*innen

ao6: (dkinrofr): Freunde

ao7: (dkinroan): Andere Person(en), und zwar: [dkinroano, 30pt]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO C1_11

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

av: Bitte geben Sie die Anzahl an Kindern in Ihrem Haushalt an (0 bis 9).

kh:

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

is:

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

C1_6
====

tc: IF dkinja = 2

vn: dkinbe (dkinbesel / dkinbepar / dkinbeelt / dkinbegelt / dkinbever /
dkinbefr / dkinbesit / dkinbetag / dkinbealo / dkinbeson / dkinbesono)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wenn Sie an eine typische Woche denken: Welche der folgenden Personen betreuen wie häufig Ihr(e) Kind(er)?

q2: Wenn Sie an eine typische Woche denken: Welche der folgenden Personen betreuen wie häufig Ihr Kind?

q3: Wenn Sie an eine typische Woche denken: Welche der folgenden Personen betreuen wie häufig Ihre Kinder?

is:

it1: (dkinbesel): ich selbst

it2: (dkinbepar): Partner\*in

it3: (dkinbeelt): anderer Elternteil (falls nicht Partner\*in)

it4: (dkinbegelt): Großeltern

it5: (dkinbever): andere Verwandte

it6: (dkinbefr): Freunde, Bekannte

it7: (dkinbesit): bezahlter Babysitter

it8: (dkinbetag): Tagesmutter

it9: (dkinbealo): Das Kind bleibt/Die Kinder bleiben alleine.

it10: (dkinbeson): Andere Person, und zwar: [dkinbesono; 30pt]

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

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_7

hi:

\--------------------------------

C1_7
====

tc: IF dkinja = 2

vn: dkinbe (dkinbekihs / dkinbehsa / dkinbeki / dkinbehts / dkinbegts /
dkinbesoe / dkinbesoeo)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wenn Sie an eine typische Woche denken: Inwieweit nutzen Sie die folgenden
Einrichtungen zur Betreuung Ihres Kindes/Ihrer Kinder?

q2: Wenn Sie an eine typische Woche denken: Inwieweit nutzen Sie die folgenden
Einrichtungen zur Betreuung Ihres Kindes?

q3: Wenn Sie an eine typische Woche denken: Inwieweit nutzen Sie die folgenden
Einrichtungen zur Betreuung Ihrer Kinder?

is:

it1: (dkinbekihs): Kita an der Hochschule

it2: (dkinbehsa): weitere hochschulspezifische Betreuungsangebote

it3: (dkinbeki): andere Kita (Kindergarten, Hort, Krippe)

it4: (dkinbehts): Halbtagsschule

it5: (dkinbegts): Ganztagsschule

it6: (dkinbesoe): Sonstige Einrichtung, und zwar: [dkinbesoeo; 30pt]

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

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_8

hi:

\--------------------------------

C1_8
====

tc: IF dkinja = 2

vn: dkinbezuf

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie zufrieden sind Sie insgesamt mit der Betreuungssituation Ihres Kindes/Ihrer Kinder?

q2: Wie zufrieden sind Sie insgesamt mit der Betreuungssituation Ihres Kindes?

q3: Wie zufrieden sind Sie insgesamt mit der Betreuungssituation Ihrer Kinder?

is:

it:

st:

ao1: 1: gar nicht zufrieden

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: sehr zufrieden

mv:

ka:

vc1: SHOW q1 IF dkinanz = k.A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \>1

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_9

hi:

\--------------------------------

C1_9
====

tc: IF dkinja = 2

vn: dkinsu (dkinsuwic / dkinsustil / dkinsuekr / dkinsuspz / dkinsuspf /
dkinsuinf / dkinsuber / dkinsubar / dkinsuspr / dkinsuwoh / dkinsukber /
dkinsubur / dkinsuso / dkinsusoo)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Gibt es an Ihrer Hochschule folgende Unterstützungsmöglichkeiten bzw. Angebote für Studierende mit Kind(ern)?

is:

it1: (dkinsuwic): Wickelräume

it2: (dkinsustil): Stillräume

it3: (dkinsuekr): Eltern-Kind-Räume

it4: (dkinsuspz): Spielzimmer

it5: (dkinsuspf): Spielflächen im Freien

it6: (dkinsuinf): Informationsangebote

it7: (dkinsuber): Studienberatung für Studierende mit Kind

it8: (dkinsubar): barrierefreie Zugänge für Kinderwagen

it9: (dkinsuspr): Gesprächskreise für Eltern

it10: (dkinsuwoh): Wohnangebote für Studierende mit Kind

it11: (dkinsukber): Angebote zur Kurzzeitbetreuung von Kindern

it12: (dkinsubur): Familienservice/-büro

it13: (dkinsuso): Sonstiges, und zwar: [dkinsusoo; Eingabefeld]

st:

ao1: 0: nein 

ao2: 1: ja 

ao3: -12: weiß ich nicht 

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_10

hi:

\--------------------------------

C1_10
=====

tc: IF dkinja = 2

vn: dkinver (dkinverdau / dkinverlver / dkinverlei / dkinverwil / dkinveratm / dkinverreg)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium mit Kind(ern) zu?

is:

it1: (dkinverdau): Durch den Zeitbedarf für mein(e) Kind(er), wird mein Studium länger dauern.

it2: (dkinverlver): Die Lehrenden meines Studiengangs haben Verständnis für die besondere Situation von Studierenden mit Kind.

it3: (dkinverlei): Es fällt mir leicht, Studium und Kind(er) zu vereinbaren.

it4: (dkinverwil): Wegen meines Kindes/meiner Kinder, kann ich nicht so studieren, wie ich will.

it5: (dkinveratm): In meinem Studiengang herrscht eine kinderfreundliche Atmosphäre.

it6: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kind(ern).

st:

ao1: 1: trifft gar nicht zu

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: trifft voll und ganz zu

mv:

ka:

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_12

hi: Items bitte zufällig rotieren.

\--------------------------------

C1_11
=====

tc: IF dkinja = 2

vn: dkin (dkinsw / dkinopfb / dkinauto / dkinfreu / dkinufur / dkinfoe)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen folgende Aussagen auf Sie zu?

is:

it1: (dkinsw): Ich kann den Bedürfnissen meines Kindes/meiner Kinder sehr gut gerecht werden.

it2: (dkinopfb): Ich würde alles aushalten für das Wohl meines Kindes/meiner Kinder.

it3: (dkinauto): Ich habe das Gefühl, dass die Betreuung und Erziehung meines
Kindes/meiner Kinder mich völlig in Beschlag nimmt und mein ganzes Leben
bestimmt.

it4: (dkinfreu): Ich freue mich immer darauf, mit meinem Kind/meinen Kindern
zusammen zu sein.

it5: (dkinufur): Ich bin ständig in Sorge, dass meinem Kind/meinen Kindern etwas
zustoßen könnte.

it6: (dkinfoe): Ich denke, wenn mein Kind/eins meiner Kinder sich falsch
verhält, macht es das mit Absicht.

st:

ao1: 1: trifft gar nicht zu

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: trifft voll und ganz zu

mv:

ka:

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_6

hi: Items bitte zufällig rotieren.

\--------------------------------

C1_12
=====

tc: IF dkinja = 2

vn: dkin (dkinmsabi / dkinzuabi / dkinmsstu / dkinzustu / dkinmsabi1 / dkinzuabi1 / dkinmsstu1 / dkinzustu1 / dkinmsabi2 / dkinzuabi2 / dkinmsstu2 / dkinzustu2)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr stimmen Sie den folgenden Aussagen zu?

is:

it1: (dkinmsabi): Für mich ist das ++Abitur++ für mein(e) Kind(er) der absolute Minimalstandard.
it2: (dkinzuabi): Mit weniger als einem ++Abitur++ für mein(e) Kind(er) würde ich mich nicht zufrieden geben.
it3: (dkinmsstu): Für mich ist ein ++Studium++ für mein(e) Kind(er) der absolute Minimalstandard.
it4: (dkinzustu): Mit weniger als einem ++Studium++ für mein(e) Kind(er) würde ich mich nicht zufrieden geben.

it5: (dkinmsabi1): Für mich ist das ++Abitur++ für mein Kind der absolute Minimalstandard.
it6: (dkinzuabi1): Mit weniger als einem ++Abitur++ für mein Kind würde ich mich nicht zufrieden geben.
it7: (dkinmsstu1): Für mich ist ein ++Studium++ für mein Kind der absolute Minimalstandard.
it8: (dkinzustu1): Mit weniger als einem ++Studium++ für mein Kind würde ich mich nicht zufrieden geben.

it9: (dkinmsabi2): Für mich ist das ++Abitur++ für meine Kinder der absolute Minimalstandard.
it10: (dkinzuabi2): Mit weniger als einem ++Abitur++ für meine Kinder würde ich mich nicht zufrieden geben.
it11: (dkinmsstu2): Für mich ist ein ++Studium++ für meine Kinder der absolute Minimalstandard.
it12: (dkinzustu2): Mit weniger als einem ++Studium++ für meine Kinder würde ich mich nicht zufrieden geben.

st:

ao1: 1: gar nicht

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: voll und ganz

mv:

ka:

vc1: SHOW it1, it2, it3, it4 IF dkinanz = k. A.

vc2: SHOW it5, it6, it7, it8 IF dkinanz = 1

vc3: SHOW it9, it10, it11, it12 IF dkinanz \> 1

av:

kh:

fv:

hv:

fo:

tr: GOTO C1_13

hi:

\--------------------------------

C1_13
=====

tc: IF dkinja = 2

vn: dkinstuja

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q1: Würden Sie wieder mit Kind(ern) studieren?

q2: Würden Sie wieder mit Kind studieren?

q3: Würden Sie wieder mit Kindern studieren?

is:

it:

st:

ao1: 1: nein, auf keinen Fall

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: ja, auf jeden Fall

mv:

ka:

vc1: SHOW q1 IF dkinanz = k. A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \> 1

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

q: Wenn Sie die Möglichkeit hätten, welche Alternative würden Sie favorisieren?

is:

it:

st:

ao1: 1: während des Studiums das Kind bekommen

ao2: 2: erst studieren, wenn das Kind selbstständiger ist

ao3: 3: erst das Studium beenden und dann ein Kind bekommen

ao4: 4: gar kein(e) Kind(er) bekommen

ao5: 5: gar kein Studium aufnehmen

ao6: 6: keine der genannten Optionen

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
