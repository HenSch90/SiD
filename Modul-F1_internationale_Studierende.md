F1_1
====

tc:

vn: aeinnorm1; aeinnorm2

qt:  Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwiefern treffen die folgenden Aussagen Ihrer Meinung nach zu?

is:

it1: (aeinnorm1): Ein Auslandsaufenthalt darf während des Studiums auf keinen Fall fehlen.

it2: (aeinnorm2): Auslandserfahrungen werden auf dem Arbeitsmarkt oftmals erwartet.

st:

ao1: 1: : trifft überhaupt nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_2b IF width.value lt 768

ELSE GOTO F1_2

hi:

\-------------------------------

F1_2
====

tc:

vn: aeinsarbm; aeinssprachk; aeinsfach; aeinspersoen; aeinskont; aeinskultur; aeinsspas; aeinsfinanz; aeinsorga; aeinsfreun; aeinsanerk; aeinszeit; aeinsfehlspra; aeinsangstl

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Was spricht Ihrer Meinung nach…

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

ao1: 1: : überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

mv:

ka1: (it1 TO it7) **… *für* einen Auslandsaufenthalt?**

ka2: (it8 TO it it14) **… *gegen* einen Auslandsaufenthalt?**

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_3

hi:

\--------------------------------

F1_2b
====

tc: 

vn: aeinsarbm; aeinssprachk; aeinsfach; aeinspersoen; aeinskont; aeinskultur; aeinsspas

qt:  Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Was spricht Ihrer Meinung nach für einen Auslandsaufenthalt?

is:

it1: (aeinsarbm): Verbesserung der Arbeitsmarktchancen

it2: (aeinssprachk): Verbesserung der Sprachkenntnisse

it3: (aeinsfach): Verbesserung der Fachkenntnisse

it4: (aeinspersoen): Persönlichkeitsentwicklung

it5: (aeinskont): Kontakte knüpfen

it6: (aeinskultur): andere Kulturen kennenlernen

it7: (aeinsspas): Spaß haben

st:

ao1: 1: : überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_2c

hi: Items bitte zufällig rotieren.

\-------------------------------

F1_2c
====

tc:

vn: aeinsfinanz; aeinsorga; aeinsfreun; aeinsanerk; aeinszeit; aeinsfehlspra; aeinsangstl

qt:  Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und was spricht Ihrer Meinung nach gegen einen Auslandsaufenthalt?

is:

it8: (aeinsfinanz): finanzielle Belastung

it9: (aeinsorga): Organisationsaufwand

it10: (aeinsfreun): Trennung von Freund\*innen und Familie

it11: (aeinsanerk): Anerkennungsschwierigkeiten

it12: (aeinszeit): Zeitverlust

it13: (aeinsfehlspra): fehlende Sprachkenntnisse

it14: (aeinsangstl): Angst vor fremder Studien- und Lebenssituation

st:

ao1: 1: : überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_3

hi: Items bitte zufällig rotieren.

\-------------------------------

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

ao1: 1: : nein

ao2: 2: : ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_4

hi:

\--------------------------------

F1_4
====

tc:

vn: avorelt; avorgeschw; avorandver; avorfreund; avorkomm; avorniem

qt: Mehrfachauswahl mit Exklusivkategorie und mit vertikalen ao

hl:

in:

q: Kennen Sie jemanden, der bereits vor Ihnen im Rahmen seines Studiums im Ausland war?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (avorniem) : nein, niemanden (Exklusivkategorie)

ao2: (avorelt) : Eltern

ao3: (avorgeschw) : Geschwister

ao4: (avorandver) : andere Verwandte

ao5: (avorfreund) : Freund\*innen

ao6: (avorkomm) : Kommiliton\*innen

mv:

ka: (it2 TO it6) ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_5

hi:

\--------------------------------

F1_5
====

tc:

vn: aauszeitlebnein; aauszeitlebfrkin; aauszeitlebwschul; aauszeitlebnschul

qt: Mehrfachauswahl mit Exklusivkategorie und mit vertikalen ao

hl:

in:

q: Haben Sie im Laufe Ihres Lebens eine längere Zeit (durchgängig mehr als 3 Monate) im Ausland verbracht?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aauszeitlebnein): nein (Exklusivkategorie)

ao2: (aauszeitlebfrkin): ja, in meiner frühen Kindheit

ao3: (aauszeitlebwschul): ja, während meiner Schulzeit

ao4: (aauszeitlebnschul): ja, direkt nach der Schulzeit

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 
GOTO F1_6 IF (vsbdeba=2 AND dnatausl=1 AND imausl=1)

GOTO F2_6 IF (vsbdeba=1 AND dnatdeu=1 AND imausl=2)

GOTO F2_6 IF (vsbdeba=1 AND dnatdeu=MISSING AND imausl=2)
GOTO F2_6 IF (vsbdeba=MISSING AND dnatdeu=1 AND imausl=2)
GOTO F2_6 IF (vsbdeba=MISSING AND dnatdeu=MISSING AND imausl=2)

GOTO F3_6 IF (vsbdeba=1 AND dnatdeu=1 AND imausl=1)

GOTO F3_6 IF (vsbdeba=1 AND dnatdeu=1 AND imausl=MISSING)
GOTO F3_6 IF (vsbdeba=1 AND dnatdeu=MISSING AND imausl=1)
GOTO F3_6 IF (vsbdeba=MISSING AND dnatdeu=1 AND imausl=1)

GOTO F1_6 IF (vsbdeba=2 AND dnatausl=1 AND imausl=MISSING)
GOTO F1_6 IF (vsbdeba=2 AND dnatausl=MISSING AND imausl=1)
GOTO F1_6 IF (vsbdeba=2 AND dnatausl=MISSING AND imausl=MISSING)


ALTERNATIV:

<zofar:transition target="F1_6" condition="(zofar.asNumber(vsbdeba)==2)"/>		

<zofar:transition target="F2_6" condition="(zofar.asNumber(vsbdeba)==1 					  			and zofar.asNumber(imausl)==2)"/>

<zofar:transition target="F2_6" condition="(zofar.isMissing(vsbdeba) 
					and zofar.asNumber(imausl)==2)"/>

<zofar:transition target="F3_6" condition="(zofar.asNumber(vsbdeba)==1 
					and zofar.asNumber(imausl)==1)"/>

<zofar:transition target="F3_6" condition="(zofar.asNumber(vsbdeba)==1 
					and zofar.isMissing(imausl))"/>
					
<zofar:transition target="F3_6" condition="(zofar.isMissing(vsbdeba) 
					and zofar.isMissing(imausl))"/>
                      
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

tr: GOTO F1_7

hi:

\--------------------------------

F1_7
====

tc:

vn: vsbanrechsch

qt: Einfachauswahl mit horizontalen ao

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

tr: GOTO F1_8

hi:

\--------------------------------

F1_8
====

tc:

vn: intdeutsch1; intdeutsch2; intdeutsch3; intdeutsch4; intdeutsch5; intdeutsch6

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Wo haben Sie die nötigen Sprachkenntnisse für ein Studium in Deutschland erworben?

is: *Bitte alles Zutreffende auswählen.*

it:

st:

ao1: (intdeutsch1): Elternhaus

ao2: (intdeutsch2): Schule/Studium im Ausland

ao3: (intdeutsch3): Sprachkurs im Ausland

ao4: (intdeutsch4): Sprachkurs in Deutschland (vor dem Studium)

ao5: (intdeutsch5): studienbegleitend an einer deutschen Hochschule

ao6: (intdeutsch6): bisher noch gar nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_9

hi:

\--------------------------------

F1_9
====

tc:

vn:  bdequaba; bdefamsba; bdeoekba; bdefinba; bdesprba; bdearbba; bdekenba 

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Warum haben Sie sich für Deutschland als Studienland entschieden?

is: !!Ich habe mich für ein Studium in Deutschland entschieden, ...!!

it1: (bdequaba): aufgrund der hohen Lebensqualität.

it2: (bdefamsba): weil bereits Freund\*innen/Verwandte in Deutschland studiert haben.

it3: (bdeoekba): aufgrund der wirtschaftlichen Lage in Deutschland.

it4: (bdefinba): weil dies meinen finanziellen Möglichkeiten entspricht.

it5: (bdesprba): um meine Sprachkenntnisse zu vertiefen.

it6: (bdearbba): um nach Studienabschluss in Deutschland zu arbeiten.

it7: (bdekenba): um Deutschland kennenzulernen.

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

tr: GOTO F1_10

hi: Items bitte zufällig rotieren.

\--------------------------------

F1_10
=====

tc:

vn: 

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Wann haben Sie erstmals ein Studium in Deutschland aufgenommen?

is:

it:

st:

ao: [Dropdown, Semesterliste: Semester; SoSe2020, WiSe2019/2020 bis SoSe2010]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:  GOTO F1_11

hi:

\--------------------------------

F1_11
=====

tc:

vn: sabsabsba

qt: Einfachauswahl

hl:

in:

q: Planen Sie, in Deutschland einen Hochschulabschluss zu erwerben?

is: Bitte beziehen Sie sich auf Ihren aktuellen Studiengang.

it:

st:

ao1: 1: Nein, ich werde in Deutschland nur einen Teil meines Studiums absolvieren.

ao2: 2: Ja, ich plane den Abschluss eines Studiums in Deutschland (z. B. Bachelor, Master, Promotion).

ao3: 3: Ja, ich plane einen Doppelabschluss in Deutschland un in meinem Herkunftsland/einem anderen Land.

ao4: 4: weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_12

hi:

\--------------------------------

F1_12
=====

tc:

vn: ainfcpba; ainfcp1osba; ainfcp2osba

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Werden Ihnen die in Deutschland erbrachten Studienleistungen auf Ihr Studium an Ihrer Heimatuniversität angerechnet?
is:

it:

st:

ao1: 1: nein

ao2: 2: offene Angabe: 2 Stellen Präfix: ja, teilweise:[ainfcp1osba], Suffix: ECTS-Punkte

ao3: 3: offene Angabe: 2 Stellen Präfix: ja, vollständig:[ainfcp2osba], Suffix: ECTS-Punkte

ao4: 4: weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_13

hi:

\--------------------------------

F1_13
=====

tc:

vn: aproselbba; aprokoopba; aproorigba; aprodaadba; aproerasba; aproeuba; aprointerba; aproanprba; aproanproba

qt: Mehrfachnennung

hl:

in:

q: Findet Ihr aktueller Aufenthalt in Deutschland im Rahmen eines Austauschprogramms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aproselbba): nein, ich habe den Aufenthalt selbst organisiert (Exklusivkategorie)

ao2: (aprokoopba): ja, Kooperationsprogramm zwischen Heimathochschule und deutscher Hochschule

ao3: (aproorigba): ja, Programm meines Herkunftslandes

ao4: (aprodaadba): ja, deutsches Programm (z. B. DAAD-Programm)

ao5: (aproerasba): ja, ERASMUS+/ERASMUS-Programm

ao6: (aproeuba): ja, anderes EU-Programm

ao7: (aprointerba): ja, Programm meiner Gasthochschule im Ausland

ao8: (aproanprba): ja, anderes Programm und zwar: offene Angabe: Präfix [100 Zeichen, aproanproba]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_14

hi: Items bitte zufällig rotieren.

\--------------------------------

F1_14
=====

tc:

vn: akontdeutstba; akonteinheimba; akontheimba; akontintstba

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig haben Sie während Ihres Aufenthalts in Deutschland Kontakt mit …

is:

it1: (akontdeutstba): … Studierenden aus Deutschland?

it2: (akonteinheimba): … anderen Einheimischen?

it3: (akontheimba): … Studierenden aus Ihrem Heimatland?

it4: (akontintstba): … anderen internationalen Studierenden (nicht aus Ihrem Heimatland)?

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

tr: GOTO F1_15

hi:

\--------------------------------

F1_15
=====

tc:

vn: azufrwillba; azufrsichba

qt: Einfachauswahl

hl:

in:

q1: (azufrwillba): Wie willkommen fühlen Sie sich in Deutschland?

q2: (azufrsichba): Wie sicher fühlen Sie sich bislang in Deutschland insgesamt?

is:

it:

st:

für q1:

ao1: 1: gar nicht willkommen

ao2: 2:

ao3: 3:

ao4: 4:

a05: 5: sehr willkommen

für q2:

ao1: 1: gar nicht sicher

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr sicher

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_16

hi:

\--------------------------------

F1_16
=====

tc:

vn: azufskein; azufskstu; azufsklehr; azuflernerf; azufinsg

qt: Einfachauswahlmatrix, Akkordeon

hl:

in:

q: Wie zufrieden sind Sie bis zum jetzigen Zeitpunkt mit …...

is:

it1: (azufskein): … dem Kontakt zu Einheimischen?

it2: (azufskstu): … dem Kontakt zu Studierenden?

it3: (azufsklehr): … dem Kontakt zu Lehrenden?

it4: (azuflernerf): … den gewonnenen fachlichen Kenntnissen?

it5: (azufinsg): … Ihrem Aufenthalt in Deutschland insgesamt?

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

tr: GOTO F1_17

hi:

\--------------------------------

F1_17
=====

tc:

vn: azufleistanf; azuforgaaufw; azuffinanzaufw

qt: Einfachauswahl, Akkordeon

hl:

in:

q: Und wie beurteilen Sie …

is:

it1: (azufleistanf): … die Leistungsanforderungen an Ihrer Hochschule?

it2: (azuforgaaufw): … den organisatorischen Aufwand Ihres Aufenthaltes?

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

tr: GOTO F1_18

hi:

\--------------------------------

F1_18
=====

tc:

vn: adeempfba

qt: Einfachauswahl

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen mit den Studien- und Lebensbedingungen in Deutschland: Würden Sie Ihren Freunden/Bekannten empfehlen, in Deutschland zu studieren?

is:

it:

st:

ao1: (adeempfba): 1: nein, überhaupt nicht

ao2: (adeempfba): 2: 

ao3: (adeempfba): 3: 

ao4: (adeempfba): 4: 

ao5: (adeempfba): 5: ja, unbedingt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_20

hi:


\--------------------------------

F1_20
=====

tc:

vn: bhiitecba; bhiiwelba; bhiivorbba; bhiitutba; bhiiheimba; bhiivermba; bhiideuba; bhiiberba; bhiibehba; bhiikulba; bhiikomba; bhiifinba; bhiiaerlba; bhiivisba; bhiikvba; bhiipsyba; bhiikeinba

qt: Mehrfachauswahl

hl:

in:

q: Welche dieser Hilfestellungen für Studierende haben Sie bisher genutzt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (bhiitecba): Einführung in wissenschaftliche Lern- und Arbeitstechniken

ao2: (bhiiwelba): Welcome-/Begrüßungsveranstaltungen

ao3: (bhiivorbba): fachliche Vorbereitungskurse

ao4: (bhiitutba): studienbegleitende Tutorien

ao5: (bhiiheimba): Betreuungsangebote in Wohnheimen

ao6: (bhiivermba): Vermittlung von Wohnraum

ao7: (bhiideuba): Deutschkurse

ao8: (bhiiberba): Studienberatung

ao9: (bhiibehba): Hilfe im Umgang mit Behörden

ao10: (bhiikulba): Kultur- und Freizeitangebote

ao11: (bhiikomba): Kommunikationsmöglichkeiten mit deutschen Studierenden

ao12: (bhiifinba): Informationen zur Finanzierung des Studiums

ao13: (bhiiaerlba): Beratung/Informationen zu Fragen der Arbeitserlaubnis

ao14: (bhiivisba): Beratung/Informationen zum Aufenthaltsrecht

ao15: (bhiikvba): Beratung/Informationen zu Fragen der Krankenversicherung

ao16: (bhiipsyba): psychologische Beratung bei persönlichen oder studienbezogenen Schwierigkeiten

ao17: (bhiikeinba): kein Angebot genutzt (Exklusivkategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_21

hi:

\--------------------------------

F1_21
=====

tc:

vn: bdebleibba

qt: Einfachauswahl

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

ao7: 7: Sonstiges

mv:

ka1 (ao1 TO ao3): Ich möchte Arbeiten, und zwar...

ka2 (ao4 TO ao6): Ich möchte weiterstudieren, und zwar...

ka3 (ao7): Etwas Anderes

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_22

hi:

\--------------------------------

F1_22
=====

tc:

vn: intpsyherkba; intpsyzeitdeu; intpsyanddeu

qt: Einfachauswahlmatrix

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsyherkba): in meinem Heimatland

it2: (intpsyzeitdeu): zeitweise in Deutschland

it3: (intpsyanddeu): dauerhaft in Deutschland

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

tr: GOTO F1_23

hi:

\--------------------------------

F1_23
=====

tc:

vn: intling1ba; intling2ba; intling3ba

qt: Einfachauswahlmatrix

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

tr: GOTO F1_24

hi:

\--------------------------------

F1_24
=====

tc:

vn: aarbchdeuba; aarbchherkba

qt: Einfachauswahlmatrix

hl:

in:

q: Wie schätzen Sie Ihre derzeitigen Berufs- und Arbeitsmarktchancen ein, und zwar in…

is:

it1: (aarbchdeuba): … Deutschland?

it2: (aarbchherkba): … Ihrem Herkunftsland?

st:

ao1: 1: überhaupt nicht gut

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut

ao6: 6: kann ich nicht beurteilen

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_56

hi:
