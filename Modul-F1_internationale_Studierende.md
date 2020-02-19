F1_1
====

tc:

vn: aeinnorm1; aeinnorm2; aeinnorm3

qt: Einfachauswahlmaxtrix und offene Angabe

hl:

in:

q: Inwiefern treffen die folgenden Aussagen Ihrer Meinung nach zu?

is:

it1: (aeinnorm1): : Ein studienbezogener Auslandsaufenthalt darf während des Studiums auf keinen Fall fehlen.

it2: (aeinnorm2): : Auslandserfahrungen werden auf dem Arbeitsmarkt oftmals erwartet.

it3: (aeinnorm3): : Jede*r Studierende sollte während des Studiums studienbezogen im Ausland gewesen sein.

st:

ao1: 1: : trifft gar nicht zu

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

		<zofar:transitions>
			<zofar:transition target="F1_2b" condition="width.value lt 768"/>
			<zofar:transition target="F1_2"/>
		</zofar:transitions>


hi: Items bitte zufällig rotieren

\-------------------------------

F1_2
====

tc:

vn: aeinsarbm; aeinssprachk; aeinsfach; aeinspersön; aeinskont; aeinskultur; aeinsspaß; aeinsfinanz; aeinsorga; aeinsfreun; aeinsanerk; aeinszeit; aeinsfehlspra; aeinsangstl

qt: Einfachauswahlmatrix

hl:

in:

q: Was spricht Ihrer Meinung nach …

is:

Überschrift: … für einen Auslandsenthalt?

it1 (aeinsarbm): verbesserte Arbeitsmarktaussichten

it2 (aeinssprachk): verbesserte Sprachkenntnisse

it3 (aeinsfach): verbesserte Fachkenntnisse

it4 (aeinspersön): Persönlichkeitsentwicklung

it5 (aeinskont): international Kontakte knüpfen

it6 (aeinskultur): andere Länder/Kulturen kennenlernen

it7 (aeinsspaß): Spaß haben

Überschrift: … gegen einen Auslandsaufenthalt?

it8 (aeinsfinanz): finanzielle Belastung

it9 (aeinsorga): Organisationsaufwand

it10 (aeinsfreun): Trennung von Freunden und Familie

it11 (aeinsanerk): Anerkennungsschwierigkeiten

it12 (aeinszeit): Zeitverlust

it13 (aeinsfehlspra): fehlende Sprachkenntnisse

it14 (aeinsangstl): Angst vor fremder Studien- und Lebenssituation

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

hi:

\--------------------------------

F1_2b
====

tc:

vn: aeinsarbm; aeinssprachk; aeinsfach; aeinspersön; aeinskont; aeinskultur; aeinsspaß

qt: Einfachauswahlmatrix

hl:

in:

ao1: 1: : überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

q: Was spricht Ihrer Meinung nach für einen Auslandsaufenthalt?

is:

it1 (aeinsarbm): verbesserte Arbeitsmarktaussichten

it2 (aeinssprachk): verbesserte Sprachkenntnisse

it3 (aeinsfach): verbesserte Fachkenntnisse

it4 (aeinspersön): Persönlichkeitsentwicklung

it5 (aeinskont): international Kontakte knüpfen

it6 (aeinskultur): andere Länder/Kulturen kennenlernen

it7 (aeinsspaß): Spaß haben

st:

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

qt: Einfachauswahlmatrix

hl:

in:

ao1: 1: : überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

q: Was spricht Ihrer Meinung nach gegen einen Auslandsaufenthalt?

is:

it8 (aeinsfinanz): finanzielle Belastung

it9 (aeinsorga): Organisationsaufwand

it10 (aeinsfreun): Trennung von Freunden und Familie

it11 (aeinsanerk): Anerkennungsschwierigkeiten

it12 (aeinszeit): Zeitverlust

it13 (aeinsfehlspra): fehlende Sprachkenntnisse

it14 (aeinsangstl): Angst vor fremder Studien- und Lebenssituation

st:

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


F1_3
====

tc:

vn: ainfpfakt

qt: Einfachauswahl

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

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Kennen Sie jemanden, der bereits vor Ihnen im Rahmen seines Studiums im Ausland war?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (avorelt) : Eltern

ao2: (avorgeschw) : Geschwister

ao3: (avorandver) : andere Verwandte

ao4: (avorfreund) : Freund*innen

ao5: (avorkomm) : Kommiliton*innen

ao6: (avorniem) : nein, niemanden (Exklusivkategorie)

mv:

ka:

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

vn: aauszeitlebnein; aauszeitlebfrkin; aauszeitlebwschul; aauszeitlebnschul; aauszeitlebbama

qt: Mehrfachauswahl

hl:

in:

q: Haben Sie im Laufe Ihres Lebens eine längere Zeit (durchgängig mehr als 3 Monate) im Ausland verbracht?

is: Bitte alles Zutreffende auswählen

it:

st:

ao1: (aauszeitlebnein): nein

ao2: (aauszeitlebfrkin): ja, in meiner frühen Kindheit

ao3: (aauszeitlebwschul): ja, während meiner Schulzeit

ao4: (aauszeitlebnschul): ja, direkt nach der Schulzeit

ao5: (aauszeitlebbama): ja, zwischen meinem Bachelor- und Masterstudium

mv:

ka:

vc: SHOW aauszeitlebbama IF sabsan=2 or sabsan=MISSING

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

qt: Einfachauswahl

hl:

in:

q: Haben Sie in Deutschland ein Studienkolleg besucht?

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

tr: GOTO F1_7

hi:

\--------------------------------

F1_7
====

tc:

vn: vsbanrechsch

qt: Einfachauswahl

hl:

in:

q: Hatten Sie Schwierigkeiten bei der Anerkennung Ihrer Vorbildung in Deutschland?

it:

st:

ao1: 1: : nein, keine Schwierigkeiten

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : ja, sehr viele Schwierigkeiten

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

vn: intdeutsch1; intdeutsch2; intdeutsch3; intdeutsch4; intdeutsch5

qt: Mehrfachauswahl

hl:

in:

q: Wo haben Sie die nötigen Sprachkenntnisse für ein Studium in Deutschland erworben?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intdeutsch1): Schule/Studium im Ausland

ao2: (intdeutsch2): Sprachkurs im Ausland

ao3: (intdeutsch3): Sprachkurs in Deutschland (vor dem Studium)

ao4: (intdeutsch4): Studienbegleitend an einer deutschen Hochschule

ao5: (intdeutsch5): bisher noch gar nicht

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

vn: bdefinba; bdekenba; bdesprba; bdefamsba; bdefamlba; bdetecba; bdeoekba; bdequaba; bdearbba

qt: Einfachauswahlmatrix

hl:

in:

q: Warum haben Sie sich für ein Studium in Deutschland entschieden?

is: Bitte geben Sie den jeweils zutreffenden Skalenwert an.

Ich habe mich für ein Studium in Deutschland entschieden, ...

it1 (bdefinba): weil dies meinen finanziellen Möglichkeiten entspricht.

it2 (bdekenba): um Deutschland kennenzulernen/weil mich die deutsche Geschichte und Kultur interessiert.

it3 (bdesprba): um meine Sprachkenntnisse zu vertiefen.

it4 (bdefamsba): weil Freunde/Verwandte in Deutschland studieren/studiert haben.

it5 (bdefamlba): weil Freunde/Verwandte in Deutschland leben/gelebt haben.

it6 (bdetecba): weil Deutschland ein hochtechnisiertes Land ist.

it7 (bdeoekba): wegen der wirtschaftlichen Lage in Deutschland.

it8 (bdequaba): wegen der Lebensqualität in Deutschland.

it9 (bdearbba): aufgrund der Möglichkeit, nach Studienabschluss in Deutschland zu arbeiten.

st:

ao1: 1: : trifft gar nicht zu

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

tr: GOTO F1_10

hi: Items bitte zufällig rotieren.

\--------------------------------

F1_10
=====

tc:

vn: ainfaba; ainfbmba; ainfbjba; ainfemba, ainfejba

qt: Akkordeon (Drop-Down Menüs, offene Angabe)

hl:

in:

q: Bitte beschreiben Sie Ihren aktuellen Aufenthalt in Deutschland näher.

is:

it:

st:

Drop-Down-Menü:
Art des Auslandsaufenthalts:

aox (ainfaba): 0: : Art des Auslandsaufenthalts

ao1 (ainfaba): 1: : Auslandsstudium mit Abschluss in Deutschland

ao2 (ainfaba): 2: : Auslandsstudium/-semester ohne Abschluss in Deutschland

ao3 (ainfaba): 3: : Praktikum/Praxisphase

ao4 (ainfaba): 4: : Sprachkurs

ao5 (ainfaba): 5: : Studienreise

ao6 (ainfaba): 6: : Projektarbeit

ao7 (ainfaba): 7: : Summerschool

ao8 (ainfaba): 8: : sonstiger Aufenthalt


Beginn:

Untereinander angeordnete Drop-Down-Menüs

ao9 (ainfbmba): : Monat: (Monat \ Januar \| … \| Dezember)

ao10 (ainfbjba): : Jahr: (Jahr \ 2020 \| 2019 \| … \| 2000 \| vor 2000)


Ende:

Untereinander angeordnete Drop-Down-Menüs

ao11 (ainfemba): : Monat: (Monat \ Januar \| … \| Dezember)

ao12 (ainfejba): Jahr: (Jahr \ 2020 \| 2021 \| … \| 2030 oder später)

mv:

ka:ka1 (ao0 -ao12): aktueller Studienbezogener Auslandsaufenthalt - bitte auswählen

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

ao1: 1: : Nein, ich werde in Deutschland nur einen Teil meines Studiums absolvieren.

ao2: 2: : Ja, ich plane den Abschluss eines Studiums in Deutschland (z. B. Bachelor, Master, Promotion).

ao3: 3: : Ja, ich plane einen Doppelabschluss in Deutschland un in meinem Herkunftsland/einem anderen Land.

ao4: 4: : weiß ich noch nicht

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

ao1: 1: : nein

ao2: 2: : offene Angabe: 2 Stellen Präfix: ja, teilweise:[ainfcp1osba], Suffix: ECTS-Punkte

ao3: 3: : offene Angabe: 2 Stellen Präfix: ja, vollstädnig:[ainfcp2osba], Suffix: ECTS-Punkte

ao: -12: : weiß ich nicht

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

ao1 (aproselbba): : nein, ich habe den Aufenthalt selbst organisiert (Exklusivkategorie)

ao2 (aprokoopba): : ja, Kooperationsprogramm zwischen Heimathochschule und deutscher Hochschule

ao3 (aproorigba): : ja, Programm meines Herkunftslandes

ao4 (aprodaadba): : ja, deutsches Programm (z. B. DAAD-Programm)

ao5 (aproerasba): : ja, ERASMUS+/ERASMUS-Programm

ao6 (aproeuba): : ja, anderes EU-Programm

ao7 (aprointerba): : ja, Programm meiner Gasthochschule im Ausland

ao8 (aproanprba): : ja, anderes Programm und zwar: offene Angabe: 100 Stellen, Präfix [aproanproba]

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

it1 (akontdeutstba): … Studierenden aus Deutschland?

it2 (akonteinheimba): … anderen Einheimischen?

it3 (akontheimba): … Studierenden aus Ihrem Heimatland?

it4 (akontintstba): … anderen internationalen Studierenden (nicht aus Ihrem Heimatland)?

st:

ao1: 1: : nie

ao2: 2: : selten

ao3: 3: : manchmal

ao4: 4: : häufig

ao5: 5: : sehr häufig

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

ao1: 1: : gar nicht willkommen

ao2: 2

ao3: 3:

ao4: 4

105: 5: : sehr willkommen

für q2:

ao1: 1: : gar nicht sicher

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr sicher

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

it1 (azufskein): … dem Kontakt zu Einheimischen?

it2 (azufskstu): … dem Kontakt zu Studierenden?

it3 (azufsklehr): … dem Kontakt zu Lehrenden?

it4 (azuflernerf): … den gewonnenen fachlichen Kenntnissen?

it5 (azufinsg): … Ihrem Aufenthalt in Deutschland insgesamt?

st:

ao1: 1: : überhaupt nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr zufrieden

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

it1 (azufleistanf): … die Leistungsanforderungen an Ihrer Hochschule?

it2 (azuforgaaufw): … den organisatorischen Aufwand Ihres Aufenthaltes?

it3 (azuffinanzaufw): … den finanziellen Aufwand Ihres Aufenthaltes?

st:

ao1: 1: : sehr niedrig

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr hoch

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

ao1 (adeempfba): 1: : nein, überhaupt nicht

ao2 (adeempfba): 2

ao3 (adeempfba): 3

ao4 (adeempfba): 4

ao5 (adeempfba): 5 : : ja, unbedingt

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

F1_19
=====

tc:

vn: bdedarlba; bdedarloba; bdedarhssia; bdedarhsoba

qt: offene Angabe

hl:

in:

q: Wenn Sie nochmals vor der Wahl stünden: In welchem Land, in welcher Stadt beziehungsweise an welcher Hochschule hätten Sie am liebsten Ihren studienbezogenen Auslandsaufenthalt durchgeführt?

is:

it1 (bdedarlba): Land: (offene Angabe: 100 Zeichen, Präfix [bdedarloba], Suffix …

it2 (bdedarhssia): Stadt/Hochschule: (offene Angabe: 100 Zeichen, Präfix [bdedarhsoba], Suffix …

it1 (-12): weiß ich nicht

st:

ao:

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

ao1 (bhiitecba): : Einführung in wissenschaftliche Lern- und Arbeitstechniken

ao2 (bhiiwelba): : Welcome-/Begrüßungsveranstaltungen

ao3 (bhiivorbba): : fachliche Vorbereitungskurse

ao4 (bhiitutba): : studienbegleitende Tutorien

ao5 (bhiiheimba): : Betreuungsangebote in Wohnheimen

ao6 (bhiivermba): : Vermittlung von Wohnraum

ao7 (bhiideuba): : Deutschkurse

ao8 (bhiiberba): : Studienberatung

ao9 (bhiibehba): : Hilfe im Umgang mit Behörden

ao10 (bhiikulba): : Kultur- und Freizeitangebote

ao11 (bhiikomba): : Kommunikationsmöglichkeiten mit deutschen Studierenden

ao12 (bhiifinba): : Informationen zur Finanzierung des Studiums

ao13 (bhiiaerlba): : Beratung/Informationen zu Fragen der Arbeitserlaubnis

ao14 (bhiivisba): : Beratung/Informationen zum Aufenthaltsrecht

ao15 (bhiikvba): Beratung/Informationen zu Fragen der Krankenversicherung

ao16 (bhiipsyba): : psychologische Beratung bei persönlichen oder studienbezogenen Schwierigkeiten

ao17 (bhiikeinba): : kein Angebot genutzt (Exklusivkategorie)

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

Ich möchte Arbeiten, und zwar …

ao1: … in Deutschland.

ao2: … in meinem Heimatland.

ao3: … in einem anderen Land.

Ich möchte weiterstudieren, und zwar …

ao4: … in Deutschland.

ao5: … in meinem Heimatland.

ao6: … in einem anderen Land.

Etwas Anderes

ao7: Sonstiges

mv:

ka:

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

it1 (intpsyherkba): in meinem Heimatland

it2 (intpsyzeitdeu): zeitweise in Deutschland

it3 (intpsyanddeu): dauerhaft in Deutschland

st:

ao1: 1: : auf keinen Fall

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : auf jeden Fall

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

it1 (intling1ba): Ich kann auf Deutsch über vertraute Themen sprechen und meine persönliche Meinung äußern.

it2 (intling2ba): Ich verstehe die wichtigsten Punkte in deutschen Radio- und Fernsehprogrammen.

it3 (intling3ba): Ich kann deutsche Zeitungsartikel lesen und verstehen.

st:

ao1: 1: : trifft gar nicht zu

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

it1 (aarbchdeuba): … Deutschland?

it2 (aarbchherkba): … Ihrem Herkunftsland?

st:

ao1: 1: :überhaupt nicht gut

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr gut

ao6: 6: : kann ich nicht beurteilen

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
