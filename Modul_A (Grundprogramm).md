\------------------------------------------------------------

index
=========

tc:

vn: sidpretest_consent

qt: Mehrfachauswahl

hl: 

in:

q: 
Vorstudie „die Studierendenbefragung in Deutschland“
(Leerzeile)

Herzlich willkommen bei **Die Studierendenbefragung in Deutschland**
(Leerzeile)

Wir freuen uns, dass Sie uns mit Ihrer Teilnahme bei der Konzeption der größten Studierendenbefragung in Deutschland unterstützen. 
(Leerzeile)

Ziel der Studie ist es, ein umfassendes Bild von der Gesamtsituation aller Studierenden in Deutschland zu erhalten. Daher umfasst die Befragung ein breites Themenspektrum, das von Fragen zu Ihrer individuellen Bildungsbiographie, den Rahmenbedingungen und Herausforderungen im Studium bis hin zu Ihren Karriereaussichten und gesellschaftlichen Wertvorstellungen reicht. Unser Anspruch ist es, detailliert auf Ihre individuelle Lebenslage einzugehen: Vor welchen besonderen Herausforderungen standen Sie im Laufe Ihres Studiums? Welche Rahmenbedingungen sind Ihrer Einschätzung nach notwendig, damit auch Studierende mit Kind oder körperlichen Beeinträchtigung erfolgreich ein Studium absolvieren zu können? Welche Wege führen ins Ausland und welche Wege führen ausländische Studierende an eine deutsche Hochschule? Diese und viele weitere Fragen sind leitend für unsere Studie.
(Leerzeile)

Die gewonnenen Daten stellen eine wesentliche Grundlage der Bildungsberichterstattung in Deutschland dar und fließen regelmäßig in die bildungspolitische Diskussion ein. Über Ihre Teilnahme tragen Sie daher aktiv zu einer Bildungs‐ und Hochschulpolitik bei, die sich an der Lebenswirklichkeit und den Bedarfen der Studierenden von heute orientiert.
(Leerzeile)

Aktuell sind wir dabei das Befragungsinstrument zu entwickeln und benötigen im Rahmen dieser Vorstudie von Ihnen erste Hinweise, welche Fragen in welcher Form die Lebenswirklichkeit der Studierenden am besten abbilden.
(Leerzeile)

Die Beantwortung des Fragebogens nimmt ca. 30-40 Minuten in Anspruch. Sie können die Befragung jederzeit pausieren und sich zu einem späteren Zeitpunkt erneut mit Ihrem Passwort einloggen. Die komfortabelste Befragungssituation erhalten Sie, wenn Sie die Befragung an einem PC oder Laptop durchführen.
(Leerzeile)

Um ein möglichst genaues Bild zu erhalten, bitten wir Sie, möglichst alle Fragen zu beantworten. Sollten einzelne Frage nicht passen, gehen Sie bitte zur nächsten Frage weiter. Selbstverständlich ist Ihre Teilnahme freiwillig. Alle Angaben werden vertraulich behandelt und nur für wissenschaftliche Zwecke genutzt.
(Leerzeile)

Weiterführende Informationen finden Sie unter www.die-studierendenbefragung.de.
(Leerzeile)

Für weitere Fragen wenden Sie sich bitte an uns: 
(Leerzeile)
(Leerzeile)

Dr. Markus Lörz #{layout.MAIL_START}loerz@dzhw.eu#{layout.MAIL_END}loerz@dzhw.eu#{layout.MAIL_STOP}
(Leerzeile)

Heike Naumann #{layout.MAIL_START}naumann@dzhw.eu#{layout.MAIL_END}naumann@dzhw.eu#{layout.MAIL_STOP}
(Leerzeile)

Weitere Informationen zum Datenschutz finden Sie #{layout.hyperlink('./SID_Informed_Consent.pdf','hier','_blank')}.

Bei **Fragen zum Datenschutz** wenden Sie sich bitte an den Datenschutzbeauftragten des DZHW, Herrn Martin Fuchs: Tel.: +49 511 450670-491; E-Mail: #{layout.MAIL_START}fuchs@dzhw.eu#{layout.MAIL_END}fuchs@dzhw.eu#{layout.MAIL_STOP}. Weitere Informationen zum Datenschutz am DZHW finden Sie hier: #{layout.hyperlink('https://www.dzhw.eu/datenschutz','https://www.dzhw.eu/datenschutz','_blank')}


is:

it:

st:

ao1: (sidpretest_consent): Ich habe die Datenschutzbestimmungen gelesen und bin damit einverstanden. Meine Teilnahme an der Befragung ist freiwillig. Diese Einwilligung bezieht sich ausdrücklich auch auf die Angaben zur gesundheitlichen Beeinträchtigung.

mv:

ka:

vc:
SHOW kh1 IF sidpretest_consent!=1

av:

kh1: Bitte beachten Sie, dass ohne Zustimmung zu den Datenschutzbestimmungen eine Teilnahme an der Vorstudie von 
						#{layout.BOLD_START}“Die Studierendenbefragung in Deutschland“#{layout.BOLD_END} leider nicht möglich ist.

fv:

hv:
mastersplit = 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14 (einmalige Randomisierung; mit gleicher Ziehungswahrscheinlichkeit)

zusatzsplit = 1, 2, 3, 4 (einmalige Randomisierung; mit gleicher Ziehungswahrscheinlichkeit)

fo:

tr: 
GOTO index IF !sidpretest_consent.value and !sf_h.value
GOTO offer IF sidpretest_consent.value and jsCheck.value and isMobile.value and width.value lt 768
GOTO A_1 IF sidpretest_consent.value


hi:


\------------------------------------------------------------

offer
=========

tc:

vn:

qt:

hl:

in:

q: Um ein optimales Befragungserlebnis zu erhalten, sollten Sie für die Beantwortung einiger Fragen das Display drehen.

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

tr: A_1

hi:


\------------------------------------------------------------

A_1
=========

tc:

vn: vsbdeba

qt: Einfachauswahl

hl:

in: Um die Befragung passend für Ihre Situation gestalten zu können und insbesondere auf die Situation internationaler Studierender eingehen zu können, müssen wir Ihnen zu Beginn zwei zentrale Eingangsfragen stellen.

q: Wo haben Sie erstmals Ihre Hochschulreife erworben?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte lediglich die Frage ("Wo haben Sie erstmals Ihre Hochschulreife erworben?") fetten und etwas vom Einleitungstext absetzen. Der Einleitungstext sollte nicht fett sein.

tr:

hi: 

\------------------------------------------------------------

A_1
=========

tc:

vn: dnatdeu, dnatausl

qt: Mehrfachauswahl

hl:

in:

q: Und: Welche Staatsangehörigkeit haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dnatdeu): 1: deutsche Staatsangehörigkeit

ao2: (dnatausl): 2: andere Staatsangehörigkeit(en)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_2 IF dnatdeu==1
    GOTO A_3 IF dnatdeu=0 AND dnatausl=1
    GOTO A_5 IF !dnatdeu.value and !dnatausl.value

hi:


\------------------------------------------------------------

A_2
====

tc:

vn: dnatderw

qt: Einfachauswahl

hl:

in:

q: Besitzen Sie die deutsche Staatsangehörigkeit …

is:

it:

st:

ao1: 1: ... von Geburt an?

ao2: 2: ... als Spätaussiedler\*in?

ao3: 3: ... durch Einbürgerung?

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 
<zofar:transition target="A_3" condition="dnatausl.value or (dnatdeu.value and (zofar.asNumber(dnatderw)==2 or zofar.asNumber(dnatderw)==3))"/>
<zofar:transition target="A_3" condition="dnatausl.value and zofar.asNumber(dnatderw)==1"/>
<zofar:transition target="A_3" condition="dnatausl.value and zofar.isMissing(dnatderw)"/>
<zofar:transition target="A_5" condition="dnatdeu.value and zofar.asNumber(dnatderw)==1"/>
<zofar:transition target="A_5" condition="dnatdeu.value and zofar.isMissing(dnatderw)"/>

hi:

\------------------------------------------------------------

A_3
====

tc:

vn: dnatko

qt: Einfachauswahl

hl:

in:

q1: Welche Staatsangehörigkeit besaßen Sie bevor Sie nach Deutschland kamen?

q2: Welche Staatsangehörigkeit besaßen Sie vor Ihrer Einbürgerung?

q3: Sie haben zu Beginn der Befragung angegeben, die deutsche und eine ausländische Staatsangehörigkeit zu haben. Welche Staatsangehörigkeit besitzen Sie neben der deutschen?

q4: Sie haben zu Beginn der Befragung angegeben, eine ausländische Staatsangehörigkeit zu haben. Welche ausländische Staatsangehörigkeit besitzen Sie?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc:

SHOW q1 if dnatderw=2 AND dnatausl=0

SHOW q2 if dnatderw=3 AND dnatausl=0

SHOW q3 if dnatdeu=1 AND dnatausl=1

SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: GOTO A_4

hi:

\------------------------------------------------------------

A_4
====

tc:

vn: dnatsta

qt: Einfachauswahl mit Dropdown

hl:

in:

q1: Bitte geben Sie nun die Staatsangehörigkeit an, die Sie hatten, bevor Sie nach Deutschland kamen.

q2: Bitte geben Sie nun Ihre Staatsangehörigkeit vor Ihrer Einbürgerung an.

q3: Bitte geben Sie nun Ihre Staatsangehörigkeit an, die Sie neben der deutschen besitzen.

q4: Bitte geben Sie nun Ihre ausländische Staatsangehörigkeit an.

is:

it:

st:

ao: (dnatsta): [infield = Staatsangehörigkeit; Staatenliste_DBI] (Dropdown)

mv:

ka:

vc: SHOW Dropdown if dnatko\>0

SHOW q1 if dnatderw=2 and dnatausl=0

SHOW q2 if dnatderw=3 and dnatausl=0

SHOW q3 if dnatdeu=1 AND dnatausl=1

SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: 

hi: Dropdown bitte nach Angabe des Kontinents in A_3 (dnatko) vorselektieren.

\------------------------------------------------------------

A_4
====

tc:

vn: dnatstao

qt: offene Angabe

hl:

in:

q: An dieser Stelle können Sie Ihre Staatsangehörigkeit auch offen angeben: 

is:

it:

st:

ao: (dnatstao): [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_5

hi:

\------------------------------------------------------------

A_5
====

tc:

vn: dgebort

qt: Einfachauswahl

hl:

in:

q: Wo wurden Sie geboren?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_6 if dgebort=2
    GOTO A_9a if (dgebort=1 OR dgebort=MISSING) AND h_split=1 (50%)
    GOTO A_9b if (dgebort=1 OR dgebort=MISSING) AND h_split=2 (50%)

hi:

\------------------------------------------------------------

A_6
====

tc:

vn: dgebko

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurden Sie geboren?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: A_7

hi:

\------------------------------------------------------------

A_7
====

tc:

vn: dgebsta

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie nun das Land an, in dem Sie geboren wurden.

is:

it:

st:

ao: (dgebsta): [infield = Geburtsland; Staatenliste_DBI] (Dropdown)

mv:

ka:

vc: SHOW Dropdown if (dgebko != MISSING AND dgebko != 0)

av:

kh:

fv:

hv:

fo:

tr: 

hi: Dropdown bitte nach Angabe des Kontinents in A_6 (dgebko) vorselektieren.

\------------------------------------------------------------

A_7
====

tc:

vn: dgebstao

qt: offene Frage

hl:

in:

q: An dieser Stelle können Sie Ihr Geburtsland auch offen angeben:

is:

it:

st:

ao: (dgebstao): [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C3_1

hi:

\------------------------------------------------------------

A_8
===

tc:

vn: baufgru (baufgrueuba; baufgrustuba; baufgruerwerb; baufgrutouba; baufgruasylba; baufgrufaman; baufgrufamba; baufgruausba; baufgruandba; baufgruandba_open)

qt: Mehrfachauswahl mit offener Angabe

hl:

in:

q: Für die Einreise nach Deutschland gibt es unterschiedliche rechtliche Grundlagen. Wie war das bei Ihnen?

Als ich nach Deutschland kam, war ich:

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (baufgrueuba): 1: Bürger\*in eines EU Mitgliedstaates bzw. des europäischen Wirtschaftsraums

ao2: (baufgrustuba): 2: Studierende\*r (auch zur Studienvorbereitung)

ao3: (baufgruerwerb): 3: Erwerbstätige\*r (Arbeitsvisum)

ao4: (baufgrutouba): 4: Tourist\*in (Besuchsvisum)

ao5: (baufgruasylba): 5: Asylbewerber\*in, Geflüchtete\*r oder Schutzsuchende\*r

ao6: (baufgrufaman): 6: Familienangehörige\*r, kam mit Eltern bzw. Ehepartner\*in

ao6: (baufgrufamba): 7: Familiennachzug, zog zu bereits in Deutschland lebender Familie

ao6: (baufgruausba): 8: (Spät-)Aussiedler\*in

ao7: (baufgruandba): 7: Anderer Status, und zwar: (baufgruandba_open) [offene Eingabe, 80 Zeichen]

ato:

mv:

ka:

vc:

av:

kh:

fv:

hv: 

fo: "Als ich nach Deutschland kam, war ich:" bitte etwas von den Einleitungssätzen absetzen.

tr: 
GOTO A_8a IF baufgruasylba=1
GOTO A_8b IF baufgruasylba=0 AND (baufgrufaman=1 OR baufgrufamba=1)
GOTO A_9a IF (baufgruasylba=0 AND baufgrufaman=0 AND baufgrufamba=0) AND h_split=1
GOTO A_9b IF (baufgruasylba=0 AND baufgrufaman=0 AND baufgrufamba=0) AND h_split=2

hi:


\------------------------------------------------------------

A_8a
=========

tc:

vn: asylantrag

qt: Einfachauswahl 

hl:

in:

q: Wie wurde über Ihren Asylantrag entschieden?

is:

it:

st:

ao1: 1: Das Asylverfahren ist noch nicht abgeschlossen.

ao2: 2: Ich wurde als Geflüchtete\*r oder Asylberechtigte\*r anerkannt.

ao3: 3: Ich habe einen subsidiären Schutzstatus bekommen.

ao4: 4: Der Asylantrag wurde abgelehnt und ich habe eine Duldung bekommen.

ao5: 5: Ich möchte keine Angabe machen.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_8b IF (baufgrufaman=1 OR baufgrufamba=1)
    GOTO A_9a IF (baufgrufaman=0 AND baufgrufamba=0) AND h_split=1
    GOTO A_9b IF (baufgrufaman=0 AND baufgrufamba=0) AND h_split=2

hi:


\------------------------------------------------------------

A_8b
=========

tc:

vn: intgrundhl intgrunddl

qt: offene Angaben

hl:

in:

q: Was waren die Gründe dafür, dass Sie oder Ihre Familie...

is:

it1: (intgrundhl): Präfix: ... Ihr Herkunftsland verlassen haben? [offene Angabe; 250 Zeichen]

it2: (intgrunddl): Präfix: ... nach Deutschland gezogen sind? [offene Angabe; 250 Zeichen]

st:

ao:

vc:

av:

kh:

fv:

hv:

fo: Die beiden Items bitte linksbündig untereinander setzen.

tr: GO TO A_9b

hi:


\------------------------------------------------------------

A_9b
=========

tc:

vn: demosex; demosexo

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Welches Geschlecht haben Sie?

is:

it:

st:

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: divers

ao4: 4: Keine der genannten Kategorien, sondern: [(demosexo); 80 Zeichen] (offene Angabe)

vc:

av:

kh:

fv:

hv:

fo: ao4 bitte etwas absetzen.

tr: GOTO A_10

hi:


\------------------------------------------------------------

A_10
=========

tc:

vn: demoage

qt: offene Frage

hl:

in:

q: Wie alt sind Sie?

is:

it:

st:

ao: Postfix: Jahre [offene Angabe; NUMBER 2-stellig]

mv:

ka:

vc:

av: NUMBER: 2-stellig: 16 TO 99

kh: Bitte geben Sie Ihr Lebensalter an (16 bis 99).

fv:

hv:

fo:

tr: GOTO A_11

hi: Bitte als 2-stellige NUMBER, 16 bis 99, programmieren.

\------------------------------------------------------------

A_11
=========

tc:

vn: demofam (demofamsin; demofampar; demofamehe; demofamaus; demofamtod; demofamka)

qt: Mehrfachauswahl

hl:

in:

q: Welchen Familienstand haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (demofamsin): ohne feste(n) Partner\*in

ao2: (demofampar): mit einer/einem festen Partner\*in

ao3: (demofamehe): verheiratet/eingetragene Lebenspartnerschaft

ao4: (demofamaus): geschieden
	
ao5: (demofamtod): verwitwet

ao6: (demofamka): keine Angabe [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: ao6 bitte als Exklusivkategorie etwas absetzen.

tr: GOTO A_12

hi:

\------------------------------------------------------------

A_12
=========

tc:

vn: dkinja

qt: Einfachauswahl

hl:

in:

q: Haben Sie Kinder?

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

tr: GOTO A_13 if dkinja=1
    GOTO C1_1 if dkinja=2
    GOTO A_13 if dkinja=MISSING

hi:

\--------------------------------

A_13
==

tc:

vn: pflegeang (pflegangno; pflegang1; pflegang2)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Pflegen Sie regelmäßig pflegebedürftige Verwandte oder Freunde?

is: Nicht gemeint ist die Betreuung der eigenen Kinder.

it:

st:

ao1: (pflegangno): nein [Exklusivkategorie]

ao2: (pflegang1): aus der Familie

ao3: (pflegang2): aus dem Freundes- und Bekanntenkreis

mv:

ka: (ao2 TO ao3): ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: "ja, und zwar:" zwischen ao1 und ao2 setzen.

tr:

GOTO A_14 IF pflegang1=1 OR pflegang2=1 
ELSE A_15

hi:

\--------------------------------

A_14
==

tc: IF pflegang1=1 OR pflegang2=1

vn: pflegt (pflegt1; pflegt2; pflegt3; pflegt4; pflegt5; pflegt5o)

qt: Einfachauswahlmatrix mit horizontalen ao, offene Angabe

hl:

in:

q: Wenn Sie an eine typische Woche denken: Wie häufig führen Sie folgende Pflegetätigkeiten aus?

is:

it1: (pflegt1): Besorgungen und Erledigungen außer Haus, z. B. Behördengänge

it2: (pflegt2): Haushaltsführung, Versorgung mit Mahlzeiten und Getränken

it3: (pflegt3): einfachere Pflegetätigkeiten, z. B. Hilfe beim An- und Auskleiden,
Waschen, Kämmen und Rasieren

it4: (pflegt4): schwierigere Pflegetätigkeiten, z. B. Hilfe beim Umbetten,
Stuhlgang

it5: (pflegt4): Etwas anderes, und zwar: [(pflegt5o); 80 Zeichen] (offene Angabe)

st:

ao0: 0: nie

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

fo: Bitte die Spalte "nie" etwas von der Skala "sehr selten" bis "sehr häufig" absetzen.

tr: GOTO A_15

hi:

\------------------------------------------------------------

A_15
=========

tc:

vn: gbeges; gartmob; gartseh; gartohr; gartspr; gartpsy; gartsom; garttls; gartson; gartka; h_gartcount

qt: Mehrfachauswahl

hl:

in: Im Folgenden stellen wir Ihnen einige kurze Fragen zu möglichen Beeinträchtigungen. Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu.

q: Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (gbeges): 1: keine [Exklusivkategorie]

ao2: (gartmob): 2: Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

ao3: (gartseh): 3: Blindheit/Sehbeeinträchtigung

ao4: (gartohr): 4: Gehörlosigkeit/Hörbeeinträchtigung

ao5: (gartspr): 5: Sprechbeeinträchtigung (z. B. Stottern)

ao6: (gartpsy): 6: psychische Erkrankung (z. B. Depression, Essstörung)

ao7: (gartsom): 7: körperlich länger dauernde/chronische Krankheit (z. B. Rheuma, MS, Darmerkrankung)

ao8: (garttls): 8: Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

ao9: (gartson): 9: andere Beeinträchtigung/Erkrankung (z. B. Tumorerkrankung, Autismus-Spektrum-Störung) [gartsono], 50 Zeichen

ao10: (gartka): 10: Ich möchte die Form meiner Beeinträchtigung nicht nennen. 

mv:

ka: (ao2 TO ao10): Ja, und zwar:

vc:

av:

kh:

fv:

hv: 

fo1: Bitte lediglich die Frage ("Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?") fetten und etwas vom Einleitungstext absetzen. Der Einleitungstext sollte nicht fett sein.

fo2: Bitte über ao2 "Ja, und zwar:" positionieren.

fo3: ao10 bitte etwas absetzen.

tr: GOTO A_16 if gbeges=1
    GOTO C2_1 if gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1
    GOTO A_16 if gbeges=MISSING AND gartmob=MISSING AND gartseh=MISSING AND gartohr=MISSING AND gartspr=MISSING AND gartpsy=MISSING AND gartsom=MISSING AND garttls=MISSING AND gartson=MISSING AND gartka=MISSING
    
hi:

\------------------------------------------------------------

A_16
=========

tc:

vn: imausl

qt: Einfachauswahl

hl:

in:

q: Befinden Sie sich zurzeit studienbezogen außerhalb Deutschlands?

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

tr: GOTO A_17

hi:

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemfs

qt: offene Frage

hl:

in:

q: Im wievielten Fachsemester befinden Sie sich zurzeit?

is1: Fachsemester sind die Semester, die Sie in Ihrem derzeitigen Studiengang eingeschrieben sind.

it:

st:

ao: Präfix: Fachsemester: [offene Angabe; NUMBER 2-stellig; 1 bis 99]

mv:

ka:

vc: 

av: NUMBER, 2-stellig (1 bis 99)

kh: Bitte geben Sie die Anzahl Ihrer Fachsemester als Zahl an.

fv:

hv:

fo:

tr: 

hi: Bitte als NUMBER, 2-stellig (1 bis 99), programmieren.

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemhs

qt: offene Frage

hl:

in:

q: Im wievielten Hochschulsemester befinden Sie sich zurzeit?

is: Hochschulsemester sind alle Semester seit Beginn des Studiums, einschließlich Urlaubs-, Auslands- und Praxissemester.

it:

st:

ao: Präfix: Hochschulsemester: [offene Angabe; NUMBER 2-stellig; 1 bis 99]

mv:

ka:

vc:

av: NUMBER, 2-stellig (1 bis 99)

kh: Bitte geben Sie die Anzahl Ihrer Hochschulsemester als Zahl an.

fv:

hv:

fo:

tr:

hi: Bitte als NUMBER, 2-stellig (1 bis 99), programmieren.

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemul

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Befinden Sie sich aktuell in einem Urlaubssemester?

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

tr: <zofar:transition target="A_19" condition="zofar.asNumber(PRELOADhs_id)==0"/>
    <zofar:transition target="A_18"/>

hi:

\------------------------------------------------------------

A_18
=======

tc:

vn: hsstand

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Wir haben Sie über die [Preload-Token: Hochschulname] angeschrieben. Ist das die Hochschule, an der Sie aktuell studieren??

is: Falls Sie aktuell an einer anderen Hochschule studieren, wählen Sie bitte “Nein” aus.
Falls Sie an mehreren Hochschulen parallel studieren, beziehen Sie Ihre Antworten bitte auf die oben genannte Hochschule. 

it1 (hsstand): Ja, und zwar am Standort [Dropdown; Standortliste].

it2 (hsstand_2): Nein, ich studiere an einer anderen Hochschule.

st:

ao:

mv:

ka:

vc: 
SHOW ao1 AND [Dropdown] IF 
zofar.asNumber(PRELOADhs_id)==10 or zofar.asNumber(PRELOADhs_id)==30 or zofar.asNumber(PRELOADhs_id)==100 or zofar.asNumber(PRELOADhs_id)==300 or zofar.asNumber(PRELOADhs_id)==370 or zofar.asNumber(PRELOADhs_id)==550 or zofar.asNumber(PRELOADhs_id)==760 or zofar.asNumber(PRELOADhs_id)==810 or zofar.asNumber(PRELOADhs_id)==820 or zofar.asNumber(PRELOADhs_id)==1190 or zofar.asNumber(PRELOADhs_id)==1220 or zofar.asNumber(PRELOADhs_id)==1250 or zofar.asNumber(PRELOADhs_id)==1290 or zofar.asNumber(PRELOADhs_id)==1310 or zofar.asNumber(PRELOADhs_id)==1320 or zofar.asNumber(PRELOADhs_id)==1540 or zofar.asNumber(PRELOADhs_id)==1560 or zofar.asNumber(PRELOADhs_id)==1630 or zofar.asNumber(PRELOADhs_id)==1920 or zofar.asNumber(PRELOADhs_id)==2210 or zofar.asNumber(PRELOADhs_id)==2270 or zofar.asNumber(PRELOADhs_id)==2370 or zofar.asNumber(PRELOADhs_id)==2380 or zofar.asNumber(PRELOADhs_id)==2570 or zofar.asNumber(PRELOADhs_id)==2580 or zofar.asNumber(PRELOADhs_id)==3050 or zofar.asNumber(PRELOADhs_id)==3060 or zofar.asNumber(PRELOADhs_id)==3070 or zofar.asNumber(PRELOADhs_id)==3120 or zofar.asNumber(PRELOADhs_id)==3240 or zofar.asNumber(PRELOADhs_id)==3710 or zofar.asNumber(PRELOADhs_id)==3970 or zofar.asNumber(PRELOADhs_id)==4980 or zofar.asNumber(PRELOADhs_id)==4990 or zofar.asNumber(PRELOADhs_id)==5150 or zofar.asNumber(PRELOADhs_id)==5160 or zofar.asNumber(PRELOADhs_id)==5250 or zofar.asNumber(PRELOADhs_id)==5270 or zofar.asNumber(PRELOADhs_id)==5310 or zofar.asNumber(PRELOADhs_id)==5380 or zofar.asNumber(PRELOADhs_id)==5390 or zofar.asNumber(PRELOADhs_id)==5410 or zofar.asNumber(PRELOADhs_id)==5500 or zofar.asNumber(PRELOADhs_id)==5690 or zofar.asNumber(PRELOADhs_id)==5700 or zofar.asNumber(PRELOADhs_id)==5710 or zofar.asNumber(PRELOADhs_id)==5720 or zofar.asNumber(PRELOADhs_id)==5730 or zofar.asNumber(PRELOADhs_id)==5750 or zofar.asNumber(PRELOADhs_id)==5800 or zofar.asNumber(PRELOADhs_id)==5820 or zofar.asNumber(PRELOADhs_id)==5830 or zofar.asNumber(PRELOADhs_id)==5840 or zofar.asNumber(PRELOADhs_id)==5860 or zofar.asNumber(PRELOADhs_id)==5890 or zofar.asNumber(PRELOADhs_id)==5900 or zofar.asNumber(PRELOADhs_id)==5990 or zofar.asNumber(PRELOADhs_id)==6030 or zofar.asNumber(PRELOADhs_id)==6210 or zofar.asNumber(PRELOADhs_id)==6230 or zofar.asNumber(PRELOADhs_id)==6240 or zofar.asNumber(PRELOADhs_id)==6270 or zofar.asNumber(PRELOADhs_id)==6280 or zofar.asNumber(PRELOADhs_id)==6400 or zofar.asNumber(PRELOADhs_id)==6410 or zofar.asNumber(PRELOADhs_id)==6520 or zofar.asNumber(PRELOADhs_id)==6530 or zofar.asNumber(PRELOADhs_id)==6580 or zofar.asNumber(PRELOADhs_id)==6710 or zofar.asNumber(PRELOADhs_id)==6730 or zofar.asNumber(PRELOADhs_id)==6740 or zofar.asNumber(PRELOADhs_id)==6750 or zofar.asNumber(PRELOADhs_id)==6790 or zofar.asNumber(PRELOADhs_id)==6840 or zofar.asNumber(PRELOADhs_id)==7190 or zofar.asNumber(PRELOADhs_id)==7300 or zofar.asNumber(PRELOADhs_id)==7310 or zofar.asNumber(PRELOADhs_id)==7350 or zofar.asNumber(PRELOADhs_id)==7380 or zofar.asNumber(PRELOADhs_id)==7520 or zofar.asNumber(PRELOADhs_id)==7530 or zofar.asNumber(PRELOADhs_id)==7550 or zofar.asNumber(PRELOADhs_id)==7970 or zofar.asNumber(PRELOADhs_id)==8010 or zofar.asNumber(PRELOADhs_id)==8020 or zofar.asNumber(PRELOADhs_id)==8030 or zofar.asNumber(PRELOADhs_id)==8070 or zofar.asNumber(PRELOADhs_id)==81000 or zofar.asNumber(PRELOADhs_id)==8110 or zofar.asNumber(PRELOADhs_id)==81700

av:

kh:

fv:

hv:

fo:

tr: 
GOTO D2_1 IF hsstand_2=0 AND (mastersplit=1 OR mastersplit=2 OR mastersplit=5 OR mastersplit=6 OR mastersplit=7 OR mastersplit=8 OR mastersplit=11 OR mastersplit=12 OR mastersplit=14)
GOTO A_22 IF hsstand_2=0 AND (mastersplit=3 OR mastersplit=4 OR mastersplit=9 OR mastersplit=10 OR mastersplit=13)
GOTO A_19 IF hsstand_2=1

hi:

\------------------------------------------------------------

A_19
=======

tc: IF hsstand_2=1

vn: hsstandbl

qt: Einfachauswahl mit Dropdown

hl:

in: 

q: In welchem Bundesland/Land liegt Ihre Hochschule?

is: 

it: (hsstandbl): [infield = Bundesland/Land; Baden-Württemberg - ... - im Ausland] (Dropdown)

st:

ao1: 1: Baden-Württemberg

ao2: 2: Bayern

ao3: 3: Berlin

ao4: 4: Brandenburg

ao5: 5: Bremen

ao6: 6: Hamburg

ao7: 7: Hessen

ao8: 8: Mecklenburg-Vorpommern

ao9: 9: Niedersachsen

ao10: 10: Nordrhein-Westfalen

ao11: 11: Rheinland-Pfalz

ao12: 12: Saarland

ao13: 13: Sachsen

ao14: 14: Sachsen-Anhalt

ao15: 15: Schleswig-Holstein

ao16: 16: Thüringen

ao17: 17: im Ausland

mv: 

ka: 

vc: 

av: 

kh: 

fv: 

hv: 

fo: 

tr: 
GOTO A_20 if hsstandbl=1-16
GOTO A_21 if hsstandbl=17

hi: 


\------------------------------------------------------------

A_20
=======

tc:

vn: sabserhs

qt: Einfachauswahl mit Dropdown

hl:

in: 

q: An welcher Hochschule studieren Sie aktuell?

is: 

it: (sabserhs): [infield = Hochschule] (Dropdown) 

st:

ao: nach Bundesland vorselektierte Dropdown-Liste

mv: 

ka: 

vc: 

av: 

kh: 

fv: 

hv: 

fo: 

tr:

hi: Dropdown-Hochschulliste bitte nach Bundesland vorselektieren.


\------------------------------------------------------------

A_20
=======

tc: 

vn: hsstandhso

qt: Offene Angabe

hl:

in: 

q: Sollte Ihre Hochschule nicht aufgeführt sein, tragen Sie diese bitte hier ein (z. B. HU Berlin, FH Bielefeld).

it: 

st:

ao: (hsstandhso): Präfix: Hochschule: [offene Angabe; 60 Zeichen]

mv: 

ka: 

av: 

kh: 

fv: 

hv: 

fo: 

tr: GOTO D2_1 if mastersplit=1, 2, 5, 6, 7, 8, 11, 12, 14
    GOTO A_22 if mastersplit=3, 4, 9, 10, 13

hi: 


\------------------------------------------------------------

A_21
=======

tc: IF hsstandbl=17 (wenn Studierende an einer ausländ. HS studieren)

vn: hsstandlao, hsstandhsao

qt: Offene Angaben

hl:

in: 

q: An welcher Hochschule studieren Sie aktuell?

is: 

it: 

st:

ao1: (hsstandlao): Präfix: Land: [offene Angabe; 60 Zeichen]

ao2: (hsstandhsao): Präfix: Hochschule: [offene Angabe; 60 Zeichen]

mv: 

ka: 

av: 

kh: 

fv: 

hv: 

fo: 

tr:
GOTO D2_1 if mastersplit=1, 2, 5, 6, 7, 8, 11, 12, 14
GOTO A_22 if mastersplit=3, 4, 9, 10, 13

hi: 


\------------------------------------------------------------

A_22
=========

tc:

vn: sperleiszufr

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Alles in allem: Wie zufrieden sind Sie insgesamt mit den Bedingungen an Ihrer Hochschule?

is:

it:

st:

ao: 1: sehr unzufrieden

ao: 2

ao: 3

ao: 4

ao: 5: sehr zufrieden

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_17 IF mastersplit= 1, 2, 3, 4, 7, 8, 9, 10, 14
    GOTO D2_13 IF mastersplit= 5, 6, 11, 12
    GOTO A_23 IF mastersplit= 13
    
hi:

\------------------------------------------------------------

A_23
=========

tc:

vn: sfach1o2, sfach2o2

qt: Offene Angaben

hl:

in:

q: Bitte geben Sie Ihr Studienfach an.

is: Bitte geben Sie nicht Ihren angestrebten Abschluss an (z. B. Masterstudent\*in, Promotionsstudent\*in).

it:

st:

ao1 (sfach1o2): Präfix: erstes Studienfach: [offene Angabe; 60 Zeichen]

ao2 (sfach2o2): Präfix: ggf. zweites Studienfach: [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_24

hi:

\------------------------------------------------------------

A_24
=========

tc:

vn: sabslaja

qt: Einfachauswahl

hl:

in:

q: Sind Sie in einem Lehramtsstudiengang eingeschrieben?

is:

it:

st:

ao1: 1: nein

ao2: 2: Lehramt an Grundschulen (Primarstufe)

ao3: 3: Lehramt an Haupt-, Real- und Sekundar-/Mittelschulen  (Sekundarstufe I)

ao4: 4: Lehramt an Gymnasien und Gesamtschulen (Sekundarstufe II)

ao5: 5: Lehramt an beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: Lehramt an Förderschulen/Sonderpädagogik

mv:

ka: (ao2 TO ao6): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: Bitte über ao2 "Ja, und zwar:" positionieren.

tr: GOTO A_25

hi:

\------------------------------------------------------------

A_25
=========

tc:

vn: sabsano; sabsanoaa; sabsanoka

qt: Einfachauswahl mit offenen Angaben

hl:

in:

q: Und welchen Abschluss streben Sie als nächstes an?

is: Sollten Sie mehrere Abschlüsse anstreben, beziehen Sie sich bitte auf den zeitlich nächsten.

it:

st:

ao1: 1: Bachelor

ao2: 2: Master

ao3: 3: Staatsexamen

ao4: 4: Diplom

ao5: 5: Promotion

ao6: 6: kirchliche Abschlussprüfung

ao7: 7: künstlerische Abschlussprüfung

ao8: 8: Anderen Abschluss (bspw. ausländischer Abschluss, Magister), und zwar: [(sabsanoaa); 60 Zeichen] (offene Angabe)

ao9: 9: Keinen Studienabschluss, sondern: [(sabsanoka); 80 Zeichen] (offene Angabe)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_27 if sabsan=9
    GOTO D1_13 if sabsan=1-8 AND mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14 
    GOTO A_27 if sabsan=1-8 AND mastersplit=5, 6, 11, 12, 13
    GOTO D1_13 if sabsan=MISSING AND mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14 
    GOTO A_27 if sabsan=MISSING AND mastersplit=5, 6, 11, 12, 13

hi:


\------------------------------------------------------------

A_27
=========

tc:

vn: sform (sformpraes; sformdua; sformberu; sformfern; sformgast; sformsons; sformsonso)

qt: Mehrfachauswahl mit offener Angabe

hl:

in:

q: Um welche Form handelt es sich bei Ihrem Studium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (sformpraes): Präsenzstudim (in Gegensatz zu Fernstudium)
ao2: (sformfern): Fernstudium
ao3: (sformdua): duales Studium
ao4: (sformberu): berufsbegleitendes Studium
ao5: (sformgast): Gasthörerschaft
ao6: (sformsons): Anderes, und zwar: [(sformsonso) offene Angabe, 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D2_3 if mastersplit=1, 2, 5, 6, 7, 8, 11, 12, 14
    GOTO B1_7 if mastersplit=3, 4, 13
    GOTO A_28 if mastersplit=9, 10

hi:

\--------------------------------

D1_9 
==

tc:

vn: sartzeit

qt: Einfachauswahl vertikal

hl:

in:

q: Betreiben Sie Ihr Studium in Vollzeit oder Teilzeit?

is:

it:

st:

ao1: 1: Vollzeit

ao2: 2: Teilzeit

ao3: 3: Vollzeitstudiengang mit individueller Teilzeitregelung

ao4: 4: Vollzeitstudiengang inoffiziell als Teilzeitstudium

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_7 IF ssemhs <= 6
    GOTO D1_7 IF ssemhs = k. A. 
    GOTO D2_6 IF (ssemhs >= 7) AND (mastersplit = 1, 2, 7, 8, 14)
    GOTO A_44 IF (ssemhs >= 7) AND (mastersplit = 3, 4, 9, 10)
       

hi:

\------------------------------------------------------------

A_28
=========

tc:

vn: spernot; spernoto

qt: offene Angabe, Einfachauswahl

hl:

in:

q: Mit welcher Note wurden Ihre bisherigen Studienleistungen bewertet?

is: Punktzahl bitte in Note umrechnen.

it:

st:

ao: Prefix: Durchschnittsnote (z. B. 2,5): [(spernoto) offene Angabe, 3-stellig, mit einer Dezimalstelle (1,0 bis 5,0), NUMBER]

ao: (spernot): -11: Ich habe bisher keine Noten erhalten.

ka:

vc:

av: NUMBER, 3-stellig, mit einer Dezimalstelle (1,0 bis 5,0)

kh: Bitte geben Sie Ihre aktuelle Durchschnittsnote an (1,0 bis 5,0)

fv:

hv:

fo: Bitte offene Angabe und Einfachauswahl untereinander, linksbündig positionieren

tr: GOTO A_29

hi: Offene Angabe bitte als NUMBER, 3-stellig, mit einer Dezimalstelle (1,0 bis 5,0), programmieren.

\------------------------------------------------------------

A_29
=========

tc:

vn: sperleisrel

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wie schätzen Sie Ihre bisherigen Studienleistungen im Vergleich zu Ihren Kommiliton\*innen ein?

is:

it:

st:

ao1: 1: unterdurchschnittlich

ao2: 2:

ao3: 3: durchschnittlich

ao4: 4:

ao5: 5: überdurchschnittlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_31

hi:


\------------------------------------------------------------

A_31
=========

tc:

vn: studerfolg; masterfolg; promoerfolg

qt: Mehrfachauswahlmatrix

hl:

in:

q: Inwieweit trauen Sie sich zu, …

is:

it1: (studerfolg): … ein Studium erfolgreich abzuschließen?

it2: (masterfolg): … ein Masterstudium erfolgreich abzuschließen?

it3: (promoerfolg): … eine Promotion erfolgreich abzuschließen?

st:

ao1: 1: überhaupt nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: vollkommen

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_32

hi:

\------------------------------------------------------------

A_32
=========

tc:

vn: deltberuv; deltberum

qt: Comparison

hl:

in:

q: Welches ist der höchste berufliche Abschluss Ihres Vaters/Ihrer Mutter?

is:

it1: (deltberuv): Vater

it2: (deltberum): Mutter

st:

ao1: 7: Promotion (Doktortitel)

ao2: 6: Universitätsabschluss

ao3: 5: Fachhochschulabschluss

ao4: 4: Abschluss an einer Meister-, Techniker-, Fachschule

ao5: 3: Lehre bzw. Facharbeiterabschluss, Abschluss an einer Berufsfach-, Handels-, Berufsaufbauschule

ao6: 2: anderer beruflicher Abschluss

ao7: 1: hat keinen beruflichen Abschluss

ao8: -12: weiß ich nicht

mv: ao8

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_33 if mastersplit=1, 2, 3, 4, 5, 6, 14
    GOTO B2_1 if mastersplit=7, 8, 9, 10, 11, 12, 13

hi:

\------------------------------------------------------------

A_33
=========

tc:

vn: deltjobv (deltjobvo1; deltjobvo2; deltjobv1; deltjobv2); deltjobm (deltjobmo1; deltjobmo2; deltjobm1; deltjobm2)

qt: Comparison, Mehrfachauswahl, offene Angaben

hl:

in:

q: Und welchen Beruf übt Ihr Vater/Ihre Mutter hauptberuflich aus? Bitte erläutern Sie die Tätigkeit Ihres Vaters/Ihrer Mutter kurz.

is: Falls Ihr Vater oder Ihre Mutter zurzeit nicht erwerbstätig sind (z. B. Rentner(in), Pensionär(in), Hausfrau/-mann oder arbeitssuchend), geben Sie bitte die jeweils zuletzt ausgeübte Tätigkeit an.

Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive Führungsaufgaben ein. Zum Beispiel:

\- Bankkaufmann/-frau (nicht: Angestellte/r) 

Beratung, Verkauf von Finanzprodukten, Abteilungsleitung

\- Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in)

Zollfahndung, Einsatzplanung

\- Maschinenbauingenieur(in) (nicht: Ingenieur/in)

Konstruktion, Optimierungsprozesse, Produktionsleitung

it1: (deltjobvo1): Prefix: Berufsbezeichnung: [offene Angabe; 100 Zeichen]

it2: (deltjobvo2): Prefix: Tätigkeitsbeschreibung: [offene Angabe; 100 Zeichen]

it3: (deltjobv1): -11: nie berufstätig gewesen [Einfachauswahl]

it4: (deltjobv2): -12: weiß ich nicht [Exklusivkategorie]

it5: (deltjobmo1): Prefix: Berufsbezeichnung: [offene Angabe; 100 Zeichen]

it6: (deltjobmo2): Prefix: Tätigkeitsbeschreibung: [offene Angabe; 100 Zeichen]

it7: (deltjobm1): -11: nie berufstätig gewesen [Einfachauswahl]

it8: (deltjobm2): -12: weiß ich nicht [Exklusivkategorie]

ao: 

ka:

vc:

av:

kh:

fv:

hv:

fo: „Vater“ und „Mutter“ bitte in einer extra Zeile positionieren, die mittig über den jeweils darunterliegenden Antwortzeilen liegt (siehe Darstellung hierunter):

Vater Mutter

Berufsbezeichnung: Eingabefeld Eingabefeld

Tätigkeitsbeschreibung: Eingabefeld Eingabefeld

weiß ich nicht Kästchen

o Bei Angabe von „weiß ich nicht“, sollen die Textfelder in der jeweiligen
Spalte bitte nicht ausgefüllt werden können und umgekehrt (Exklusivkategorie).

tr: GOTO B2_2a if mastersplit=7, 8, 9, 10, 11, 12, 13 AND h_split==1 (50%)
    GOTO B2_2b if mastersplit=7, 8, 9, 10, 11, 12, 13 AND h_split==2 (50%)
    GOTO B1_6 if mastersplit=1, 2, 3, 4, 5, 6
    GOTO A34 if mastersplit=14

hi:

\------------------------------------------------------------

A_34
=========

tc:

vn: deltgebv; deltgebm

qt: Comparison

hl:

in:

q: Wo wurden Ihre Eltern geboren?

is:

it1 (deltgebv): Vater

it2 (deltgebm): Mutter

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

ao3: 3: weiß ich nicht

mv: ao3

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: <zofar:transition target="A_35" condition="zofar.asNumber(deltgebv)==2 or zofar.asNumber(deltgebm)==2"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.asNumber(deltgebv)==1 and zofar.asNumber(deltgebm)==1)"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.isMissing(deltgebv) and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.asNumber(deltgebv)==1 and zofar.asNumber(deltgebm)==1)"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.isMissing(deltgebv) and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.asNumber(deltgebv)==1 and zofar.asNumber(deltgebm)==1)"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.isMissing(deltgebv) and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.asNumber (deltgebv)==1 and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.asNumber (deltgebm)==1 and zofar.isMissing(deltgebv))"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.asNumber (deltgebv)==1 and zofar.asNumber (deltgebm)==3)"/>
    <zofar:transition target="A_38a" condition="(zofar.asNumber(vsbdeba)==2 and zofar.asNumber (deltgebm)==1 and zofar.asNumber (deltgebv)==3)"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.asNumber (deltgebv)==1 and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.asNumber (deltgebm)==1 and zofar.isMissing(deltgebv))"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.asNumber (deltgebv)==1 and zofar.asNumber (deltgebm)==3)"/>
    <zofar:transition target="A_38" condition="(zofar.asNumber(vsbdeba)==1 and zofar.asNumber (deltgebm)==1 and zofar.asNumber (deltgebv)==3)"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.asNumber (deltgebv)==1 and zofar.isMissing(deltgebm))"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.asNumber (deltgebm)==1 and zofar.isMissing(deltgebv))"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.asNumber (deltgebv)==1 and zofar.asNumber (deltgebm)==3)"/>
    <zofar:transition target="A_38" condition="(zofar.isMissing(vsbdeba) and zofar.asNumber (deltgebm)==1 and zofar.asNumber (deltgebv)==3)"/>
    
hi:

\------------------------------------------------------------

A_35
=====

tc: IF deltgebv=2 

vn: deltgkov

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurde Ihr Vater geboren?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

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

\------------------------------------------------------------

A_35
=====

tc: IF deltgebm=2

vn: deltgkom

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurde Ihre Mutter geboren?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_36

hi:

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstav

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihres Vaters an.

is:

it:

st:

ao: [Dropdown; Staatenliste_DBI_Eltern]

mv:

ka:

vc:  visible="(!zofar.isMissing(deltgkov) or zofar.asNumber(deltkov)!=0) and zofar.asNumber(deltgebv)==2"

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstavo

qt: offene Frage

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihres Vaters an.

is:

it:

st:

ao1: Prefix: Geburtsland des Vaters: [offene Angabe, 50 Zeichen]

mv:

ka:

vc:  visible="(zofar.isMissing(deltgkov) or zofar.asNumber(deltgkov)==0) and zofar.asNumber(deltgebv)==2"

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstam

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihrer Mutter an.

is:

it:

st:

ao: [Dropdown; Staatenliste_DBI_Eltern]

mv:

ka:

vc: visible="(!zofar.isMissing(deltgkom) or zofar.asNumber(deltgkom)!=0) and zofar.asNumber(deltgebm)==2"

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstamo

qt: offene Frage

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihrer Mutter an.

is:

it:

st:

ao1: Prefix: Geburtsland der Mutter:: [offene Angabe, 50 Zeichen]

mv:

ka:

vc: visible="(zofar.isMissing(deltgkom) or zofar.asNumber(deltgkom)==0) and zofar.asNumber(deltgebm)==2"

av:

kh:

fv:

hv:

fo:

tr: GOTO C3_2

hi:

\------------------------------------------------------------

A_37a
========

tc:

vn: vsbplz; vsbort

qt: offene Frage

hl:

in:

q: An welchem Ort haben Sie gewohnt, als Sie die Studienberechtigung erhalten haben? Bitte tragen Sie die fünfstellige Postleitzahl ein.

it:

st:

ao1: (vsbplz): Präfix: Postleitzahl: [offene Angabe, NUMBER, 5-stellig]

ao2: (vsbort): : [offene Angabe, 25-stellig]

mv:

ka:

vc:

av: number, 5-stellig: 01000 TO 99999

kh:

fv: 

hv:

fo: Softreminder: Bitte den Text „Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an:“ erst dann einblenden,
wenn die PLZ nicht angegeben wurde.

tr: GOTO A_41

hi:

\------------------------------------------------------------

A_37b
==========

tc:

vn: vsbplzb; vsbortb

qt: offene Frage

hl:

in:

q: An welchem Ort haben Sie gewohnt, als Sie die Studienberechtigung erhalten haben?

is: Bitte tragen Sie die fünfstellige Postleitzahl und ggf. den Wohnort ein.

it:

st:

ao1: (vsbplzb): Präfix: Postleitzahl: [(vsbplzo) offene Angabe, NUMBER, 5-stellig]

ao2: (vsbortb): : [offene Angabe, 25-stellig]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_41

hi:

\------------------------------------------------------------
A_38a
==========

tc:

vn: intbild1 intbild2 intbild3 intbild4 intbild5 intbild6 intbild7

qt: Mehrfachauswahl

hl:

in:

q: Welchen Bildungsstand hatten Sie, als Sie nach Deutschland kamen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intbild1): Promotion

ao2: (intbild2): Hochschulstudium mit zweitem Abschluss (z. B. Master)

ao3. (intbild3): Hochschulstudium mit erstem Abschluss (z. B. Bachelor)

ao4: (intbild4): begonnenes Hochschulstudium ohne Abschluss

a05: (intbild5): Schulabschluss, der zum Studium berechtigt"

ao6: (intbild6): Schulabschluss ohne Studienberechtigung

ao7: (intbild7): kein Schulabschluss

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: <zofar:transition target="A_38b" condition="(intbild1.value or intbild2.value or intbild3.value or intbild4.value or intbild5.value)"/>
    <zofar:transition target="A_38c" condition="(intbild6.value or intbild7.value)"/>
    <zofar:transition target="A_38c" condition="(!intbild1.value and !intbild2.value and !intbild3.value and !intbild4.value and !intbild5.value and !intbild6.value and !intbild7.value)"

hi:

\------------------------------------------------------------
A_38b
==========

tc:

vn: ankbild1 ankbild2 ankbild3 ankbild4 ankbild5

qt: Einfachauswahlmatrix

hl:

in:

q: Wurden diese Bildungsabschlüsse bzw. Ihre bisherigen Studienleistungen in Deutschland anerkannt?

is:

it1: (ankbild1): Promotion

it2: (ankbild2): Hochschulstudium mit zweitem Abschluss

it3: (ankbild3): Hochschulstudium mit erstem Abschluss

it4: (ankbild4): Teile meines bisherigen Studiums

it5: (ankbild5): schulische Studienberechtigung

st:

ao1: 1: vollständig anerkannt

ao2: 2: teilweise anerkannt

ao3: 3: nicht anerkannt

ao6: -13: weiß ich nicht

mv: ao6

ka:

vc: SHOW it1 if intbild1>0
      SHOW it2 if intbild2>0
      SHOW it3 if intbild3>0
      SHOW it4 if intbild4>0
      SHOW it5 if intbild5>0
av:

kh:

fv:

hv:

fo:

tr: GOTO A_38c

hi:

\------------------------------------------------------------
A_38c
==========

tc:

vn: intvors1 intvors2 intvors3 intvors4 intvors5 intvors5o intvors6

qt: Mehrfachauswahl

hl:

in:

q: Welche zusätzlichen Voraussetzungen mussten Sie für ein Studium in Deutschland erfüllen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intvors1): Feststellungsprüfung

ao2: (intvors2): Nachweis deutscher Sprachkenntnisse (z. B. TestDaF, DSH)

ao3: (intvors3): Nachweis englischer Sprachkenntnisse (z. B. Cambridge FCE, TOEFL, IELTS)

ao4: (intvors4): fachliche Eignungsprüfung (z. B. Kunst, Musik, Sport)

ao5: (intvors5): Etwas anderes, und zwar: [(intvors5o), offene Angabe, 250 Zeichen]

ao6: (intvors6): keine

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 
GOTO D1_2 IF mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14
ELSO GOTO A_40

hi:

\------------------------------------------------------------

A_38
==========

tc:

vn: vsbart

qt: Einfachauswahl

hl:

in:

q: Welchen höchsten Schulabschluss hatten Sie vor Beginn des Studiums erworben?

is:

it:

st:

ao1: 1: allgemeine Hochschulreife

ao2: 2: fachgebundene Hochschulreife

ao3: 3: Fachhochschulreife

ao4: 4: Mittlere Reife

ao5: 5: Hauptschulabschluss

ao6: 6: anderer Abschluss

a07: 7: kein Abschluss

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_39

hi:

\------------------------------------------------------------

A_39
==========

tc:

vn: vsbstyp (vsbstyp1-vsbstyp2; vsbstyp3; vsbstyp4; vsbstyp5; vsbstyp6; vsbstyp7; vsbstyp8; vsbstyp9; vsbstyp10; vsbstyp11; vsbstyp12; vsbstyp13; vsbstyp14; vsbstyp15); vsbtypob

qt: Mehrfachauswahl mit offener Abfrage

hl:

in:

q: Die Berechtigung zum Studium kann in Deutschland auf unterschiedlichen Wegen erfolgen: Zum einen (klassisch) über ein Schulzeugnis, zum anderen aber auch über die Anerkennung beruflicher Qualifikationen oder besonderer Eignungen.

Auf welchem Weg erfolgte Ihre Zulassung zu Ihrem ersten Studium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (vsbtyp1): Gymnasium

ao2: (vsbtyp2): Gesamtschule mit gymnasialer Oberstufe

ao3: (vsbtyp3): Schule in freier Trägerschaft (z. B. Waldorfschule)

ao4: (vsbtyp4): Abendgymnasium, Kolleg (nicht Berufskolleg)

ao5: (vsbtyp5): Fachgymnasium, berufliches Gymnasium

ao6: (vsbtyp6): Berufsfachschule

ao7: (vsbtyp7): Berufsoberschule

ao8: (vsbtyp8): Fachoberschule

ao9: (vsbtyp9): andere berufsbildende Schule (z. B. Fachschule, Fachakademie, Berufskolleg u. a.) [Exklusivkategorie]

ao10: (vsbtyp10): berufliche Aufstiegsfortbildung (z. B. Meister\*in, Techniker\*in, Fachwirt\*in, Erzieher\*in)

ao11: (vsbtyp11): abgeschlossene Berufsausbildung mit anschließender Berufspraxis 

ao12: (vsbtyp12): Eignungsprüfung (z. B. Kunst, Musik, Sport)

ao13: (vsbtyp13): Begabtenprüfung

ao14: (vsbtyp14): Mediziner\*innen-Test (TMS)

ao15: (vsbtyp15): auf einem anderen Weg, und zwar: [(vsbtypob); offen Angabe, 30 Zeichen]

mv:

ka1 (ao1 TO ao9) Schulischer Weg:

ka2(ao10 TO ao11) Berufliche Qualifikation:

ka3(ao12 TO ao15) Eignungsprüfungen:

vc:

av:

kh:

fv:

hv:

fo: Bitte die Beispiele in Klammern in etwas kleinerer Schriftgröße (2pt kleiner) umsetzen.

tr: GOTO D1_1 if (mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14) AND (vsbtyp1=1 OR vsbtyp2=1 OR vsbtyp3=1 OR vsbtyp4=1 OR vsbtyp5=1 OR vsbtyp6=1 OR vsbtyp7=1 OR vsbtyp8=1 OR vsbtyp9=1)
    GOTO A_40 IF ELSE

hi:

\------------------------------------------------------------

A_40
========

tc:

vn: vsbnoteo; vsbnote

qt: Einfachauswahl mit offener Abfrage

hl:

in:

q: Welche Abschlussnote hatten Sie in dem Zeugnis, das Sie zur Aufnahme eines Studiums berechtigt?

is: Punktzahl bitte in Note umrechnen

it:

st:

ao1: 3: Präfix: Durchschnittsnote (z. B. 2,5): [(vsbnoteo); offene Angabe, NUMBER, 3-stellig mit einer Dezimalstelle]

ao2: -11: Ich habe keine Note erhalten. 

ao3: -12: weiß ich nicht 

ka:

vc:

av: 

kh: Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr: 

hi:

\------------------------------------------------------------

A_40
========

tc:

vn: vsbzpj

qt: Einfachauswahl mit Dropdown

hl:

in:

q: In welchem Jahr haben Sie die Hochschulzugangsberechtigung erlangt?

is: Zeitpunkt der Zeugnisübergabe

it: Jahr: [Dropdown, Jahresliste: Jahr, 2019 ... 1999 und früher]

st:

ao:

vc:

av:

kh:

fv:

hv:

fo:

tr:
GOTO A_37a IF h_split=1
GOTO A_37b IF h_split=2

hi:

\------------------------------------------------------------

A_41
===========

tc: 

vn: vausbja

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor dem Studium eine Berufsausbildung begonnen bzw. abgeschlossen?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, begonnen und nicht abgeschlossen

ao3: 3: ja, begonnen und abgeschlossen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_42 if vausbja=1 | k.A.
    GOTO D1_5 if (vausbja=2) AND (mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14)
    GOTO D1_4 if (vausbja=3) AND (mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14)   
    GOTO A_42 if (vausbja=2 | 3) AND (mastersplit=5, 6, 11, 12, 13)

hi:

\------------------------------------------------------------

A_42 
==========

tc:

vn: eaktsens

qt: Einfachauswahl

hl:

in:

q1: Sind Sie während der Vorlesungszeit erwerbstätig?

q2: Sind Sie während der Vorlesungszeit neben Ihrem dualen Studium erwerbstätig?

is: 

it:

st:

ao1: 1: nein

ao2: 2: ja, mit einer Tätigkeit

ao3: 3: ja, mit zwei verschiedenen Tätigkeiten

ao4: 4: ja, mit drei oder mehreren Tätigkeiten

mv:

ka:

vc1: SHOW q1 IF sformdua < 1

vc2: SHOW q2 IF sformdua = 1

av:

kh:

fv:

hv:

fo:

tr: GOTO A_43 IF eaktsens=2 OR eaktsens=3 OR eaktsens=4
    GOTO A_44 IF (eaktsens=1 | k.A.) AND (mastersplit=13)
    GOTO D3_20 IF (eaktsens =1 | k.A. & sformberu=1 | sformdua=1) AND (mastersplit=3, 4, 5, 6, 9, 10, 11, 12, 14)
    GOTO D3_22 IF (eaktsens =1 | k.A. & sformberu!=1 | sformdua!=1) AND (mastersplit=3, 4, 5, 6, 9, 10, 11, 12, 14)
    GOTO D1_9 IF eaktsens=1 | k.A.) AND (mastersplit=1, 2, 7, 8)

hi:

\------------------------------------------------------------

A_43
=========

tc: if eaktsens=2 OR eaktsens=3 OR eaktsens=4

vn: efachnah1, efachnah2, efachnah3

qt: Einfachauswahlmatrix

hl:

in:

q1: In welchem Maße hat ihre Erwerbstätigkeit einen fachlichen Bezug zu Ihrem aktuellen Studium?

q2: In welchem Maße hat Ihre Erwerbstätigkeit, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben, einen fachlichen Bezug zu Ihrem aktuellen Studium?

q3: In welchem Maße haben Ihre Erwerbstätigkeiten einen fachlichen Bezug zu Ihrem aktuellen Studium?

q4: In welchem Maße haben Ihre Erwerbstätigkeiten, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben, einen fachlichen Bezug zu Ihrem aktuellen Studium?

q5: In welchem Maße haben Ihre Erwerbstätigkeiten einen fachlichen Bezug zu Ihrem aktuellen Studium?

q6: In welchem Maße haben Ihre Erwerbstätigkeiten, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben, einen fachlichen Bezug zu Ihrem aktuellen Studium?

is:

it: (efachnah1): Tätigkeit A 

it: (efachnah2): Tätigkeit B 

it: (efachnah3): Tätigkeit C 

st:

ao1: 1: in gar keinem Maße

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv:

ka:

vc1: SHOW q1 IF eaktsens=2 AND sformdua!=1

vc2: SHOW q2 IF eaktsens=2 AND sformdua=1 

vc3: SHOW q3 IF eaktsens=3 AND sformdua!=1

vc4: SHOW q4 IF eaktsens=3 AND sformdua=1 

vc5: SHOW q5 IF eaktsens=4 AND sformdua!=1

vc6: SHOW q6 IF eaktsens=4 AND sformdua=1 

vc7: SHOW it1 IF eaktsens=2 OR eaktsens=3 OR eaktsens=4

vc8: SHOW it2 IF eaktsens=3 OR eaktsens=4 

vc9: SHOW it3 IF eaktsens=4 

av:

kh:

fv:

hv:

fo: 

tr: GOTO D3_19 IF mastersplit=3, 4, 5, 6, 9, 10, 11, 12, 14
    GOTO D1_9 IF mastersplit=1, 2, 7, 8
    GOTO A44 IF mastersplit=13
    
hi:

\------------------------------------------------------------

A_44
=========

tc:

vn: sabsja

qt: Einfachauswahl

hl:

in:

q: Haben Sie bereits einen Hochschulabschluss erworben?

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

tr: GOTO A_49a IF sabsja=1 AND sabser=1
    GOTO A_49b IF sabsja=1 AND sabser!=1
    GOTO A_45 IF sabsja=2
    GOTO A_49a IF sabsja=MISSING AND sabser=1
    GOTO A_49b IF sabsja=MISSING AND sabser!=1
    
hi:

\------------------------------------------------------------

A_45
===========

tc: sabsja==2

vn: sabszp, sabszp2

qt: Einfachauswahl mit Dropdown x2

hl:

in:

q: Wann haben Sie diesen Abschluss erworben?

is:

it1: (sabszp): [Dropdown; infield = Monat; Januar - Februar - März - ... - Dezember]

it2: (sabszp2): [Dropdown; infield = Jahr; 2019 - 2018 - 2017 - ... - 2009 und früher]

st:

ao: 

ao0: (sabszp): 0: Monat

ao1: (sabszp): 1: Januar

ao2: (sabszp): 2: Februar

ao3: (sabszp): 3: März

ao4: (sabszp): 4: April

ao5: (sabszp): 5: Mai

ao6: (sabszp): 6: Juni

ao7: (sabszp): 7: Juli

ao8: (sabszp): 8: August

ao9: (sabszp): 9: September

ao10: (sabszp): 10: Oktober

ao11: (sabszp): 11: November

ao12: (sabszp): 12: Dezember


ao0: (sabszp2): 0: Jahr

ao1: (sabszp2): 1: 2019

ao2: (sabszp2): 2: 2018

ao3: (sabszp2): 3: 2017

ao4: (sabszp2): 4: 2016

ao5: (sabszp2): 5: 2015

ao6: (sabszp2): 6: 2014

ao7: (sabszp2): 7: 2013

ao8: (sabszp2): 8: 2012

ao9: (sabszp2): 9: 2011

ao10: (sabszp2): 10: 2010

ao11: (sabszp2): 11: 2009 und früher

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_46

hi:

\------------------------------------------------------------

A_46
=========

tc: sabsja==2

vn: sabser

qt: Einfachauswahl

hl:

in:

q: Welchen Abschluss haben Sie bereits erworben?

is:

it:

st:

ao1: 1: Bachelor

ao2: 2: Master

ao3: 3: Staatsexamen

ao4: 4: Diplom

ao5: 5: Promotion

ao6: 6: kirchliche Abschlussprüfung

ao7: 7: künstlerische Abschlussprüfung

ao8: 8: anderen Abschluss (bspw. ausländischer Abschluss)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_47
        
hi:

\------------------------------------------------------------

A_47
========

tc: sabsja==2

vn: sabsla

qt: Einfachauswahl

hl:

in:

q: Handelt es sich hierbei um ein Lehramtsstudium?

is: Bei mehreren Hochschulabschlüssen bitte den letzten angeben.

it:

st:

ao1: 1: nein

ao2: 2: ja, und zwar Lehramt an Grundschulen (Primarstufe)

ao3: 3: ja, und zwar Lehramt an Haupt-, Real- und Mittelschulen (Sekundarstufe I)

ao4: 4: ja, und zwar Lehramt an Gymnasien (Sekundarstufe II)

ao5: 5: ja, und zwar Lehramt an beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: ja, und zwar Lehramt an Förderschulen/Sonderpädagogik

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_48

hi:

\------------------------------------------------------------

A_48
=========

tc: sabsja==2

vn: sabsernot, sabsernoto

qt: Einfachauswahl mit offene Angabe

hl:

in:

q: Welche Abschlussnote haben Sie in Ihrem vorherigen Studium erhalten?

is: Für den Fall, dass Sie keine Noten erhalten haben, sondern Ihre Studienleistungen mit Punkten, Prozentangaben o. Ä. bewertet werden, rechnen Sie diese bitte in eine Abschlussnote um.

it:

st:

ao1 (sabsernot): 1: Prefix: Abschlussnote (z. B. 2,5): [(sabsernoto); offene Angabe: 3 Zeichen mit einer Dezimalstelle]

ao2 (sabsernot): -11: Ich habe keine Note erhalten. / In meinem vorigen Studium gab es keine Noten.

ao3 (sabsernot): -12: weiß ich nicht

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr: GOTO D1_10a IF mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14
    GOTO A_49a IF (mastersplit=5, 6, 11, 12, 13) AND (sabser==1)
    GOTO A_49b IF (mastersplit=5, 6, 11, 12, 13) AND (sabser!=1)

hi:

\------------------------------------------------------------

A_49a
=========

tc:

vn: mastplan; promoplan

qt: Einfachauswahlmatrix

hl:

in:

q: Wie wahrscheinlich ist es, dass Sie…

is:

it1: (mastplan): … ein Masterstudium aufnehmen?

It2: (promoplan) … eine Promotion aufnehmen?

st:

ao1: 1: sehr unwahrscheinlich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:  GOTO KSM-anf01 IF (mastersplit=1, 3, 5) AND zusatzsplit=2 AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf02 IF (mastersplit=7, 9, 11, 13) AND zusatzsplit=2 AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf01 IF (mastersplit=2, 4, 6, 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf02 IF (mastersplit=8, 10, 12) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=2) AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-ma01 IF (mastersplit=1, 3, 5, 7, 9, 11, 13) AND zusatzsplit=2 AND sabsan=1 AND ssemfs>5
     GOTO KSM-ma01 IF (mastersplit=2, 4, 6, 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND sabsan=1 AND ssemfs>5
     GOTO KSM-phd01 IF (mastersplit=1, 3, 5, 7, 9, 11, 13) AND zusatzsplit=2 AND (sabsan=2, 3, 4, 6, 7, 8) AND ssemfs>5
     GOTO KSM-phd01 IF (mastersplit=2, 4, 6, 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND (sabsan=2, 3, 4, 6, 7, 8) AND ssemfs>5
     GOTO A_50 IF zusatzsplit=1 OR zusatzsplit=3 OR zusatzsplit=4
     GOTO A_50 IF (mastersplit=2, 4, 6, 8, 10, 12, 14) AND zusatzsplit=2 AND (vsbdeba=1 AND imausl=1)
     GOTO A_50 IF (mastersplit=2, 4, 6, 8, 10, 12, 14) AND zusatzsplit=2 AND (vsbdeba=MISSING OR imausl=MISSING)
     
hi:


\------------------------------------------------------------

A_49b
=========

tc:

vn: promoplan

qt: Einfachauswahl mit Horizontalen ao

hl:

in:

q: Wie wahrscheinlich ist es, dass Sie...

is:

it:

st: … eine Promotion aufnehmen?

ao1: 1: sehr unwahrscheinlich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:  GOTO KSM-anf01 IF (mastersplit=1, 3, 5) AND zusatzsplit=2 AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf02 IF (mastersplit=7, 9, 11, 13) AND zusatzsplit=2 AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf01 IF (mastersplit=2, 4, 6, 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-anf02 IF (mastersplit=8, 10, 12) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=2) AND (sabsan=1, 3, 4, 6, 7, 8) AND ssemfs<=5
     GOTO KSM-ma01 IF (mastersplit=1, 3, 5, 7, 9, 11, 13) AND zusatzsplit=2 AND sabsan=1 AND ssemfs>5
     GOTO KSM-ma01 IF (mastersplit=2, 4, 6, 8, 10, 12 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND sabsan=1 AND ssemfs>5
     GOTO KSM-phd01 IF (mastersplit=1, 3, 5, 7, 9, 11, 13) AND zusatzsplit=2 AND (sabsan=2, 3, 4, 6, 7, 8) AND ssemfs>5
     GOTO KSM-phd01 IF (mastersplit=2, 4, 6, 8, 10, 12 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1) AND (sabsan=2, 3, 4, 6, 7, 8) AND ssemfs>5
     GOTO A_50 IF zusatzsplit=1 OR zusatzsplit=3 OR zusatzsplit=4
     GOTO A_50 IF (mastersplit=2, 4, 6, 8, 10, 12, 14) AND zusatzsplit=2 AND (vsbdeba=1 AND imausl=1)
     GOTO A_50 IF (mastersplit=2, 4, 6, 8, 10, 12, 14) AND zusatzsplit=2 AND (vsbdeba=MISSING OR imausl=MISSING)
     

hi:

\------------------------------------------------------------

A_50
=========

tc:

vn: ssweja; saweja; shwja; ssuja

qt: Einfachauswahl matrix

hl:

in:

q: Haben Sie seit Ihrer Erstimmatrikulation…

is: Nicht gemeint sind Veränderungen bzw. Unterbrechungen beim Übergang vom Bachelor- ins Masterstudium.

it1: (ssweja): … das Studienfach gewechselt?

it2: (saweja): … den Abschluss gewechselt?

it3: (shwja): … die Hochschule gewechselt?

it4: (ssuja): … das Studium zwischenzeitlich unterbrochen?

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

tr: GOTO D1_14 IF (ssweja=1 OR saweja=1 OR shwja=1 OR ssuja=1) AND (mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14)
    GOTO A_51a if (ssweja=1 OR saweja=1 OR shwja=1 OR ssuja=1 AND h_split=1 (50%)) AND (mastersplit=5, 6, 11, 12, 13)
    GOTO A_51b if (ssweja=1 OR saweja=1 OR shwja=1 OR ssuja=1 AND h_split=2 (50%)) AND (mastersplit=5, 6, 11, 12, 13)
    GOTO A_51a if (ssweja=2 AND saweja=2 AND shwja=2 AND ssuja=2) AND (h_split=1 (50%))
    GOTO A_51b if (ssweja=2 AND saweja=2 AND shwja=2 AND ssuja=2) AND (h_split=2 (50%))
    GOTO A_51a if (ssweja=k.A. AND saweja=k.A. AND shwja=k.A. AND ssuja=k.A.) AND (h_split=1 (50%))
    GOTO A_51b if (ssweja=k.A. AND saweja=k.A. AND shwja=k.A. AND ssuja=k.A.) AND (h_split=2 (50%))

hi:

\------------------------------------------------------------

A_51a
=========

tc:

vn: ssahswe; ssafawe; ssaunt; ssaaja

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit denken Sie daran…

is:

it1: (ssahswe): … die Hochschule zu wechseln?

it2: (ssafawe): … Ihr Studienfach zu wechseln?

it3: (ssaunt): … Ihr aktuelles Studium zu unterbrechen?

it4: (ssaaja): … das Studium ganz aufzugeben?

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr ernsthaft

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_20 IF mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14
    GOTO A_52 IF mastersplit=5, 6, 11, 12, 13	

hi:

\------------------------------------------------------------

A_51b
=========

tc:

vn: ssahswe; ssafawe; ssaunt; ssaaja

qt: Einfachauswahlmatrix

hl:

in:

q: Wie ernsthaft denken Sie zur Zeit daran …

is:

it1: (ssahswe): … die Hochschule zu wechseln?

it2: (ssafawe): … Ihr Studienfach zu wechseln?

it3: (ssaunt): … Ihr aktuelles Studium zu unterbrechen?

it4: (ssaaja): … das Studium ganz aufzugeben?

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr ernsthaft

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_20 IF mastersplit=1, 2, 3, 4, 7, 8, 9, 10, 14
    GOTO A_52 IF mastersplit=5, 6, 11, 12, 13	

hi:

\------------------------------------------------------------

A_52
=========

tc:

vn: wohnfo

qt: Einfachauswahl

hl:

in:

q1: Wie wohnen Sie während der Vorlesungszeit des aktuellen Semesters? 

is: Bitte beziehen Sie Ihre Angaben auf Ihren Hauptwohnsitz.
Wenn Sie bei Ihren Eltern oder anderen Verwandten/Bekannten wohnen, geben Sie bitte die Wohnform Ihrer Eltern bzw. der Verwandten/Bekannten an.

it:

st:

ao1: 1: zur Miete (auch Wohngemeinschaft)

ao2: 2: zur Untermiete

ao3: 3: als (Mit-)Eigentümer\*in

ao4: 4: im Einzelzimmer (Flurgemeinschaft)

ao5: 5: im Einzelzimmer (in einer Wohngruppe)

ao6: 6: im Einzelappartement

ao7: 7: in einer Mehrzimmerwohnung (für Paare oder Studierende mit Kind)

mv:

ka1: (ao1 TO ao3): in einer Wohnung, einem Zimmer oder einem Haus

ka2: (ao4 TO ao7): im Studierendenwohnheim

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_1 if mastersplit=3, 4, 5, 6, 9, 10, 11, 12, 14
    GOTO A_53 IF mastersplit=1, 2, 7, 8, 13	

  
hi:

\------------------------------------------------------------

A_53
=========

tc:

vn: wohnal; wohnwg; wohnel; wohnpar; wohnkin; wohnfam; wohnsons

qt: Mehrfachauswahl

hl:

in:

q1: Mit wem wohnen Sie während der Vorlesungszeit des aktuellen Semesters überwiegend zusammen?

is: 

it:

st: Ich wohne …

ao1: (wohnal): allein. [Exklusivkategorie]

ao2: (wohnwg): mit Mitbewohner\*innen in einer Wohngemeinschaft.

ao3: (wohnel): bei meinen Eltern (bzw. einem Elternteil)

ao4: (wohnpar): mit meinem/meiner (Ehe-) Partner\*in.

ao5: (wohnkin): mit meinem Kind/meinen Kindern.

ao6: (wohnfam): mit anderen Familienangehörigen.

ao7: (wohnsons): mit anderen Personen.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_2 IF wohnal != 1 AND mastersplit = 3, 4, 5, 6, 9, 10, 11, 12, 14
    GOTO D3_4 IF wohnal = 1 AND mastersplit = 3, 4, 5, 6, 9, 10, 11, 12, 14
    GOTO B2_5 IF mastersplit= 7, 8, 13
    GOTO B1_5 IF mastersplit= 1, 2
  
hi:

\------------------------------------------------------------

A_54
=========

tc:

vn: ainfaus

qt: Einfachauswahl

hl:

in:

q: Waren Sie im Rahmen Ihres Studiums bereits im Ausland?

is: 

it:

st:

ao1: 1: nein

ao2: 2: ja, ein Aufenthalt

ao3: 3: ja, zwei Aufenthalte

ao4: 4: ja, drei oder mehr Aufenthalte

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_55

hi:

\------------------------------------------------------------

A_55
=========

tc:

vn: auslandint

qt: Einfachauswahl

hl:

in:

q1: Beabsichtigen Sie künftig einen studienbezogenen Auslandsaufenthalt durchzuführen?

q2: Beabsichtigen Sie einen weiteren studienbezogenen Auslandsaufenthalt durchzuführen?

is:

it:

st:

ao1: 1: nein, kein Interesse

ao2: 2: nein, sehe keine Realisierungschance

ao3: 3: weiß ich noch nicht

ao4: 4: ja

mv:

ka:

vc: 

SHOW q1 if ainfaus=1

SHOW q2 if ainfaus=2 OR ainfaus=3 OR ainfaus=4

av:

kh:

fv:

hv:

fo:

tr: GOTO F1_1 if mastersplit=2, 4, 6, 8, 10, 12, 14
    GOTO E1_1 if mastersplit=1, 3, 5, 7, 9, 11, 13 AND zusatzsplit=1
    GOTO KSM-pol01 if mastersplit=1, 3, 5, 7, 9, 11, 13 AND zusatzsplit=3
    GOTO KSM-fai01 if mastersplit=1, 3, 5, 7, 9, 11, 13 AND zusatzsplit=4
    GOTO A_56 IF (mastersplit=1, 3, 5, 7, 9, 11, 13) AND zusatzsplit=2
    GOTO A_56 IF (mastersplit=2, 4, 6, 8, 10, 12 14) AND zusatzsplit=2 AND ((vsbdeba=1 AND dnatausl=0) OR imausl=1)

hi:


\------------------------------------------------------------

A_56
=========

tc:

vn: (zlvwo, zlvwo2) (zseswo, zseswo2) (zerwo, zerwo2) (zcarwo, zcarwo2)

qt: offene Frage Matrix

hl:

in:

q: Wie viele Stunden wenden Sie in einer für Sie typischen Woche für folgende Aktivitäten auf?

is: Bitte runden Sie Ihre Zeitangaben jeweils auf volle Zeitstunden.

it: Vorlesungszeit / Studienphase

it: vorlesungsfreien Zeit / Praxisphase

st:

ao1: (zlvwo, zlvwo2): Lehrveranstaltungen (Vorlesungen, Seminare, Übungen, Tutorien usw.)

ao2: (zseswo, zseswo2): Selbststudium (Vor‐/Nachbereitung, Referate, Fachlektüre, Studien-/Haus-/Abschlussarbeiten, stud. Lerngruppen, Prüfungsvorbereitung usw.)

ao3: (zerwo, zerwo2): Erwerbstätigkeit (Nebenjob, Beruf, freiberufliche/selbstständige Tätigkeit usw.)

ao4: (zcarwo, zcarwo2): Pflege- und Betreuungsarbeiten (Familienleben, Kinderbetreuung, Pflege Angehöriger usw.)

mv:

ka: Während der...

vc:

av: number: \<= zweistellig, 0 TO 99

kh: Bitte geben Sie volle Zeitstunden an (0 bis 99).

fv:

hv:

fo:

tr: <zofar:transition target="N_1" condition="zofar.asNumber(zusatzsplit)==1"/>
    <zofar:transition target="N_13" condition="zofar.asNumber(zusatzsplit)==4"/>
    <zofar:transition target="N_5" condition="zofar.asNumber(zusatzsplit)==3"/>
    <zofar:transition target="A_57" condition="zofar.asNumber(zusatzsplit)==2"/>

hi:


\------------------------------------------------------------

N_1
=========
tc: IF NRW / zusatzsplit ==1

vn: nrwstudium, nrwfach

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Würden Sie wieder…

is:

it1: (nrwstudium): … ein Studium aufnehmen?

it2: (nrwfach): … das gleiche Studienfach wählen?

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

tr: GOTO N_2

hi:


\------------------------------------------------------------

N_2
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwstudium2

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie überzeugt sind Sie momentan von Ihrer Entscheidung, zu studieren?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_3

hi:


\------------------------------------------------------------

N_3
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwfach2

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie überzeugt sind Sie momentan von Ihrer Entscheidung, Ihren Studiengang/Ihre Fächerkombination zu studieren?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_4

hi:


\------------------------------------------------------------

N_4
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwregel

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie wichtig ist Ihnen ein Abschluss in Regelstudienzeit, d. h. in der Anzahl an Fachsemestern, wie es der Studienverlaufsplan vorsieht?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_57

hi:


\------------------------------------------------------------

N_5
=========

tc: IF zusatzsplit == 3

vn: nrwdigbed

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie schätzen Sie Ihren Bedarf an digitalen Selbstlernangeboten in Ihrem Studiengang ein?

is:

it:

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

tr: GOTO N_6

hi:


\------------------------------------------------------------

N_6
=========

tc:

vn: nrwdigged

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: In welchem Maße wird Ihr Bedarf an digitalen Selbstlernangeboten durch die Hochschule gedeckt?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_7

hi:


\------------------------------------------------------------

N_7
=========

tc:

vn: nrwselbtest

qt: vertikale Einfachauswahlmatrix

hl:

in:

q: Haben Sie vor/zu Studienbeginn einen von Ihrer Hochschule angebotenen Selbsttest zur fachlichen Eignung durchgeführt? Und wie 
hilfreich waren die Ergebnisse des Selbsttests (bspw. Online-Self-Assessment/OSA, Studicheck, Wissenstest etc.)?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv: 7: Test nicht durchgeführt/angeboten

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_8

hi: mv ist von den übrigen aos abgesetzt, nicht Teil der Antwortmatrix


\------------------------------------------------------------

N_8
=========

tc:

vn: nrwstudipor

qt: vertikale Einfachauswahlmatrix

hl:

in:

q: Haben Sie zu Studienbeginn die E-Learning-Angebote im landesweiten Onlineportal "Studiport" genutzt? Halten Sie rückblickend diese E-Learning-Angebote für hilfreich?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

mv: 7: Angebot nicht bekannt/nicht genutzt

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_9

hi: mv ist von den übrigen aos abgesetzt, nicht Teil der Antwortmatrix


\------------------------------------------------------------

N_9
=========

tc:

vn: digorg1, digorg2, digorg3, digorg4, digorg5

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie häufig werden die folgenden Aspekte Ihrer Lehrveranstaltungen über digitale Plattformen organisiert? (z. B. StudIP, Moodle, 
Ilias, Olat)

is:

it1: (digorg1): An-/Abmeldung zu Lehrveranstaltungen

it2: (digorg2): Kommunikation innerhalb der Lehrveranstaltungen

it3: (digorg3): Bereitstellung von Literatur und Lehrmaterialien

it4: (digorg4): Erbringung von Leistungsnachweisen / elektronische Prüfungen

it5: (digorg5): An-/Abmeldung zu Prüfungen, Ergebniseinsicht

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig 

ao6: -13:  weiß nicht  

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_10

hi: ao6 (missing) ist abgesetzt von ao1-ao5


\------------------------------------------------------------

N_10
=========

tc:

vn: diglehr1, diglehr2, diglehr3, diglehr4, diglehr5, diglehr6, diglehr7, diglehr8, diglehr9, diglehr10, diglehr11, diglehr12, 
diglehr12o

qt: horizontale Einfachauswahlmatrix / offene Angabe

hl:

in:

q: Wie häufig kommen folgende digitale Methoden bzw. Medien im Rahmen der von Ihnen besuchten Lehrveranstaltungen zum Einsatz?

is:

it1: (diglehr1): Online-Vorlesung (z. B. Live-Digitized-Lecture oder archivierte Aufzeichnung)

it2: (diglehr2): Online-Seminare

it3: (diglehr3): Online-Selbststudium mit anschließender Vertiefung im Präsenzstudium

it4: (diglehr4): virtuelle Lernorte / Labore

it5: (diglehr5): Lehr- und Lernvideos / E-Lecture

it6: (diglehr6): E-Tutorial / E-Coaching (z. B. Web Based Training)

it7: (diglehr7): Lernspiele / Game-Based Learning

it8: (diglehr8): Präsentationssoftware (z. B. PowerPoint, Prezi)

it9: (diglehr9): Smart-Board 

it10: (diglehr10): fachspezifische Software (z. B. Statistik- oder Transkriptionsprog.)

it11: (diglehr11): Kommunikationstools

it12: (diglehr12): Etwas anderes und zwar: [diglehr12o, 50 Zeichen] 

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig 

ao6: -13: kenne ich nicht

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_11

hi: ao6 (missing) ist abgesetzt von ao1-ao5


\------------------------------------------------------------

N_11
=========

tc:

vn: digkom1, digkom2, digkom3, digkom4, digkom5, digkom6

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Inwieweit nutzen Sie die folgenden digitalen Möglichkeiten bei der Zusammenarbeit mit Ihren Kommiliton\*innen)? 

is:

it1: (digkom1): Instant Messaging-Dienste (z. B. WhatsApp, Telegram)

it2: (digkom2): Soziale Netzwerke (z. B. Facebook, Instagram)

it3: (digkom3): Online Verwaltungstools (z. B. Doodle)

it4: (digkom4): Tools der Lernmanagementsysteme (z. B. Peer-Feedback, Foren)

it5: (digkom5): Clouddienste zum gemeinsamen Schreiben (z.B. Etherpad, Google docs)

it6: (digkom6): Clouddienste zum Dateienaustausch (z. B. Dropbox)

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig 

ao6: -13: kenne ich nicht

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_12

hi: ao6 (missing) ist abgesetzt von ao1-ao5


\------------------------------------------------------------

N_12
=========

tc:

vn: digan1, digan2, digan3, digan4, digan5, digan6, digan7, digan8, digan9, digan10, digan11

qt: horizontale Einfachauswahlmatrix

hl:

in:

q: Wie leicht würde es Ihnen fallen, …

is:

it1: (digan1): … eine animierte Präsentation zu gestalten (z. B. mit Power Point, Prezi)? 

it2: (digan2): … eine Literaturdatenbank anzulegen (z. B. mit Citavi, EndNote)?

it3: (digan3): … eine bestimmte Publikation als Download zu finden?

it4: (digan4): … zentrale Literatur zu einem wissenschaftlichen Thema online zu recherchieren?

it5: (digan5): … einen Text nach bestimmten Vorgabe  zu formatieren (z. B. mit Word, Latex)? 

it6: (digan6): …  wissenschaftliche von nicht-wissenschaftlichen Internetquellen zu unterscheiden?

it7: (digan7): … sich in ein neues Computerprogramm einzuarbeiten?

it8: (digan8): … eine Website zu programmieren?

it9: (digan9): … eine Programmiersprache (z. B. Python, SQL, QML) sicher anzuwenden?

it10: (digan10): … digitale Gruppen/Netzwerke zu recherchieren und sich zu beteiligen?

it11: (digan11): … digitale Gruppen/Netzwerke zu initiieren und zu moderieren?

st:

ao1: 1: sehr leicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr schwer

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_57

hi:


\------------------------------------------------------------

N_13
=========

tc: IF zusatzsplit ==4

vn: diskjane, diskjane1, diskjane2, diskjane3, diskjane4, diskjane5, diskjane6, diskjane7, diskjane8, diskjane9, diskjane10, 
diskjane11, diskjane12, diskjane13, diskjane14, diskjane15, diskjane16, diskjane16o

qt: Mehrfachauswahl

hl:

in: Nun geht es um das Thema Diskriminierung. Diskriminierung bedeutet, dass eine Person aus bestimmten Gründen schlechter behandelt 
wird als andere Menschen, ohne dass es dafür eine sachliche Rechtfertigung gibt. 

q: !!Haben Sie selbst bereits diskriminierende Erfahrungen im Rahmen Ihres Studiums gemacht?!!

is:

it:

st:

ao1: (diskjane): nein  

ao2: (diskjane1): Leistungen wurden mir nicht zugetraut.

ao3: (diskjane2): Von mir erbrachte Leistungen wurden herabgesetzt (z. B. ungerecht bewertet).

ao4: (diskjane3): Regeln/Verfahren wurden so gestaltet, dass ich benachteiligt wurde. 

ao5: (diskjane4): Mir wurden Rechte/Informationen vorenthalten.

ao6: (diskjane5): Mein Antrag wurde abgelehnt oder mir wurde eine Leistung verwehrt. 

ao7: (diskjane6): Ich wurde durch Barrieren eingeschränkt (z. B. Hindernisse, Erreichbarkeit von Räumen). 

ao8: (diskjane7): Ich wurde ausgegrenzt oder übergangen (z. B. in Arbeitsgruppen).

ao9: (diskjane8): Menschen wie ich wurden stereotyp/herabwürdigend dargestellt.

ao10: (diskjane9): Mir sind unangebrachte Fragen oder Bemerkungen zu meinem Privatleben begegnet. 

ao11: (diskjane10): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

ao12: (diskjane11): Ich wurde beleidigt oder beschimpft. 

ao13: (diskjane12): Ich habe unerwünschte sexualisierte Kommentare erlebt.

ao14: (diskjane13): Ich habe sexualisierte körperliche Übergriffe erlebt. 

ao15: (diskjane14): Ich wurde körperlich bedroht.

ao16: (diskjane15): Ich wurde körperlich angegriffen. 

ao17: (diskjane16): sonstiges: [(diskjane16o), 50 Zeichen] 

mv:

ka (ao2 TO ao17): ja, und zwar: 

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_57 IF diskjane=1
    GOTO N_14 IF diskjane!=1


\------------------------------------------------------------

N_14
=========

tc:

vn: diskanza1, diskanza2, diskanza3, diskanza4, diskanza5, diskanza6, diskanza7, diskanza8, diskanza9, diskanza10, diskanza11, 
diskanza12, diskanza13, diskanza14, diskanza15

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig haben Sie diese Erfahrungen im Rahmen des Studiums gemacht?

is:

it1: (diskanza1): Leistungen wurden mir nicht zugetraut.

it2: (diskanza2): Von mir erbrachte Leistungen wurden herabgesetzt (z. B. ungerecht bewertet).

it3: (diskanza3): Regeln/Verfahren wurden so gestaltet, dass ich benachteiligt wurde.

it4: (diskanza4): Mir wurden Rechte/Informationen vorenthalten.

it5: (diskanza5): Mein Antrag wurde abgelehnt oder mir wurde eine Leistung verwehrt.

it6: (diskanza6): Ich wurde durch Barrieren eingeschränkt (z. B. Hindernisse, Erreichbarkeit von Räumen).

it7: (diskanza7): Ich wurde ausgegrenzt oder übergangen (z. B. in Arbeitsgruppen).

it8: (diskanza8): Menschen wie ich wurden stereotyp/herabwürdigend dargestellt.

it9: (diskanza9): Mir sind unangebrachte Fragen oder Bemerkungen zu meinem Privatleben begegnet.

it10: (diskanza10): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

it11: (diskanza11): Ich wurde beleidigt oder beschimpft.

it12: (diskanza12): Ich habe unerwünschte sexualisierte Kommentare erlebt.

it13: (diskanza13): Ich habe sexualisierte körperliche Übergriffe erlebt.

it14: (diskanza14): Ich wurde körperlich bedroht.

it15: (diskanza15): Ich wurde körperlich angegriffen.

st:

ao1: 1: einmal

ao2: 2: mehrmals

ao3: 3: regelmäßig

ao4: 4: weiß nicht wie häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO N_15

hi:


\------------------------------------------------------------

N_15
=========

tc:

vn: diskwem1; diskwem2; diskwem3; diskwem4; diskwem5; diskwem6; diskwem7; diskwem8; diskwem8o

qt:  Mehrfachauswahl mit vertikaler Antwortoption und offenem Feld

hl:

in:

q: Von wem oder was ging die Benachteiligung/Diskriminierung aus?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (diskwem1): Studierende

ao2: (diskwem2): Tutor\*innen

ao3: (diskwem3): Lehrende

ao4: (diskwem4): Verwaltungsmitarbeiter\*innen

ao5: (diskwem5): Materielle Gegebenheiten/technische Ausstattung

ao6: (diskwem6): Verfahren/Regelungen

ao7: (diskwem7): Keine Angabe

ao8: (diskwem8): Andere: [diskwem8o, 350 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_57

hi:


\------------------------------------------------------------

A_57
=========

tc:

vn: sdkzei1; sdkzei2; sdkzei3; sdkzei4; sdkzei5; sdkzei6; sdkzei7; sdkzei8; sdkzei9; sdkzei10; sdkzei11; sdkzei12; sdkzei13; sdkzei14; sdkzei15; sdkzei16

qt: Einfachauswahlmatrix

hl:

in:

q: Wie wichtig sind Ihnen die folgenden Aspekte des weiteren Berufs- und Lebensweges?

is:.

it: (sdkzei1): hohes Einkommen

it: (sdkzei2): prestigeträchtige Berufsposition

it: (sdkzei3): sicherer Arbeitsplatz

it: (sdkzei4): gute Aufstiegsmöglichkeiten

it: (sdkzei5): flexible Arbeitszeiten

it: (sdkzei6): die Erwartungen meiner Vorgesetzten zu erfüllen

it: (sdkzei7): verantwortungsvolle Aufgaben zu übernehmen

it: (sdkzei8): eigene Ideen verwirklichen zu können

it: (sdkzei9): selbstständig Entscheidungen treffen zu können

it: (sdkzei10): eine Arbeit, die mir immer wieder neue Aufgaben stellt

it: (sdkzei11): Möglichkeit zu wissenschaftlicher Tätigkeit

it: (sdkzei12): anderen Menschen helfen zu können

it: (sdkzei13): ein Beruf, in dem ich Nützliches für die Allgemeinheit tun kann

it: (sdkzei14): Vereinbarkeit von Privatleben und Beruf

it: (sdkzei15): eine glückliche Beziehung zu führen

it: (sdkzei16): eine Familie zu gründen

st:

ao1: 1: unbedeutend

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr bedeutend

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO ABSCHLUSSSEITE

hi:
