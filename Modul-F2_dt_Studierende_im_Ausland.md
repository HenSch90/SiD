F2_6
====

tc:

vn: ainf (ainfasia; ainflosia; ainfstosia; ainfbmsia; ainfbjsia; ainfdausia)

qt: Einfachauswahl mit Dropdown und offene Angaben

hl:

in:

q: Sie befinden sich zurzeit im Ausland: Bitte beschreiben Sie diesen Aufenthalt näher.

is:

ao1: (ainfasia): [infield = Art des Aufenthalts; Auslandsstudium mit angestrebtem Abschluss im Ausland - ... - sonstiger Aufenthalt] (Dropdown)

    (ainfasia): 1: Auslandsstudium mit Abschluss

    (ainfasia): 2: Auslandssemester

    (ainfasia): 3: Auslandspraktikum/-praxisphase

    (ainfasia): 4: Sprachkurs

    (ainfasia): 5: Studienreise

    (ainfasia): 6: Projektarbeit

    (ainfasia): 7: Summer School

    (ainfasia): 8: sonstiger Aufenthalt





ao2: (ainflosia): [infield = Land; 100 Zeichen] (offene Angabe)

ao3: (ainfstosia): [infield = Stadt/Hochschule; 100 Zeichen] (offene Angabe)


ao4: (ainfbmsia): [infield = Monat; Januar - Februar - ... - November - Dezember] (Dropdown)

ao5: (ainfbjsia): [infield = Jahr; 2020 - 2019 - ... - 2009 - vor 2009] (Dropdown)


ao6: (ainfdausia): [infield = Dauer des Aufenthalts; 1 Monat - 2 Monate - ... - 12 Monate - mehr als 12 Monate] (Dropdown)

mv:

ka:(ao4 To ao5) Start des Aufenthalts:

vc: SHOW ao2 AND ao3 if hsstandbl=17 AND hsstandlao=MISSING AND hsstandhsao=MISSING

av:

kh:

fv:

hv:

fo: Bitte ainfasia ainflandosia ainfortosia linkdbündig untereinander positionieren. Darunter dann linksbündig die Kategorienüberschrift "Start des Aufenthalts:" und darunter linksbündig ainfbmsia und daneben ainfbjsia. Zuletzt dann ebenfalls darunter linksbündig ainfdausia.

tr:

        <zofar:transitions>
            <zofar:transition target="F2_7" condition="(zofar.asNumber(ainfasia) ge 3 or zofar.asNumber(ainfasia) le 8) or      ((zofar.asNumber(ainfasia)==1 or zofar.asNumber(ainfasia)==2) and (!hsstand_2.value or (zofar.asNumber(hsstandbl) ge 1 and zofar.asNumber(hsstandbl) le 16)))"/>
            <zofar:transition target="F2_7" condition="(zofar.asNumber(ainfasia)==1 or zofar.asNumber(ainfasia)==2) and zofar.isMissing(hsstandlao)"/>
            <zofar:transition target="F2_8"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_8
====

tc:

vn: bde (bdequasia; bdefamssia; bdeoeksia; bdefinsia; bdesprsia; bdearbsia; bdekensia)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Ich habe mich für ein Studium in diesem Land entschieden, …

is: 

it1: (bdequasia): … aufgrund der hohen Lebensqualität.

it2: (bdefamssia): … weil bereits Freund\*innen/Verwandte in diesem Land studiert haben.

it3: (bdeoeksia): … aufgrund der wirtschaftlichen Lage.

it4: (bdefinsia): … weil dies meinen finanziellen Möglichkeiten entspricht.

it5: (bdesprsia): … um meine Sprachkenntnisse zu vertiefen.

it6: (bdearbsia): … um nach Studienabschluss in diesem Land zu arbeiten.

it7: (bdekensia): … um dieses Land kennenzulernen.

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

fo: Frage und Satzbeginn ("Ich habe mich für ein Studium...") bitte linksbündig untereinander positionieren und etwas voneinander absetzen. 

tr:

        <zofar:transitions>
            <zofar:transition target="F2_9"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_9
====

tc:

vn: sabsabssia

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Planen Sie, im Ausland einen Hochschulabschluss zu erwerben?

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

        <zofar:transitions>
            <zofar:transition target="F2_10"/>
        </zofar:transitions>

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

        <zofar:transitions>
            <zofar:transition target="F2_11"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_11
==

tc:

vn: apro (apronosia; aproerassia; aprodaadsia; aprohhssia; aprogahssia; aproanprsia)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Findet Ihr Auslandsaufenthalt im Rahmen eines Austauschprogramms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (apronosia): nein (Exklusivkategorie)

ao2: (aproerassia): ERASMUS+

ao3: (aprodaadsia): DAAD-Programm

ao4: (aprohhssia): Programm meiner Heimathochschule

ao5: (aprogahssia): Programm der Gasthochschule in Deutschland

ao6: (aproanprsia): anderes Programm

mv:

ka: (ao2 TO ao6): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: Bitte über ao2 "Ja, und zwar:" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F2_12"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_13
=====

tc:

vn: akont (akontgastsia; akontbuergsia; akontdeustsia; akontintstsia)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig unterhalten Sie sich mit…

is:

it1: (akontgastsia): … Studierenden des Gastlandes?

it2: (akontbuergsia): … anderen Bürger\*innen des Gastlandes?

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

fo: Bitte etwas Abstand zwischen Frage und Antwortitems. Im Pretest waren diese sehr nah beieinander.

tr:

        <zofar:transitions>
            <zofar:transition target="F2_14"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_14
=====

tc:

vn: asprach (asprachgaslsia; asprachheimlsia; asprachandsia; asprachandsiao)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig sprechen Sie während Ihres Auslandsaufenthalts die folgenden Sprachen?

is:

it1: (asprachgaslsia): Landessprache des Gastlandes

it2: (asprachheimlsia): Deutsch




it3: (asprachandsia): Andere Sprache, und zwar: [(asprachandsiao); offene Angabe, 60 Zeichen]

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

        <zofar:transitions>
            <zofar:transition target="F2_15"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_15
=====

tc:

vn: azuf (azuflernerfsia; azufinsgsia)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie bis zum jetzigen Zeitpunkt mit …

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

        <zofar:transitions>
            <zofar:transition target="F2_16"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_16
=====

tc:

vn: azuf (azuforgaufsia; azuffinaufsia)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und wie beurteilen Sie …

is:

it1: (azuforgaufsia): … den organisatorischen Aufwand Ihres Aufenthaltes?

it2: (azuffinaufsia): … den finanziellen Aufwand Ihres Aufenthaltes?

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

        <zofar:transitions>
            <zofar:transition target="F2_17"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_17
=====

tc:

vn: aeempfsia

qt: Einfachauswahl mit vertikaler ao

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

        <zofar:transitions>
            <zofar:transition target="F2_18"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_19 
======

tc: 

vn: intpsy (intpsydeusia; intpsyzeitasia; intpsydauasia)

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

        <zofar:transitions>
            <zofar:transition target="F2_20"/>
        </zofar:transitions>

hi:

\--------------------------------

F2_20
=====

tc:

vn: intling (intling1sia; intling2sia; intling3sia)

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

        <zofar:transitions>
            <zofar:transition target="A_56"/>
        </zofar:transitions>

hi:
