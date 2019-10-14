F1_1
====

tc:

vn: aeinnormba1; aeinnormba2; aeinnormba3; aeinnormando; aeinnormando

qt: Einfachauswahlmaxtrix und offene Angabe

hl:

in:

q: Inwiefern treffen die folgenden Aussagen Ihrer Meinung nach zu?

is:

it1: (aeinnorm1): : Ein studienbezogener Auslandsaufenthalt darf während des
Studiums auf keinen Fall fehlen.

it2: (aeinnorm2): : Auslandserfharungen warden auf dem Arbeitsmarkt oftmals
erwartet.

it3: (aeinnorm3): : Jede\*r Studierende sollte während des Studiums
studienbezogen im Ausland gewesen sein.

it4: (aeinnormand): anderes, und zwar (offene Angabe: 100 Zeichen; Präfix
[aeinnormando], Suffix

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

tr:

GOTO F1_2

hi: Items bitte zufällig rotieren (Ausnahme: aeinnormandoba)

\-------------------------------

F1_2
====

tc:

vn: aeinsarbm; aeinssprachk; aeinsfach; aeinspersön; aeinskont; aeinskultur;
aeinsspaß; aeinsfinanz; aeinsorga; aeinsfreun; aeinsanerk; aeinszeit;
aeinsfehlspra; aeinsangstl

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

tr:

GOTO F1_3

hi:

\--------------------------------

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

tr:

GOTO F1_4

hi:

\--------------------------------

F1_4
====

tc:

vn: avorelt; avorgeschw; avorandver; avorfreund; avorkomm; avorniem

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Kennen Sie jemanden, der bereits vor Ihnen im Rahmen seines Studiums im
Ausland war?

is: Mehrfachauswahl

it:

st:

ao1: (avorelt) : Eltern

ao2: (avorgeschw) : Geschwister

ao3: (avorandver) : andere Verwandte

ao4: (avorfreund) : Freunde

ao5: (avorkomm) : Kommiliton\*innen

ao6: (avorniem) : nein, niemanden (Exklusivkategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_5

hi:

\--------------------------------

F1_5
====

tc:

vn: aauszeitlebnein; aauszeitlebfrkin; aauszeitlebwschul; aauszeitlebnschul;
aauszeitlebbama

qt: Mehrfachauswahl

hl:

in:

q: Haben Sie im Laufe Ihres Lebens eine längere Zeit (durchgängig mehr als 3
Monate) Im Ausland verbracht?

is: Bitte alles Zutreffende ankreuzen.

it:

st:

ao1: (aauszeitlebnein): nein

ao2: (aauszeitlebfrkin): ja, in meiner frühen Kindheit

ao3: (aauszeitlebwschul): ja, während meiner Schulzeit

ao4: (aauszeitlebnschul): ja, direkt nach der Schulzeit

ao5: (aauszeitlebbama): ja, zwischen meinem Bachelor- und Masterstudium

mv:

ka:

vc: SHOW aauszeitlebbama IF sabsan=2

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_6

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

tr:

GOTO F1_7

hi:

\--------------------------------

F1_7
====

tc:

vn: vsbanrechsch

qt: Einfachauswahlmatrix

hl:

in:

q: Hatten Sie Schwierigkeiten bei der Anerkennung Ihrer Vorbildung in
Deutschland?

it:

st:

ao1: 1: : nein, überhaupt nicht

ao2: 2

ao3: 3: : teils, teils

ao4: 4

ao5: 5: : ja, sehr viele Schwierigkeiten

ao6: 6: : weiß ich nicht (Exklusivkategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_8

hi:

\--------------------------------

F1_8
====

tc:

vn: vsbpruefba; vsbeignba; vsbhsreifba; ssbbachba; vsbmastba; vsbteilba; vsbwnba

qt: Mehrfachauswahl

hl:

in:

q: Wie wurde Ihre Vorbildung in Deutschland anerkannt?

it:

st:

ao1: (vsbpruefba) :nach einer Feststellungsprüfung als Studienberechtigbung (z.
B. am Studienkolleg an einer Hochschule)

ao2: (vsbeignba): nach einer Eignungsprüfung (z. B. für Kunst, Sport) an einer
Hochschule als Studienberechtigung

ao3: (vsbhsreifba): als fachorientierte oder nicht-fachorientierte
Studienberechtigung

ao4: (vsbbachba): als Bachelorabschluss

ao5: (vsbmastba): als Master-/Dipolom-/Magisterabschluss

ao6: (vsbteilba): von meinen Studienleistungen wurden Teile anerkannt (z. B.
einzelne Studienleistungen, Credit Points, Module, Scheine)

ao7: (vsbwnba): weiß ich nicht (Exklusivkategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_9

hi:

\--------------------------------

F1_9
====

tc:

vn: bdefinba; bdekenba; bdesprba; bdefamsba; bdefaiba; bdetecba; bdeoekba;
bdequaba; bdearbba

qt: Einfachauswahl

hl:

in:

q: Warum haben Sie sich für Deutschland als Studienlang entschieden?

is: Bitte geben Sie den jeweils zutreffenden Skalenwert an.

it1 (bdefinba): weil dies meinen finanziellen Möglichkeiten entspricht.

it2 (bdekenba): um Deutschland kennenzulernen/weil mich die deutsche Geschichte
und Kultur interessiert.

it3 (bdesprba): um meine Sprachkenntnisse zu vertiefen.

it4 (bdefamsba): weil Freunde/Verwandte in Deutschland studieren/studiert haben.

it5 (bdefamlba): weil Freunde/Verwandte in Deutschland leben/gelebt haben.

it6 (ddetecba): weil Deutschland ein hochtechnisiertes Land ist.

it7 (bdeoekba): wegen der wirtschaftlichen Lage in Deutschland.

it8 (bdequaba): wegen der Lebensqualität in Deutschland.

it9 (bdearbba): auf der Möglichkeit, nach Studienabschluss in Deutschland zu
arbeiten.

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

tr:

GOTO F1_10

hi: Items bitte zufällig rotieren.

\--------------------------------

F1_10
=====

tc:

vn: ainfaba; ainfbmba; ainfbjba; ainfemba, ainfejba

qt: Tableau-Frage Drop-Down Menüs, offene Angabe

hl:

in:

q: Bitte beschreiben Sie Ihren aktuellen Aufenthalt in Deutschland näher.

is:

it:

st:

Drop-Down-Menü:

ao1 (ainfaba): 1: : Auslandsstudium mit angestrebtem Abschluss in Deutschland

ao2 (ainfaba): 2: : Auslandsstudium/-semester ohne angestrebten Abschluss in
Deutschland

ao3 (ainfaba): 3: : Praktikum/Praxisphase

ao4 (ainfaba): 4: : Sprachkurs

ao5 (ainfaba): 5: : Studienreise

ao6 (ainfaba): 6: : Projektarbeit

ao7 (ainfaba): 7: : Summerschool

ao8 (ainfaba): 8: : sonstiger Aufenthalt

Nebeneinander angeordnete Drop-Down-Menüs:

ao9 (ainfbmba): : Monat: (Januar \| … \| Dezember)

ao10 (ainfbjba): : Jahr: (2020 \| 2019 \| … \| 2000 \| vor 2000)

Nebeneinander angeordnete Drop-Down-Menüs:

ao11 (ainfemba): : Monat: (Januar \| … \| Dezember)

ao12 (ainfejba): Jahr: (2030 \| 2029 \| … \| 2000 \| vor 2000)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hl:

in:

q:

is:

it:

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

tr:

GOTO F1_11

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

ao1: 1: : Nein, ich werde in Deutschland nur einen Teil meines Studiums
absolvieren.

ao2: 2: : Ja, ich plane den Abschluss eines Studiums in Deutschland (z. B.
Bachelor, Master, Promotion)

ao3: 3: : Ja, ich plane einen Doppelabschluss in Deutschland un in meinem
Herkunftsland/einem anderen Land.

ao4: 4: : weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_12

hi:

\--------------------------------

F1_12
=====

tc: IF sabsabsba=1 AND sabsabsba=3

vn: ainfcpba; ainfcp1osba; ainfcp2osba

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Wissen Sie bereits, ob Ihr Aufenthalt in Deutschland auf Ihr Studium in Ihrem
Heimatland angerechnet wird, z. B. in Form ECTS-Punkten?

is:

it:

st:

ao1: 1: : nein

ao2: 2: : offene Angabe: 2 Stellen Präfix [ainfcp1osba], Suffix: ja, teilweise:
… ECTS-Punkte

ao3: 3: : offene Angabe: 2 Stellen Präfix [ainfcp2osba], Suffix: ja,
vollständig: … ECTS-Punkte

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_13

hi:

\--------------------------------

F1_13
=====

tc:

vn: aproselbba; aprokoopba; aproorigba; aprodaadba; aproerasba; aproeuba;
aprointerba; aproanprba

qt: Mehrfachnennung

hl:

in:

q: Findet Ihr aktueller Aufenthalt in Deutschland im Rahmen eines
Austauschprogramms statt?

is: Mehrfachnennungen sind möglich.

it:

st:

ao1 (aproselbba): : nein, ich habe den Aufenthalt selbst organisiert
(Exklusivkategorie)

ao2 (aprokoopba): : ja, Kooperationsprogramm zwischen Heimathochschule und
deutscher Hochschule

ao3 (aproorigba): : ja, Programm meines Herkunftslandes

ao4 (aprodaadba): : ja, deutsches Programm (z. B. DAAD-Programm)

ao5 (aproerasba): : ja, ERASSMUS+/ERASMUS-Programm

ao6 (aproeuba): : ja, anderes EU-Programm

ao7 (aprointerba): : ja, Programm einer internationalen Organisation

ao8 (aproanprba): : ja, anderes Programm offene Angabe: 100 Stellen, Präfix
[aproanproba], Suffix:und zwar:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_14

hi:

\--------------------------------

F1_14
=====

tc:

vn: akontdeutstba; akonteinheimba; akontheimba; akontintstba

qt: Einfachauswahl

hl:

in:

q: Wie häufig haben Sie während Ihres Aufenthalts in Deutschland ingesamt
Gespräche/Kontakt…

is:

it1 (akontdeutstba): … mit Studierenden aus Deutschland?

it2 (akonteinheimba): … mit anderen Einheimischen?

it3 (akontheimba): … mit Studierenden aus Ihrem Heimatland?

it4 (akontintstba): … mit anderen internationalen Studierenden (nicht aus Ihrem
Heimatland)?

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

tr:

GOTO F1_15

hi:

\--------------------------------

F1_15
=====

tc:

vn: azufrwillba;azufrsichba

qt: Einfachauswahl

hl:

in:

q1: Wie willkommen fühlen Sie sich in Deutschland?

q2: Wie sicher fühlen Sie sich bisland in Deutschland insgesamt?

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

tr:

GOTO F1\_

hi: 16

\--------------------------------

F1_16
=====

tc:

vn: azufskein; azufskstu; azufsklehr; azuflernerf; azufinsg

qt: Einfachauswahl, Akkordeon

hl:

in:

q: Wie zufrieden sind Sie bis zum jetzigen Zeitpunkt mit …

is:

it1 (azufskein): … dem sozialen Kontakt zu Einheimischen?

it2 (azufskstu): … dem sozialen Kontakt zu Studierenden?

it3 (azufsklehr): … dem sozialen Kontakt zu Lehrenden?

it4 (azuflernerf): … den gewonnenen fachlichen Kenntnissen?

it5 (azufinsg): … Ihrem Aufenthalt in Deutschland insgesamt?

st:

ao1: 1: : überhaupt nicht zufriden

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

tr:

GOTO F1_17

hi:

\--------------------------------

F1_17
=====

tc:

vn: azufleistanf; azuforgaufw; azuffinanzaufw

qt: Einfachauswahl, Akkordeon

hl:

in:

q: Und wie beurteilen Sie …

is:

it1 (azufleistanf): … die aktuellen Leistungsanforderungen?

it2 (azuforgaaufw): … den aktuellen organisatorischen Aufwand?

it3 (azuffinanzaufw): … den aktuellen finanziellen Aufwand?

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

tr:

GOTO F1_18

hi:

\--------------------------------

F1_18
=====

tc:

vn: adeempfba

qt: Einfachauswahl

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen mit den Studien- und
Lebensbedingungen in Deutschland: Würden Sie Ihren Freunden/Bekannten empfehlen,
ein Studium in Deutschland durchzuführen?

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

tr:

GOTO F1_19

hi:

\--------------------------------

F1_19
=====

tc:

vn: bdedarlba; bdedarloba; bdedarhssia; bdedarhsoba

qt: Einfachauswahl, offene Angabe

hl:

in:

q: Hinsichtlich Ihres Auslandsaufenthalts: Wenn Sie die freie Wahl gehabt
hätten, in welchem Land und an welchem Ort hätten Sie am liebsten studiert?

is:

it1 (bdedarlba): Land: (offene Angabe: 100 Zeichen, Präfix [bdedarloba], Suffix
…

i t1 (bdedarhssia): Stadt/Hochschule: (offene Angabe: 100 Zeichen, Präfix
[bdedarhsoba], Suffix …

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

tr:

GOTO F1_20

hi:

\--------------------------------

F1_20
=====

tc:

vn: bhiitecba; bhiiwelba; bhiivorbba; bhiitutba; bhiiheimba; bhiivermba;
bhiideuba; bhiiberba; bhiibehba; bhiikulba; bhiikomba; bhiifinba; bhiiaerlba;
bhiivisba; bhiikvba; bhiipsyba; bhiikeinba

qt: Einfachauswahl

hl:

in:

q: Welche der Hilfestellungen für Studierende haben Sie bisher genutzt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (bdedarhsoba): : Einführung in wissenschaftliche Lern- und Arbeitstechniken

ao2 (bhiiwelba): : Welcome-Veranstaltungen/Begrüßungsveranstaltung

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

ao16 (bhiipsyba): : psychologische Beratung bei persönlichen oder
studienbezogenen Schwierigkeiten

Lehrzeile

ao17 (bhiikeinba): : kein Angebot genutzt (Exklusivkategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_21

hi:

\--------------------------------

F1_21
=====

tc:

vn: bdebleibba

qt: Einfachauswahl

hl:

in:

q: Was planen Sie direct im Anschluss an Ihr Studium in Deutschland?

is:

it:

st:

Ich möchte Arbeiten, und zwar …

ao1: … in Deutschland

ao2: … in meinem Heimatland

ao3: … in einem anderen Land

Ich möchte weiterstudieren, und zwar …

ao4: … in Deutschland

ao5: … in meinem Heimatland

ao6: … in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_22

hi:

\--------------------------------

F1_22
=====

tc:

vn: intpsyherkba; intpsyzeitdeu; intpsyanddeu

qt: Einfachauswahl

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

tr:

GOTO F1_23

hi:

\--------------------------------

F1_23
=====

tc:

vn: intling1ba; intling2ba; intling3ba

qt: Einfachauswahl

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie zu?

is:

it1 (intling1ba): Ich kann auf Deutsch über vertraute Themen sprechen und
persönliche Meinungen äußern.

it2 (intling2ba): Ich verstehen die wichtigsten Punkte in Radio- und
Fernsehprogrammen, die auf Deutsch gesendet warden.

it3 (intling3ba): Ich kann deutsche Zeitungsartikel lesen und vollständig
verstehen.

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

tr:

GOTO F1_24

hi:

\--------------------------------

F1_24
=====

tc:

vn: aarbchdeuba; aarbchherkba; aarbchandlba

qt: Einfachauswahl

hl:

in:

q: Wie schätzen Sie Ihre derzeitigen Berufs- und Arbeitsmarktchancen ein?

is:

it1 (aarbchdeuba): in Deutschland?

it2 (aarbchherkba): in Ihrem Herkunftsland?

it3 (aarbchandlba): in einem anderen Land?

st:

ao1: 1: :überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr gut

ao6: 6: : kann ich nicht beurteilen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO nächstes Modul

hi:
