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

        <zofar:transitions>
            <zofar:transition target="C1_2"/>
        </zofar:transitions>
        
hi:

\--------------------------------

C1_2
====

tc: IF dkinja = 2

vn: dkinage (dkinagej / dkinage1 / dkinage2 / dkinage3 / dkinage4 / dkinage5)

qt: Mehrere Dropdownmenüs vertikal

hl:

in:

q1: Wie alt ist Ihr jüngstes Kind?

q2: Wie alt ist Ihr Kind?

q3: Wie alt sind Ihre Kinder?

is: Mit “1. Kind” meinen wir Ihr ältestes Kind.

it1: (dkinagej) Alter jüngstes Kind:

it2: (dkinage1): Alter Ihres Kindes:

it3: (dkinage2): Alter 1. Kind:

it4: (dkinage3): Alter 2. Kind:

it5: (dkinage4): Alter 3. Kind:

it6: (dkinage5): Alter 4. Kind:

st:

ao0: 0: Alter
  
ao1: 1: < 1 Jahr
  
ao2: 2: 1 Jahr
  
ao3: 3: 2 Jahre
  
ao4: 4: 3 Jahre
  
ao5: 5: 4 Jahre
  
ao6: 6: 5 Jahre
  
ao7: 7: 6 Jahre
  
ao8: 8: 7 Jahre
  
ao9: 9: 8 Jahre

ao10: 10: 9 Jahre

ao11: 11: 10 Jahre

ao12: 12: 11 Jahre

ao13: 13: 12 Jahre

ao14: 14: 13 Jahre

ao15: 15: 14 Jahre

ao16: 16: 15 Jahre

ao17: 17: 16 Jahre

ao18: 18: 17 Jahre

ao19: 19: 18 Jahre

ao20: 20: 19 Jahre

ao21: 21: 20 Jahre

ao22: 22: 21 Jahre

ao23: 23: 22 Jahre

ao24: 24: 23 Jahre

ao25: 25: 24 Jahre

ao26: 26: 25 Jahre

ao27: 27: 26 Jahre

ao28: 28: 27 Jahre

ao29: 29: 28 Jahre

ao30: 30: 29 Jahre

ao31: 31: 30 Jahre

ao32: 32: >30 Jahre

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

kh: 

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="C1_4"/>
        </zofar:transitions>

hi: Kategorien des Dropdown-Menüs sind für jede Variable gleich (siehe ao1-ao32). ao1 (Alter) soll vorausgewählt sein

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

tr: 

        <zofar:transitions>
            <zofar:transition target="C1_5"/>
        </zofar:transitions>

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

tr: 

        <zofar:transitions>
                <zofar:transition target="C1_7" condition="
                        (zofar.asNumber(dkinagej) lt 23 and zofar.asNumber(dkinagej) ge 1) or 
                        (zofar.asNumber(dkinage1) lt 23 and zofar.asNumber(dkinage1) ge 1) or 
                        (zofar.asNumber(dkinage2) lt 23 and zofar.asNumber(dkinage2) ge 1) or 
                        (zofar.asNumber(dkinage3) lt 23 and zofar.asNumber(dkinage3) ge 1) or 
                        (zofar.asNumber(dkinage4) lt 23 and zofar.asNumber(dkinage4) ge 1) or 
                        (zofar.asNumber(dkinage5) lt 23 and zofar.asNumber(dkinage5) ge 1)"/>
                <zofar:transition target="C1_7" condition="
                        (zofar.isMissing(dkinagej) and zofar.isMissing(dkinanz)) or 
                        (zofar.isMissing (dkinage1) and zofar.asNumber(dkinanz)==1) or 
                        ((zofar. isMissing(dkinage2) or zofar. isMissing(dkinage3)) and zofar.asNumber(dkinanz)==2) or
                        ((zofar. isMissing(dkinage2) or zofar. isMissing(dkinage3) or zofar. isMissing(dkinage4)) and zofar.asNumber(dkinanz)==3) or
                        ((zofar. isMissing(dkinage2) or zofar. isMissing(dkinage3) or zofar. isMissing(dkinage4) or zofar. isMissing(dkinage5)) and zofar.asNumber(dkinanz)==4)"/>
            <zofar:transition target="C1_12"/>
        </zofar:transitions>


hi:

\--------------------------------

C1_7
====

tc: IF dkinja = 2

vn: dkinbe (dkinbehs / dkinbekit / dkinbekig / dkinbeho / dkinbehts / dkinbehtsn / dkinbegts / dkinbek)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q1: Nutzen Sie üblicherweise die folgenden Einrichtungen/Angebote zur Betreuung Ihres Kindes/Ihrer Kinder?

q2: Nutzen Sie üblicherweise die folgenden Einrichtungen/Angebote zur Betreuung Ihres Kindes?

q3: Nutzen Sie üblicherweise die folgenden Einrichtungen/Angebote zur Betreuung Ihrer Kinder?

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

tr:

        <zofar:transitions>
            <zofar:transition target="C1_6"/>
        </zofar:transitions>

hi:

\--------------------------------

C1_6
====

tc: IF dkinja = 2

vn: dkinbe (dkinbesel / dkinbepar / dkinbeelt / dkinbegelt / dkinbefr / dkinbesit / dkinbealo)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie häufig betreuen üblicherweise die folgenden Personen Ihr(e) Kind(er)?

q2: Wie häufig betreuen üblicherweise die folgenden Personen Ihr Kind?

q3: Wie häufig betreuen üblicherweise die folgenden Personen Ihre Kinder?

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

tr:

        <zofar:transitions>
            <zofar:transition target="C1_10"/>
        </zofar:transitions>

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

it1: (dkinverlver): Die Lehrenden meines Studiengangs haben Verständnis für die besondere Situation von Studierenden mit Kindern.

it2: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kind(ern).

it3: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kind.

it4: (dkinverreg): Die geltenden Studienregelungen erleichtern das Studieren mit Kindern.

it5: (dkinveratm): In meinem Studiengang herrscht eine kinderfreundliche Atmosphäre.


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

vc4: SHOW it2 IF dkinanz = k.A.

vc5: SHOW it3 IF dkinanz = 1

vc6: SHOW it4 IF dkinanz \>1

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="C1_12"/>
        </zofar:transitions>

hi: 

\--------------------------------

C1_12
=====

tc: IF dkinja = 2

vn: dkinwistu

qt: Einfachauswahlmatrix/5er-Skala mit vertikalen ao

hl:

in:

q1: Wie wichtig ist es Ihnen, dass Ihr Kind später einmal studiert/Ihre Kinder später einmal studieren?

q2: Wie wichtig ist es Ihnen, dass Ihr Kind später einmal studiert?

q3: Wie wichtig ist es Ihnen, dass Ihre Kinder später einmal studieren?

is:

it1: 

st:

ao1: 1: gar nicht wichtig

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: sehr wichtig

mv: -12: weiß ich nicht

ka:

vc1: SHOW q1 IF dkinanz = k. A.

vc2: SHOW q2 IF dkinanz = 1

vc3: SHOW q3 IF dkinanz \> 1

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" etwas absetzen.

tr: 

        <zofar:transitions>
            <zofar:transition target="C1_14"/>
        </zofar:transitions>

hi:

\--------------------------------

C1_14
=====

tc: IF dkinja = 2

vn: dkinsturev

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Was würden Sie angehenden Studierenden empfehlen?

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_13"/>
        </zofar:transitions>

hi:
