F1_1
====

tc:

vn: aeinnorm (aeinnorm1; aeinnorm2)

qt:  Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwiefern treffen die folgenden Aussagen Ihrer Meinung nach zu?

is:

it1: (aeinnorm1): Ein Auslandsaufenthalt darf während des Studiums auf keinen Fall fehlen.

it2: (aeinnorm2): Auslandserfahrungen werden auf dem Arbeitsmarkt oftmals erwartet.

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

tr:

        <zofar:transitions>
            <zofar:transition target="F1_2b" condition="width.value lt 768"/>
            <zofar:transition target="F1_2"/>
        </zofar:transitions>

hi:

\-------------------------------

F1_2
====

tc:

vn: aeins (aeinsarbm; aeinssprachk; aeinsfach; aeinspersoen; aeinskont; aeinskultur; aeinsspas; aeinsfinanz; aeinsorga; aeinsfreun; aeinsanerk; aeinszeit; aeinsfehlspra; aeinsangstl)

qt: Einfachauswahlmatrix/5er-Skala mit Zwischenüberschriften und horizontalen ao

hl:

in:

q: Was spricht Ihrer Meinung nach …

is:

it1: (aeinsarbm): Verbesserung der Arbeitsmarktchancen

it2: (aeinssprachk): Verbesserung der Sprachkenntnisse

it3: (aeinsfach): Verbesserung der Fachkenntnisse

it4: (aeinspersoen): Persönlichkeitsentwicklung

it5: (aeinskont): Kontakte knüpfen

it6: (aeinskultur): andere Kulturen kennenlernen

it7: (aeinsspas): Spaß haben

it8: (aeinsfinanz): finanzielle Belastung

it9: (aeinsorga): Organisationsaufwand

it10: (aeinsfreun): Trennung von Freund\*innen und Familie

it11: (aeinsanerk): Anerkennungsschwierigkeiten

it12: (aeinszeit): Zeitverlust

it13: (aeinsfehlspra): fehlende Sprachkenntnisse

it14: (aeinsangstl): Angst vor fremder Studien- und Lebenssituation

st:

ao1: 1: überhaupt nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr stark

mv:

ka1: (it1 TO it7) !!… **für** einen Auslandsaufenthalt?!!

ka2: (it8 TO it it14) !!… **gegen** einen Auslandsaufenthalt?!!

vc:

av:

kh:

fv:

hv:




fo1: Bitte über it1 "... **für** einen Auslandsaufenthalt" linksbündig positionieren.

fo2: Bitte über it8 "... **gegen** einen Auslandsaufenthalt" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_3"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_3
====

tc:

vn: ainfpfakt

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist in Ihrem Studiengang ein Auslandsaufenthalt verpflichtend vorgeschrieben?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja

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
            <zofar:transition target="F1_4"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_4
====

tc:

vn: avor (avorniem; avorelt; avorgeschw; avorandver; avorfreund; avorkomm)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Kennen Sie jemanden, der bereits vor Ihnen im Rahmen seines Studiums im Ausland war?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (avorniem): nein, niemanden (Exklusivkategorie)

ao2: (avorelt): Eltern

ao3: (avorgeschw): Geschwister

ao4: (avorandver): andere Verwandte

ao5: (avorfreund): Freund\*innen

ao6: (avorkomm): Kommiliton\*innen

mv:

ka: (it2 TO it6) Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo1: ao1 bitte etwas absetzen.

fo2: Bitte über it2 "Ja, und zwar:" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_5"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_5
====

tc:

vn: aauszeitleb (aauszeitlebnein; aauszeitlebfrkin; aauszeitlebwschul; aauszeitlebnschul)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie im Laufe Ihres Lebens eine längere Zeit (durchgängig mehr als 3 Monate) im Ausland verbracht?




is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aauszeitlebnein): nein (Exklusivkategorie)

ao2: (aauszeitlebfrkin): ja, in meiner frühen Kindheit

ao3: (aauszeitlebwschul): ja, während meiner Schulzeit

ao4: (aauszeitlebnschul): ja, zwischen Schule und Studium

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
            <zofar:transition target="F1_6" condition="(zofar.asNumber(vsbdeba)==2)"/>
            <zofar:transition target="F2_6" condition="(zofar.asNumber(vsbdeba)==1              and zofar.asNumber(imausl)==2)"/>
            <zofar:transition target="F2_6" condition="(zofar.isMissing(vsbdeba)              and zofar.asNumber(imausl)==2)"/>
            <zofar:transition target="F3_6" condition="(zofar.asNumber(vsbdeba)==1              and zofar.asNumber(imausl)==1)"/>
            <zofar:transition target="F3_6" condition="(zofar.asNumber(vsbdeba)==1              and zofar.isMissing(imausl))"/>
            <zofar:transition target="F3_6" condition="(zofar.isMissing(vsbdeba)              and zofar.isMissing(imausl))"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_6
====

tc:

vn: vsbkolba

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie in Deutschland ein Studienkolleg besucht?

it:

st:

ao1: 1: nein

ao2: 2: ja

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
            <zofar:transition target="F1_7"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_7
====

tc:

vn: vsbanrschba

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Hatten Sie Schwierigkeiten bei der Anerkennung Ihrer Vorbildung in Deutschland?

it:

st:

ao1: 1: nein, keine Schwierigkeiten

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: ja, sehr viele Schwierigkeiten

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
            <zofar:transition target="F1_8"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_8
====

tc:

vn: intdeutsch (intdeutsch1ba; intdeutsch2ba; intdeutsch3ba; intdeutsch4ba; intdeutsch5ba; intdeutsch6ba)

qt: Mehrfachauswahl mit vertikalen ao und Exklusivkat.

hl:

in:

q: Wo haben Sie die nötigen Sprachkenntnisse für ein Studium in Deutschland erworben?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intdeutsch1ba): Elternhaus

ao2: (intdeutsch2ba): Schule/Studium außerhalb Deutschlands

ao3: (intdeutsch3ba): Sprachkurs außerhalb Deutschlands

ao4: (intdeutsch4ba): Sprachkurs in Deutschland (vor dem Studium)

ao5: (intdeutsch5ba): studienbegleitend an einer deutschen Hochschule

ao6: (intdeutsch6ba): bisher noch gar nicht [Exklusivkategorie]

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
            <zofar:transition target="F1_9"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_9
====

tc:

vn: bde (bdequaba; bdefamsba; bdeoekba; bdefinba; bdesprba; bdearbba; bdekenba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Warum haben Sie sich für Deutschland als Studienland entschieden?

q2: !!Ich habe mich für ein Studium in Deutschland entschieden, ...!!

is:

it1: (bdefamsba): ... weil bereits Freund\*innen/Verwandte in Deutschland studiert haben.

it2: (bdefinba): ... weil dies meinen finanziellen Möglichkeiten entspricht.

it3: (bdesprba): ... um meine Sprachkenntnisse zu vertiefen.

it4: (bdekenba): ... um Deutschland kennenzulernen.

it5: (bdeoekba): ... aufgrund der wirtschaftlichen Lage in Deutschland.

it6: (bdequaba): ... aufgrund der hohen Lebensqualität.

it7: (bdearbba): ... um nach Studienabschluss in Deutschland zu arbeiten.

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

fo: q2 bitte unterhalb und mit etwas Abstand von q1 positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_10"/>
        </zofar:transitions>

hi: Rotation der Items bitte entfernen

\--------------------------------

F1_10
=====

tc:

vn: simmaba

qt: Drop-Down

hl:

in:

q: Wann haben Sie erstmals ein Studium in Deutschland aufgenommen?

is:

it:

st:




ao: (simmaba): [infield = Semester; 1: Sommersemester 2021 - 2: Wintersemester 20/21 - 3: Sommersemester 2020 - ... - 23: Sommersemester 2010 - 24: vor Sommersemester 2010] (Drop-Down)

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
            <zofar:transition target="F1_11"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_11
=====

tc:

vn: sabsabsba

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Planen Sie in Deutschland einen Hochschulabschluss zu erwerben?

is: Bitte beziehen Sie sich auf Ihr aktuelles Auslandsstudium.

is: 

it:

st:

ao1: 1: nein

ao2: 2: Ja, ich plane einen Studienabschluss in Deutschland (z. B. Bachelor, Master, Promotion).

ao3: 3: Ja, ich plane einen Doppelabschluss (Deutschland und anderes Land).

ao4: -12: weiß ich noch nicht 

mv: ao4

ka:

vc:

av:

kh:

fv:

hv:




fo: mv/"weiß ich noch nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_12"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_12
=====

tc:

vn: ainfcpba

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wird Ihr gegenwärtiger Auslandsaufenthalt auf Ihr Studium im Heimatland angerechnet?

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




fo: mv/"weiß ich nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_13"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_13
=====

tc:

vn: apro (apronoba; aproerasba; aprodaadba; aprohhsba; aprogahsba; aproanprba)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Findet Ihr aktueller Aufenthalt in Deutschland im Rahmen eines Austauschprogramms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (apronoba): nein (Exklusivkategorie)

ao2: (aproerasba): ERASMUS+

ao3: (aprodaadba): DAAD-Programm

ao4: (aprohhsba): Programm meiner Heimathochschule

ao5: (aprogahsba): Programm der Gasthochschule in Deutschland

ao6: (aproanprba): anderes Programm

mv:

ka: (ao2 TO ao6) Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo1: ao1 bitte etwas absetzen.  

fo2: Bitte über it2 "Ja, und zwar:" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_14"/>
        </zofar:transitions>

hi: 

\--------------------------------

F1_14
=====

tc:

vn: akont (akontdeustba; akontbuergba; akontheimba; akontintstba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig unterhalten Sie sich mit …

is:

it1: (akontdeustba): … deutschen Studierenden?

it2: (akontbuergba): … anderen deutschen Bürger\*innen?

it3: (akontheimba): … Studierenden aus Ihrem Heimatland?

it4: (akontintstba): … anderen internationalen Studierenden?

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
            <zofar:transition target="F1_15"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_15
=====

tc:

vn: azufrwillba; azufrsichba

qt: Einfachauswahl mit horizontalen ao 

hl:

in:

q1: (azufrwillba): Wie willkommen fühlen Sie sich in Deutschland?

q2: (azufrsichba): Wie sicher fühlen Sie sich in Deutschland insgesamt?

is:

it:

st:

ao1 (azufrwillba): 1: gar nicht willkommen

ao2 (azufrwillba): 2:

ao3 (azufrwillba): 3:

ao4 (azufrwillba): 4:

ao5 (azufrwillba): 5: sehr willkommen


ao6 (azufrsichba): 1: gar nicht sicher

ao7 (azufrsichba): 2:

ao8 (azufrsichba): 3:

ao9 (azufrsichba): 4:

ao10 (azufrsichba): 5: sehr sicher

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte zuerst q1 mit ao1-ao5 darstellen und darunter dann q2 mit ao6-ao10 darstellen.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_16"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_16
=====

tc:

vn: azuf (azuflernerfba; azufinsgba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie bis zum jetzigen Zeitpunkt mit …

is:

it1: (azuflernerfba): … den in Deutschland gewonnenen fachlichen Kenntnissen?

it2: (azufinsgba): … Ihrem Aufenthalt in Deutschland insgesamt?

st:

ao1: 1: gar nicht zufrieden

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
            <zofar:transition target="F1_17"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_17
=====

tc:

vn: azuf (azuforgaufba; azuffinaufba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und wie beurteilen Sie …

is:

it1: (azuforgaufba): … den organisatorischen Aufwand Ihres Aufenthaltes?

it2: (azuffinaufba): … den finanziellen Aufwand Ihres Aufenthaltes?

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
            <zofar:transition target="F1_18"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_18
=====

tc:

vn: aeempfba

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen: Würden Sie Ihren Freund\*innen/Bekannten empfehlen, in Deutschland zu studieren?

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
            <zofar:transition target="F1_20"/>
        </zofar:transitions>

hi:


\--------------------------------

F1_21
=====

tc:

vn: bdebleibba; bdebleibbao

qt: Einfachauswahl mit Zwischenüberschriften und vertikalen ao

hl:

in:

q: Was planen Sie direkt im Anschluss an Ihr Studium in Deutschland?

is:

it:

st:

ao1: 1: … in Deutschland.

ao2: 2: … in meinem Heimatland.

ao3: 3: … in einem anderen Land.

ao4: 4: … in Deutschland.

ao5: 5: … in meinem Heimatland.

ao6: 6: … in einem anderen Land.

ao7: 7: … und zwar: [(bdebleibbao); (offene Angabe); 250 Zeichen]

mv:

ka1 (ao1 TO ao3): !!Ich möchte arbeiten, und zwar …!!

ka2 (ao4 TO ao6): !!Ich möchte weiterstudieren/promovieren, und zwar …!!

ka3 (ao7): !!Etwas Anderes, ...!!

vc:

av:

kh:

fv:

hv:

fo1: Bitte über ao1 "Ich möchte arbeiten, und zwar …" mit etwas Abstand linksbündig positionieren.

fo2: Bitte über ao4 "Ich möchte weiterstudieren/promovieren, und zwar …" mit etwas Abstand linksbündig positionieren.

fo3: Bitte über ao7 "Etwas Anderes" mit etwas Abstand linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="F1_22"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_22
=====

tc:

vn: intpsy (intpsydaudeuba; intpsyzeitdeuba; intpsyherkba; intpsyandlba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsydaudeuba): in Deutschland

it2: (intpsyzeitdeuba): zeitweise in Deutschland

it3: (intpsyherkba): in meinem Heimatland

it4: (intpsyandlba): in einem anderen Land

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
            <zofar:transition target="F1_23"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_23
=====

tc:

vn: intling (intling1ba; intling2ba; intling3ba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie zu?

is:

it1: (intling1ba): Ich kann auf Deutsch über vertraute Themen sprechen und meine persönliche Meinung äußern.

it2: (intling2ba): Ich verstehe die wichtigsten Punkte in deutschen Radio- und Fernsehprogrammen.

it3: (intling3ba): Ich kann deutsche Zeitungsartikel lesen und verstehen.

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
            <zofar:transition target="F1_24"/>
        </zofar:transitions>

hi:

\--------------------------------

F1_24
=====

tc:

vn: aarbch (aarbchherkba; aarbchdeuba)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie schätzen Sie Ihre derzeitigen Berufs- und Arbeitsmarktchancen ein, und zwar in …

is:

it1: (aarbchherkba): … Ihrem Heimatland?

it2: (aarbchdeuba): … Deutschland?

st:

ao1: 1: sehr schlecht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut

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

\--------------------------------

F1_25
=====

tc:

vn: asprachgaslba; asprachheimlba; asprachandba; asprachandbao

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig sprechen Sie während Ihres Aufenthalts in Deutschland die folgenden Sprachen?

is:

it1: (asprachgaslba): Deutsch

it2: (asprachheimlba): Sprache Ihres Heimatlandes

it3: (asprachandba): Andere Sprache, und zwar: ([asprachandbao]; 60 Zeichen)

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

hi:
