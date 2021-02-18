\------------------------------------------------------------

index
=========

tc:

vn: sid_ic

qt: Mehrfachauswahl

hl: 

in:

q: 
Studie: !!Die Studierendenbefragung in Deutschland!!
(Leerzeile)

Herzlich willkommen bei !!Die Studierendenbefragung in Deutschland!!
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

ao: (sid_ic): Ich habe die Datenschutzbestimmungen gelesen und bin damit einverstanden. Meine Teilnahme an der Befragung ist freiwillig. Diese Einwilligung bezieht sich ausdrücklich auch auf die Angaben zur gesundheitlichen Beeinträchtigung.

mv:

ka:

vc:
SHOW kh1 IF sid_ic != 1

av:

kh1: Bitte beachten Sie, dass ohne Zustimmung zu den Datenschutzbestimmungen eine Teilnahme an der Vorstudie von 
						#{layout.BOLD_START}“Die Studierendenbefragung in Deutschland“#{layout.BOLD_END} leider nicht möglich ist.

fv:

hv:
mastersplit= 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14 (einmalige Randomisierung; mit gleicher Ziehungswahrscheinlichkeit)

zusatzsplit = 1, 2, 3, 4 (einmalige Randomisierung; mit gleicher Ziehungswahrscheinlichkeit)

fo:

tr: 

	<zofar:transitions>
  		<zofar:transition target="index" condition="!sidpretest_consent.value and !sf_h.value"/>
  		<zofar:transition target="offer" condition="sidpretest_consent.value and jsCheck.value and isMobile.value and width.value lt 768"/>
  		<zofar:transition target="A_1" condition="sidpretest_consent.value"/>
	</zofar:transitions>

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_1"/>
        </zofar:transitions

hi:


\------------------------------------------------------------

A_1
=========

tc:

vn: vsbdeba

qt: Einfachauswahl mit vertikalen ao

hl:

in: Um die Befragung passend für Ihre Situation gestalten zu können und insbesondere auf die Situation internationaler Studierender eingehen zu können, müssen wir Ihnen zu Beginn zwei zentrale Eingangsfragen stellen:

q: Wo haben Sie erstmals Ihre Hochschulzugangsberechtigung erworben?

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

vn: dnatdeu; dnatausl

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Und: Welche Staatsangehörigkeit haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dnatdeu): deutsche Staatsangehörigkeit

ao2: (dnatausl): andere Staatsangehörigkeit(en)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte diese Frage zusammen mit der vorherigen Frage auf einer Seite (A1) darstellen. Fragetext,Ausfüllanweisung und Antwortoptionen der vorliegenden Frage bitte zusammen unterhalb von Fragetext und Antwortoptionen der vorhergehenden Frage platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_2" condition="dnatdeu.value"/>
            <zofar:transition target="A_3" condition="!dnatdeu.value and dnatausl.value"/>
            <zofar:transition target="A_5" condition="!dnatdeu.value and !dnatausl.value"/>
        </zofar:transitions>

hi:


\------------------------------------------------------------

A_2
====

tc:

vn: dnatderw

qt: Einfachauswahl mit vertikalen ao

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

        <zofar:transitions>
            <zofar:transition target="A_3" condition="dnatausl.value or (dnatdeu.value and (zofar.asNumber(dnatderw)==2 or zofar.asNumber(dnatderw)==3))"/>
            <zofar:transition target="A_3" condition="dnatausl.value and zofar.asNumber(dnatderw)==1"/>
            <zofar:transition target="A_3" condition="dnatausl.value and zofar.isMissing(dnatderw)"/>
            <zofar:transition target="A_5" condition="dnatdeu.value and zofar.asNumber(dnatderw)==1"/>
            <zofar:transition target="A_5" condition="dnatdeu.value and zofar.isMissing(dnatderw)"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_3
====

tc:

vn: dnatko

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Welche Staatsangehörigkeit besaßen Sie, bevor Sie nach Deutschland kamen?

q2: Welche Staatsangehörigkeit besaßen Sie vor Ihrer Einbürgerung?

q3: Sie haben angegeben, die deutsche und eine ausländische Staatsangehörigkeit zu haben. Welche Staatsangehörigkeit besitzen Sie neben der deutschen?

q4: Sie haben angegeben, eine ausländische Staatsangehörigkeit zu haben. Welche ausländische Staatsangehörigkeit besitzen Sie?

is: Bitte wählen Sie zunächst den Kontinent aus. 

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

SHOW q1 IF dnatderw=2 AND dnatausl=0

SHOW q2 IF dnatderw=3 AND dnatausl=0

SHOW q3 IF dnatdeu=1 AND dnatausl=1

SHOW q4 IF dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: 

        <zofar:transitions>
            <zofar:transition target="A_4"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_4
====

tc:

vn: dnatsta; dnatstao

qt: Dropdown; offene Angabe

hl:

in:

q1: Bitte geben Sie nun die Staatsangehörigkeit an, die Sie hatten, bevor Sie nach Deutschland kamen.

q2: Bitte geben Sie nun Ihre Staatsangehörigkeit vor Ihrer Einbürgerung an.

q3: Bitte geben Sie nun Ihre Staatsangehörigkeit an, die Sie neben der deutschen besitzen.

q4: Bitte geben Sie nun Ihre ausländische Staatsangehörigkeit an.

is:

it:

st:

ao1: (dnatsta): [infield = Staatsangehörigkeit; Staatenliste_DBI] (Dropdown)

ao2: (dnatstao): Präfix: !!An dieser Stelle können Sie Ihre Staatsangehörigkeit auch offen angeben:!! [offene Angabe; 60 Zeichen]

mv:

ka:

vc1: SHOW q1 if dnatderw=2 and dnatausl=0

vc2: SHOW q2 if dnatderw=3 and dnatausl=0

vc3: SHOW q3 if dnatdeu=1 AND dnatausl=1

vc4: SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo: Das Präfix bei ao2 ("An dieser Stelle können Sie Ihre Staatsangehörigkeit auch offen angeben:") bitte linksbündig und in fett oberhalb des offenen Eingabefeldes platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_5"/>
        </zofar:transitions>

hi: Dropdown bitte nach Angabe des Kontinents in A_3 (dnatko) vorselektieren.

\------------------------------------------------------------

A_5
====

tc:

vn: dgebort

qt: Einfachauswahl mit vertikalen ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_6" condition="zofar.asNumber(dgebort)==2"/>
            <zofar:transition target="A_9a" condition="(zofar.asNumber(dgebort)==1 or zofar.isMissing(dgebort)) and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_9b" condition="(zofar.asNumber(dgebort)==1 or zofar.isMissing(dgebort)) and zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_6
====

tc:

vn: dgebko

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: In welchem Land wurden Sie geboren?

is: Bitte wählen Sie zunächst den Kontinent aus.

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

        <zofar:transitions>
            <zofar:transition target="A_7"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_7
====

tc:

vn: dgebsta; dgebstao

qt: Dropdown; offene Angabe

hl:

in:

q: Bitte geben Sie nun das Land an, in dem Sie geboren sind.

is:

it:

st:

ao1: (dgebsta): [infield = Geburtsland; Staatenliste_DBI] (Dropdown)

ao2: (dgebstao): Präfix: !!An dieser Stelle können Sie Ihr Geburtsland auch offen angeben:!! [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Das Präfix bei ao2 ("An dieser Stelle können Sie Ihr Geburtsland auch offen angeben:") bitte linksbündig und in fett oberhalb des offenen Eingabefeldes platzieren.

tr: 

        <zofar:transitions>
            <zofar:transition target="C3_1"/>
        </zofar:transitions>

hi: Dropdown bitte nach Angabe des Kontinents in A_6 (dgebko) vorselektieren.

\------------------------------------------------------------

A_8
===

tc:

vn: baufgru (baufgrueuba; baufgrustuba; baufgruerwerb; baufgrutouba; baufgruasylba; baufgrufaman; baufgrufamba; baufgruausba; baufgruandba; baufgruandbao)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Für die Einreise nach Deutschland gibt es unterschiedliche rechtliche Grundlagen. Wie war das bei Ihnen? #{layout.BREAK}#{layout.BREAK }
Als ich nach Deutschland kam, war ich:

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (baufgrueuba): Bürger\*in eines EU-Mitgliedstaates bzw. des europäischen Wirtschaftsraums

ao2: (baufgrustuba): Studierende\*r (auch zur Studienvorbereitung)

ao3: (baufgruerwerb): Erwerbstätige\*r (Arbeitsvisum)

ao4: (baufgrutouba): Tourist\*in (Besuchsvisum)

ao5: (baufgruasylba): Asylbewerber\*in, Geflüchtete\*r oder Schutzsuchende\*r

ao6: (baufgrufaman): Familienangehörige\*r, kam mit Eltern bzw. mit/wegen (Ehe-)Partner\*in

ao6: (baufgrufamba): Familiennachzug, zog zu bereits in Deutschland lebender Familie

ao6: (baufgruausba): (Spät-)Aussiedler\*in

ao7: (baufgruandba): Anderer Status, und zwar: [(baufgruandbao); offene Angabe, 80 Zeichen]

ato:

mv:

ka:

vc:

av:

kh:

fv:

hv: 

fo: "Als ich nach Deutschland kam, war ich:" bitte etwas von den beiden Einleitungssätzen in der question absetzen.

tr: 

        <zofar:transitions>
            <zofar:transition target="A_8a" condition="baufgruasylba.value"/>
            <zofar:transition target="A_8b" condition="!baufgruasylba.value and (baufgrufaman.value or baufgrufamba.value)"/>
            <zofar:transition target="A_9a" condition="(!baufgruasylba.value and !baufgrufaman.value and !baufgrufamba.value) and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_9b" condition="(!baufgruasylba.value and !baufgrufaman.value and !baufgrufamba.value) and zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:


\------------------------------------------------------------

A_8a
=========

tc:

vn: asylantrag

qt: Einfachauswahl mit vertikalen ao

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

tr: 

        <zofar:transitions>
            <zofar:transition target="A_8b" condition="baufgrufaman.value or baufgrufamba.value"/>
            <zofar:transition target="A_9a" condition="(!baufgrufaman.value and !baufgrufamba.value) and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_9b" condition="(!baufgrufaman.value and !baufgrufamba.value) and zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_8b
=========

tc:

vn: intgrundhl; intgrunddl

qt: offene Angaben

hl:

in:

q: Was waren die Gründe dafür, dass Sie bzw. Ihre Familie ...

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_9a" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_9b" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_9b
=========

tc:

vn: demosex; demosexo

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Welches Geschlecht haben Sie?

is:

it:

st:

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: divers

ao4: 4: Keine der genannten Kategorien, sondern: [(demosexo); 50 Zeichen] (offene Angabe)

vc:

av:

kh:

fv:

hv:

fo: ao4 bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="A_10"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_10
=========

tc:

vn: demoage

qt: offene Angabe

hl:

in:

q: Wie alt sind Sie?

is:

it:

st:

ao: [offene Angabe; Number, 2-stellig: 15 TO 99], Postfix: Jahre 

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihr Lebensalter an (15 bis 99).

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_11"/>
        </zofar:transitions>

hi: 

\------------------------------------------------------------

A_11
=========

tc:

vn: demofam (demofamsin; demofampar; demofamehe; demofamaus; demofamtod; demofamka)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Welchen Familienstand haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (demofamsin): ohne feste\*n Partner\*in

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_12"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_12
=========

tc:

vn: dkinja

qt: Einfachauswahl mit vertikalen ao

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

tr: 

        <zofar:transitions>
            <zofar:transition target="A_13" condition="zofar.asNumber(dkinja)==1"/>
            <zofar:transition target="C1_1" condition="zofar.asNumber(dkinja)==2"/>
            <zofar:transition target="A_13" condition="zofar.isMissing(dkinja)"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_12a
=========

tc:

vn: dsib; dsibo

qt: Einfachauswahl mit vertikalen ao und offener Angabe

hl:

in:

q: Haben Sie Geschwister?

is: Bitte geben Sie auch Ihre Halb- und Stiefgeschwister an.

it:

st:

ao1: (dsib): 1: nein

ao2: (dsib): 2: Ja, und zwar: ([dsibo], NUMBER, 2-Steller)

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

A_12b
=========

tc:

vn: dsibageo1; dsibsex1; dsibageo2; dsibsex2; dsibageo3; dsibsex3
 
qt: Offene Angabe und Dropdown

hl:

in:

q1: Wie alt ist Ihr Geschwisterteil und welches Geschlecht hat Ihr Geschwisterteil?

q2: Wie alt sind Ihre Geschwister und welches Geschlecht haben Ihre Geschwister jeweils?

is: Sollten Sie mehr als drei Geschwister haben, so nennen Sie uns bitte Ihre drei zeitlich nahestehendsten Geschwister. 


it1: (dsibageo1): ([offene Angabe]; infield = Alter; NUMBER, 2-Steller); Suffix: Jahre
it2: (dsibsex1): (infield = Geschlecht; männlich, weiblich, divers)  (Dropdown)

it3: (dsibageo2): ([offene Angabe]; infield = Alter; NUMBER, 2-Steller); Suffix: Jahre
it4: (dsibsex2): (infield = Geschlecht; männlich, weiblich, divers) (Dropdown)

it5: (dsibageo3): ([offene Angabe]; infield = Alter; NUMBER, 2-Steller); Suffix: Jahre
it6: (dsibsex3): (infield = Geschlecht; männlich, weiblich, divers) (Dropdown)

st:

aox: 0: Geschlecht 

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: divers

mv:

ka1: (it1-it2): Geschwisterteil:

ka2: (it1-it2): 1. Geschwisterteil:

ka3: (it3-it4): 2. Geschwisterteil:

ka4: (it5-it6): 3. Geschwisterteil:

vc1: SHOW q1 AND ka1 AND it1-it2 IF dsibo = 1

vc2: SHOW q2 AND ka2-ka3 AND it1-it4 IF dsibo = 2

vc2: SHOW q2 AND ka2-ka4 AND it1-it6 IF dsibo = 3

vc3: SHOW q2 AND is AND ka2-ka4 AND it1-it6 IF dsibo > 3

av:

kh: Bitte geben Sie das Lebensalter an (0 bis 99).

fv:

hv:

fo:

tr:
    
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

ka: (ao2 TO ao3): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: "Ja, und zwar:" über ao2 linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_14" condition="zofar.asNumber(pflegang)==2"/>
            <zofar:transition target="A_15"/>
        </zofar:transitions>

hi:

\--------------------------------

A_14
==

tc: IF pflegang1=1 OR pflegang2=1

vn: pflegt (pflegt1; pflegt2; pflegt3; pflegt4; pflegt5; pflegt5o)

qt: Einfachauswahlmatrix mit horizontalen ao

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

it5: (pflegt5): Etwas anderes, und zwar: [(pflegt5o); 80 Zeichen] (offene Angabe)

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_15"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_15
=========

tc:

vn: gbeges; gartmob; gartseh; gartohr; gartspr; gartpsy; gartsom; garttls; gartson; gartsono; gartka; h_gartcount

qt: Mehrfachauswahl mit vertikalen ao

hl:

in: Im Folgenden stellen wir Ihnen einige kurze Fragen zu möglichen Beeinträchtigungen. Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu.

q: Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (gbeges): keine [Exklkusivkategorie]

ao2: (gartmob): Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

ao3: (gartseh): Blindheit/Sehbeeinträchtigung

ao4: (gartohr): Gehörlosigkeit/Hörbeeinträchtigung

ao5: (gartspr): Sprechbeeinträchtigung (z. B. Stottern)

ao6: (gartpsy): psychische Erkrankung (z. B. Depression, Essstörung)

ao7: (gartsom): körperlich länger dauernde/chronische Krankheit (z. B. Rheuma, MS, Darmerkrankung)

ao8: (garttls): Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

ao9: (gartson): andere Beeinträchtigung/Erkrankung (z. B. Tumorerkrankung, Autismus-Spektrum-Störung): [(gartsono), 50 Zeichen]

ao10: (gartka): Ich möchte die Form meiner Beeinträchtigung nicht nennen. 

mv:

ka: (ao2 TO ao10): Ja, und zwar:

vc:

av:

kh:

fv:

hv: 

fo1: Bitte lediglich die Frage ("Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?") fetten und etwas vom Einleitungstext absetzen. Der Einleitungstext sollte nicht fett sein.

fo2: Bitte über ao2 "Ja, und zwar:" linksbündig positionieren.

fo3: ao10 bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="C2_1" condition="gartmob.value or gartseh.value                or gartohr.value or gartspr.value                or gartpsy.value or gartsom.value                or garttls.value or gartson.value                or gartka.value"/>
            <zofar:transition target="A_16"/>
        </zofar:transitions>

hi: Bitte die Systemvariable h_gartcount erzeugen. Diese soll die Anzahl an genannten beeinträchtigungen abbilden (sum ao2-ao10 bzw. sum gartmob-gartka)

\------------------------------------------------------------

A_16
=========

tc:

vn: imausl

qt: Einfachauswahl mit vertikalen ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_17"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemfs

qt: offene Angabe

hl:

in:

q: Im wievielten Fachsemester befinden Sie sich zurzeit?

is: Fachsemester sind die Semester, die Sie in Ihrem derzeitigen Studiengang eingeschrieben sind.

it:

st:

ao: Präfix: Fachsemester: [offene Angabe; Number, 2-stellig: 1 TO 99]

mv:

ka:

vc: 

av: 

kh: Bitte geben Sie die Anzahl Ihrer Fachsemester an (1 bis 99).

fv:

hv:

fo: Bitte diese Frage zusammen mit den beiden Folgefrage auf einer Seite (A17) darstellen. Fragetext, Ausfüllanweisung und ao der vorliegenden Frage bitte zusammen oberhalb von den beiden nachhfolgenden Fragen platzieren.


tr: 

hi: 

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemhs

qt: offene Angabe

hl:

in:

q: Im wievielten Hochschulsemester befinden Sie sich zurzeit?

is: Hochschulsemester sind alle Semester seit Beginn des Studiums, einschließlich Urlaubs-, Auslands- und Praxissemester.

it:

st:

ao: Präfix: Hochschulsemester: [offene Angabe; Number, 2-stellig: 1 TO 99]

mv:

ka:

vc:

av: 

kh: Bitte geben Sie die Anzahl Ihrer Hochschulsemester an (1 bis 99).

fv:

hv:

fo: Bitte diese Frage zusammen mit der vorherigen Frage und der Folgefrage auf einer Seite (A17) darstellen. Fragetext, Ausfüllanweisung und ao der vorliegenden Frage bitte zusammen zwischen der vorherigen Frage und der nachhfolgenden Frage platzieren.

tr:

hi: 

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

fo: Bitte diese Frage zusammen mit den beiden vorhergehenden Fragen auf einer Seite (A17) darstellen. Fragetext, Ausfüllanweisung und ao der vorliegenden Frage bitte zusammen unterhalb von den beiden vorhergehenden Fragen platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_19" condition="zofar.asNumber(PRELOADhs_id)==0"/>
            <zofar:transition target="A_18"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_18
=======

tc:

vn: hsstand

qt: Einfachauswahl mit vertikalen ao und Dropdown

hl:

in:

q: Wir haben Sie über die [Preload-Token: Hochschulname] angeschrieben. Ist das die Hochschule, an der Sie aktuell studieren?

is: Falls Sie aktuell an einer anderen Hochschule studieren, wählen Sie bitte “Nein” aus. #{layout.BREAK }
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

        <zofar:transitions>
            <zofar:transition target="D2_1" condition="!hsstand_2.value and             (zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_22" condition="!hsstand_2.value and             (zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==13)"/>
            <zofar:transition target="A_19" condition="hsstand_2.value"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_19
=======

tc: IF hsstand_2=1

vn: hsstandbl

qt: Dropdown

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

        <zofar:transitions>
            <zofar:transition target="A_20" condition="zofar.asNumber(hsstandbl) lt 17"/>
            <zofar:transition target="A_21" condition="zofar.asNumber(hsstandbl) == 17"/>
        </zofar:transitions>

hi: 

\------------------------------------------------------------

A_20
=======

tc:

vn: sabserhs

qt: Dropdown

hl:

in: 

q: An welcher Hochschule studieren Sie aktuell?

is: 

it: (sabserhs): [infield = Hochschule] (Dropdown) 

st:

ao: nach Bundesland vorselektierte Dropdown-Hochschulliste

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
            <zofar:transition target="D2_1" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="A_22" condition="zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

hi: Dropdown-Hochschulliste bitte nach Bundesland vorselektieren.

\------------------------------------------------------------

A_20
=======

tc: 

vn: hsstandhso

qt: offene Angabe

hl:

in: 

q: Sollte Ihre Hochschule nicht aufgeführt sein, tragen Sie diese bitte hier ein (z. B. HU Berlin, FH Bielefeld).

it: 

st:

ao: (hsstandhso): [infield = Name der Hochschule; 60 Zeichen] (offene Angabe)

mv: 

ka: 

av: 

kh: 

fv: 

hv: 

fo: Bitte diese Frage zusammen mit der vorhergehenden Frage auf einer Seite (A20) darstellen. Fragetext und ao der vorliegenden Frage bitte zusammen unterhalb  der vorhergehenden Fragen platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D2_1" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="A_22" condition="zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

hi: 

\------------------------------------------------------------

A_21
=======

tc: IF hsstandbl=17 (wenn Studierende an einer ausländ. HS studieren)

vn: hsstandlao; hsstandhsao

qt: offene Angaben

hl:

in: 

q: An welcher Hochschule studieren Sie aktuell?

is: 

it: 

st:

ao1: (hsstandlao): Präfix: Land: [offene Angabe; 100 Zeichen]

ao2: (hsstandhsao): Präfix: Hochschule: [offene Angabe; 100 Zeichen]

mv: 

ka: 

av: 

kh: 

fv: 

hv: 

fo: 

tr:

        <zofar:transitions>
            <zofar:transition target="D2_1" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="A_22" condition="zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

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

ao1: 1: sehr unzufrieden

ao2: 2

ao3: 3

ao4: 4

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
            <zofar:transition target="D1_17" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="D2_13" condition="zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12"/>
            <zofar:transition target="A_23" condition="zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>
    
hi:

\------------------------------------------------------------

A_23
=========

tc:

vn: sfach1o2; sfach2o2

qt: offene Angaben

hl:

in:

q: Bitte geben Sie Ihr Studienfach an.

is: Bitte schreiben Sie das Studienfach aus (z. B. Wirtschaftsinformatik, Soziale Arbeit).

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_24"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_24
=========

tc:

vn: sabslaja

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Sind Sie in einem Lehramtsstudiengang eingeschrieben?

is:

it:

st:

ao1: 1: nein

ao2: 2: ... Grundschulen (Primarstufe)

ao3: 3: ... Haupt-, Real- und Sekundar-/Mittelschulen (Sekundarstufe I)

ao4: 4: ... Gymnasien und Gesamtschulen (Sekundarstufe II)

ao5: 5: ... beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: ... Förderschulen/Sonderpädagogik

mv:

ka: (ao2 TO ao6): Ja, und zwar Lehramt an ...

vc:

av:

kh:

fv:

hv:

fo: Bitte über ao2 "Ja, und zwar:" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_25"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_25
=========

tc:

vn: sabsano; sabsanoaa; sabsanoka

qt: Einfachauswahl mit vertikalen ao und offenen Angaben

hl:

in:

q: Und welchen Abschluss streben Sie als nächstes an?

is: Sollten Sie mehrere Abschlüsse anstreben, beziehen Sie sich bitte auf den zeitlich nächsten.

it:

st:

ao1: (sabsano): 1: Bachelor

ao2: (sabsano): 2: Master

ao3: (sabsano): 3: Staatsexamen

ao4: (sabsano): 4: Diplom

ao5: (sabsano): 5: Promotion

ao6: (sabsano): 6: kirchliche Abschlussprüfung

ao7: (sabsano): 7: künstlerische Abschlussprüfung

ao8: (sabsano): 8: Anderen Abschluss (bspw. ausländischer Abschluss, Magister), und zwar: [(sabsanoaa), offene Angabe, 80 Zeichen]

ao9: (sabsano): 9: Keinen Studienabschluss, sondern: [(sabsanoka), offene Angabe, 80 Zeichen]

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
            <zofar:transition target="A_26" condition="zofar.asNumber(sabsan)==9"/>
            <zofar:transition target="D1_13" condition="zofar.asNumber(sabsan) lt 9 and             (zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_27" condition="zofar.asNumber(sabsan) lt 9 and             (zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)"/>
            <zofar:transition target="D1_13" condition="zofar.isMissing(sabsan) and             (zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_27" condition="zofar.isMissing(sabsan) and             (zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)"/>
        </zofar:transitions>
	
hi:


\------------------------------------------------------------

A_25b
=========

tc:

vn: sabsanpr

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Sie haben angegeben, dass Sie die Promotion anstreben: Sind Sie darüber hinaus in einem regulären Studiengang eingeschrieben?

is: 

it:

st:

ao1: (sabsanpr): -11: nein


ao2: (sabsanpr): 1: Bachelor

ao3: (sabsanpr): 2: Master

ao4: (sabsanpr): 3: Staatsexamen

ao5: (sabsanpr): 4: Diplom

ao7: (sabsanpr): 6: kirchliche Abschlussprüfung

ao8: (sabsanpr): 7: künstlerische Abschlussprüfung

ao9: (sabsanpr): 8: Anderer Abschluss (bspw. ausländischer Abschluss, Magister)

mv:

ka: (ao2 to ao9): Ja, und zwar: 

vc:

av:

kh:

fv:

hv:

fo:  "Ja, und zwar:" über ao2 linksbündig positionieren.

tr:

hi:


\------------------------------------------------------------

A_27
=========

tc:

vn: sform (sformpraes; sformfern; sformdua; sformberu; sformgast; sformsons; sformsonso)


qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Um welche Form handelt es sich bei Ihrem Studium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (sformpraes): Präsenzstudium (im Gegensatz zu Fernstudium)
ao2: (sformfern): Fernstudium
ao3: (sformdua): duales Studium
ao4: (sformberu): berufsbegleitendes Studium
ao5: (sformgast): Gasthörerschaft
ao6: (sformsons): Anderes, und zwar: [(sformsonso), offene Angabe, 60 Zeichen]

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
            <zofar:transition target="D2_3" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="B1_7" condition="zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==13"/>
            <zofar:transition target="A_28" condition="zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_9 
==

tc:

vn: sartzeit

qt: Einfachauswahl mit vertikalen ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="D1_7" condition="(zofar.asNumber(ssemhs) le 5 or             zofar.asNumber(ssemhs) le 6)"/>
            <zofar:transition target="D1_7" condition="zofar.isMissing(ssemhs)"/>
            <zofar:transition target="D2_6" condition="zofar.asNumber(ssemhs) ge 7 and             (zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_44" condition="zofar.asNumber(ssemhs) ge 7 and             (zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10)"/>
        </zofar:transitions>

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

ao1: (spernot): Präfix: Durchschnittsnote (z. B. 2,5): [(spernoto): Number, 3-stellig: 1,0 TO 5,0]

ao2: (spernot): -11: Ich habe bisher keine Noten erhalten.

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihre aktuelle Durchschnittsnote an (1,0 bis 5,0)

fv:

hv:

fo: Bitte offene Angabe und Einfachauswahl untereinander, linksbündig positionieren

tr:

        <zofar:transitions>
            <zofar:transition target="A_29"/>
        </zofar:transitions>

hi: Offene Angabe bitte als NUMBER mit einer Dezimalstelle (1,0 bis 5,0), programmieren.

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_30"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_31
=========

tc:

vn: studerfolg; masterfolg; promoerfolg

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit trauen Sie sich zu, …

is:

it1: (studerfolg): … Ihr Studium erfolgreich abzuschließen?

it2: (masterfolg): … ein Masterstudium erfolgreich abzuschließen?

it3: (promoerfolg): … eine Promotion (Dr., PhD) erfolgreich abzuschließen?

st:

ao1: 1: überhaupt nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: vollkommen

mv:

ka:

vc: SHOW it2 IF sabsano = 1

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_32"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_32
=========

tc:

vn: deltberuv; deltberum

qt: Einfachauswahl mit vertikalen ao im Spaltenformat/Comparison

hl:

in:

q: Welches ist der höchste berufliche Abschluss Ihres Vaters/Ihrer Mutter?

is:

it1: (deltberuv): Vater

it2: (deltberum): Mutter

st:

ao1: 7: Promotion (Dr., PhD)

ao2: 6: Universitätsabschluss

ao3: 5: Fachhochschulabschluss

ao4: 4: Abschluss an einer Meister-, Techniker-, Fachschule

ao5: 3: Lehre bzw. Facharbeiterabschluss, Abschluss an einer Berufsfach-, Handels-, Berufsaufbauschule

ao6: 2: anderer beruflicher Abschluss

ao7: 1: hat keinen beruflichen Abschluss

mv: -12: weiß ich nicht 

ka:

vc:

av:

kh:

fv:

hv:

fo1: mv/"weiß ich nicht" bitte etwas absetzen.

fo2: "Vater" und Mutter bitte jeweils als Spaltenüberschrift.

tr:

        <zofar:transitions>
            <zofar:transition target="A_33" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="B2_1" condition="zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_33
=========

tc:

vn: deltjobv (deltjobvo1; deltjobv1; deltjobv2); deltjobm (deltjobmo1; ddeltjobm1; deltjobm2)

qt: offene Angaben; Einfachauswahl;

hl:

in:

q: Und welchen Beruf übt Ihr Vater/Ihre Mutter hauptberuflich aus?

is: Falls Ihre Eltern zurzeit nicht erwerbstätig sind, geben Sie bitte den jeweils zuletzt ausgeübten Beruf an.

Bitte tragen Sie die Berufsbezeichnung möglichst genau ein, z. B.:
Bankkauffrau oder -mann (nicht: Angestellte\*r), Zollbeamtin oder -beamter (nicht: Beamtin oder Beamter), Maschinenbauingenieur\*in (nicht: Ingenieur\*in).


it1: Vater

it2: Mutter

ao1: (deltjobvo1): Präfix: Berufsbezeichnung: [offene Angabe; 100 Zeichen]

ao2: (deltjobv1): -11: nie berufstätig gewesen [Einfachauswahl]

ao3: (deltjobv2): -12: weiß ich nicht [Exklusivkategorie]

ao4: (deltjobmo1): Präfix: Berufsbezeichnung: [offene Angabe; 100 Zeichen]

ao5: (deltjobm1): -11: nie berufstätig gewesen [Einfachauswahl]

ao6: (deltjobm2): -12: weiß ich nicht [Exklusivkategorie]

ka:

vc:

av:

kh:

fv:

hv:

fo: „Vater“ und „Mutter“ bitte jeweils in einer extra Zeile positionieren, die linksbündig über den jeweils darunterliegenden Antwortzeilen liegt (siehe Darstellung hierunter):

Vater
Berufsbezeichnung: Eingabefeld
nie berufstätig gewesen-Kästchen
weiß ich nicht-Kästchen

Mutter
Berufsbezeichnung: Eingabefeld
nie berufstätig gewesen-Kästchen
weiß ich nicht-Kästchen


tr:

        <zofar:transitions>
            <zofar:transition target="B2_2a" condition="(zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="B2_2b" condition="(zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="B1_6" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6"/>
            <zofar:transition target="A_34" condition="zofar.asNumber(mastersplit)==14"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_34
=========

tc:

vn: deltgebv; deltgebm

qt: Einfachauswahl mit vertikalen ao im Spaltenformat/Comparison

hl:

in:

q: Wo wurden Ihre Eltern geboren?

is:

it1 (deltgebv): Vater

it2 (deltgebm): Mutter

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

fo: "Vater" und Mutter bitte jeweils als Spaltenüberschrift.

tr:

        <zofar:transitions>
            <zofar:transition target="A_35" condition="zofar.asNumber(deltgebv)==2 or zofar.asNumber(deltgebm)==2"/>
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
        </zofar:transitions>
    
hi:

\------------------------------------------------------------

A_35
=====

tc: IF deltgebv=2 

vn: deltgkov

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: In welchem Land wurde Ihr Vater geboren?

is: Bitte wählen Sie zunächst den Kontinent aus.

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

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: In welchem Land wurde Ihre Mutter geboren?

is: Bitte wählen Sie zunächst den Kontinent aus.

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

fo: Bitte diese Frage zusammen mit der vorhergehenden Frage auf einer Seite (A35) darstellen. Fragetext, Ausfüllanweisung und ao der vorliegenden Frage bitte zusammen unterhalb der vorhergehenden Frage platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_36"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstav; deltgstavo

qt: Dropdown; offene Angabe

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihres Vaters an.

is:

it:

st:

ao1: (deltgstav): [infield = Geburtsland Vater; Staatenliste_DBI] (Dropdown)

ao2: (deltgstavo): Präfix: An dieser Stelle können Sie das Geburtsland auch offen angeben: [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi: Dropdown bitte nach Angabe des Kontinents in A_35 (deltgkov) vorselektieren.

\------------------------------------------------------------

A_36
=====

tc:

vn: deltgstam; deltgstamo

qt: Dropdown; offene Angabe

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihrer Mutter an.

is:

it:

st:

ao1: (deltgstam): [infield = Geburtsland Mutter; Staatenliste_DBI] (Dropdown)

ao2: (deltgstamo): Präfix: An dieser Stelle können Sie das Geburtsland auch offen angeben: [offene Angabe; 60 Zeichen]

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo: Bitte diese Frage zusammen mit der vorhergehenden Frage auf einer Seite (A36) darstellen. Fragetext und ao der vorliegenden Frage bitte zusammen unterhalb der vorhergehenden Frage platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="C3_2"/>
        </zofar:transitions>

hi: Dropdown bitte nach Angabe des Kontinents in A_35 (deltgkom) vorselektieren.

\------------------------------------------------------------

A_37a
========

tc:

vn: vsbplz; vsbort

qt: offene Angabe

hl:

in:

q: An welchem Ort haben Sie gewohnt, als Sie die Studienberechtigung (HZB) erhalten haben?

it:

st:

ao1: (vsbplz): Präfix: Bitte tragen Sie die fünfstellige Postleitzahl ein: [Infield = Postleitzahl; Number, 5-stellig: 01000 TO 99999] (offene Angabe)

ao2: (vsbort): Präfix: Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an: [Infield = Ort; 60 Zeichen] (offene Angabe)

mv:

ka:

vc:

av: 

kh:

fv: 

hv:

fo: Bitte jeweils zwischen den Präfixen und den Feldern für die offenen Angaben einen Zeilenumbruch einfügen (Präfixe also über den Feldern positionieren). Alles linksbündig untereinander anordnen.

tr:

        <zofar:transitions>
            <zofar:transition target="A_41"/>
        </zofar:transitions>

hi: Besteht die Möglichkeit, dass bei PLZ mit einer 0 vorne, diese nicht gelöscht wird?

\------------------------------------------------------------

A_38a
==========

tc:

vn: intbild (intbild1; intbild2; intbild3; intbild4; intbild5; intbild6; intbild7)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Welche Bildungsabschlüsse hatten Sie bereits, als Sie nach Deutschland kamen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intbild1): Promotion (Dr., PhD)

ao2: (intbild2): Hochschulstudium mit zweitem Abschluss (z. B. Master)

ao3: (intbild3): Hochschulstudium mit erstem Abschluss (z. B. Bachelor)

ao4: (intbild4): begonnenes Hochschulstudium ohne Abschluss

a05: (intbild5): Schulabschluss, der zum Studium berechtigt

ao6: (intbild6): Schulabschluss ohne Studienberechtigung

ao7: (intbild7): keinen Schulabschluss

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
            <zofar:transition target="A_38b" condition="(intbild1.value                 or intbild2.value                 or intbild3.value                 or intbild4.value                 or intbild5.value)"/>
            <zofar:transition target="A_38c" condition="(intbild6.value                 or intbild7.value)"/>
            <zofar:transition target="A_38c" condition="(!intbild1.value                 and !intbild2.value                 and !intbild3.value                 and !intbild4.value                 and !intbild5.value                 and !intbild6.value                 and !intbild7.value)"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_38b
==========

tc:

vn: ankbild (ankbild1; ankbild2; ankbild3; ankbild4; ankbild5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wurden diese Bildungsabschlüsse bzw. Ihre bisherigen Studienleistungen in Deutschland anerkannt?

is:

it1: (ankbild1): Promotion (Dr., PhD)

it2: (ankbild2): Hochschulstudium mit zweitem Abschluss

it3: (ankbild3): Hochschulstudium mit erstem Abschluss

it4: (ankbild4): Teile meines bisherigen Studiums

it5: (ankbild5): schulische Studienberechtigung

st:

ao1: 1: vollständig anerkannt

ao2: 2: teilweise anerkannt

ao3: 3: nicht anerkannt

mv: -12: weiß ich nicht


ka:

vc1: SHOW it1 if intbild1 > 0
vc2: SHOW it2 if intbild2 > 0
vc3: SHOW it3 if intbild3 > 0
vc4: SHOW it4 if intbild4 > 0
vc5: SHOW it5 if intbild5 > 0

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="A_38c"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_38c
==========

tc:

vn: intvors (intvors1; intvors2; intvors3; intvors4; intvors5; intvors5o; intvors6)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Welche zusätzlichen Voraussetzungen mussten Sie für ein Studium in Deutschland erfüllen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (intvors1): Feststellungsprüfung

ao2: (intvors2): Nachweis deutscher Sprachkenntnisse (z. B. TestDaF, DSH)

ao3: (intvors3): Nachweis englischer Sprachkenntnisse (z. B. Cambridge FCE, TOEFL, IELTS)

ao4: (intvors4): fachliche Eignungsprüfung (z. B. TestAS, Medizin, Kunst, Musik, Sport)

ao5: (intvors5): Etwas anderes, und zwar: [(intvors5o), offene Angabe, 250 Zeichen]

ao6: (intvors6): Keine [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: ao6 als Exklusivkategorie bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="D1_2" condition="(zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_40"/>
        </zofar:transitions>

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

a07: 7: keinen Abschluss

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
            <zofar:transition target="A_39"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_39
==========

tc:

vn: vsbtyp (vsbtyp1; vsbtyp2; vsbtyp3; vsbtyp4; vsbtyp5; vsbtyp6; vsbtyp7; vsbtyp8; vsbtyp9; vsbtyp9o, vsbtyp10; vsbtyp11; vsbtyp12; vsbtyp13; vsbtyp14; vsbtyp15; vsbtyp15o)

qt: Mehrfachauswahl mit offener Angabe

hl:

in:

q: Auf welchem Weg haben Sie Ihre Studienberechtigung erhalten (über den schulischen Weg, eine berufliche Qualifikation oder besondere Eignung)?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (vsbtyp1): Gymnasium

ao2: (vsbtyp2): Gesamtschule mit gymnasialer Oberstufe

ao3: (vsbtyp3): freie Waldorfschule

ao4: (vsbtyp4): Abendgymnasium, Kolleg (nicht Berufskolleg)

ao5: (vsbtyp5): Fachgymnasium, berufliches Gymnasium

ao6: (vsbtyp6): Berufsfachschule

ao7: (vsbtyp7): Berufsoberschule

ao8: (vsbtyp8): Fachoberschule

ao9: (vsbtyp9): andere Schulform, und zwar: [(vsbtyp9o); offen Angabe, 80 Zeichen]


ao10: (vsbtyp10): berufliche Aufstiegsfortbildung (z.B. Meister\*in, Techniker\*in, Fachwirt\*in, Erzieher\*in)

ao11: (vsbtyp11): abgeschlossene Berufsausbildung mit anschließender Berufspraxis 


ao12: (vsbtyp12): Eignungsprüfung (z. B. Kunst, Musik, Sport)

ao13: (vsbtyp13): Begabtenprüfung

ao14: (vsbtyp14): Mediziner\*innen-Test (TMS)

ao15: (vsbtyp15): Auf einem anderen Weg, und zwar: [(vsbtyp15o); offen Angabe, 80 Zeichen]

mv:

ka1 (ao1 TO ao9) Schulischer Weg

ka2 (ao10 TO ao11) Berufliche Qualifikation

ka3 (ao12 TO ao15o) Eignungsprüfungen

vc:

av:

kh:

fv:

hv:

fo1: Bitte die Beispiele in Klammern in etwas kleinerer Schriftgröße (2pt kleiner) umsetzen.

fo2: "Schulischer Weg" linksbündig über ao1; "Berufliche Qualifikation" linksbündig über ao10; "Eignungsprüfungen" linksbündig über ao12

tr:

        <zofar:transitions>
            <zofar:transition target="D1_1" condition="(zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==14)                 and (vsbtyp1.value or vsbtyp2.value                  or vsbtyp3.value or vsbtyp4.value                  or vsbtyp5.value or vsbtyp6.value                  or vsbtyp7.value or vsbtyp8.value                  or vsbtyp9.value)"/>
            <zofar:transition target="A_40"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_40
========

tc:

vn: vsbnotej; vsbnoteo; vsbnote

qt: offene Angaben; Einfachauswahl

hl:

in:

q: Wann und mit welcher Note haben Sie ihre Hochschulzugangsberechtigung erlangt?

is: Punktzahl bitte in Note umrechnen.

it:

st:

ao1: (vsbnotej): Präfix: Jahr (z. B. 2017): [offene Angabe, NUMBER, 4-stellig]

ao2: (vsbnoteo): Präfix: Durchschnittsnote (z. B. 2,5): [offene Angabe, NUMBER, 3-stellig mit einer Dezimalstelle]

ao3: (vsbnote): Ich habe keine Note erhalten.

mv:

ka:

vc:

av1: (vsbnotej): NUMBER, 4-stellig (1950 bis 2020)

av2: (vsbnoteo): NUMBER, 3-stellig mit einer Dezimalstelle (1,0 bis 4,0)

kh1: (vsbnotej): Bitte geben Sie die vierstellige Jahreszahl an.

kh2: (vsbnoteo): Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_37a" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_37b" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi1: vsbnotej bitte als NUMBER, 4-stellig (1950 bis 2020) programmieren.

hi2: vsbnoteo bitte als NUMBER, 3-stellig mit einer Dezimalstelle (1,0 bis 4,0) programmieren.

\------------------------------------------------------------

A_41
===========

tc:

vn: vausbja

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor dem Studium eine Berufsausbildung/berufliche Aufstiegsfortbildung abgeschlossen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: 1: nein

ao2: 2: ja, eine Berufsausbildung abgeschlossen

ao3: 3: ja, eine berufliche Aufstiegsfortbildung abgeschlossen

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
            <zofar:transition target="A_42" condition="zofar.asNumber(vausbja)==1                or zofar.isMissing(vausbja)"/>
            <zofar:transition target="D1_5" condition="zofar.asNumber(vausbja)==2               and (zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D1_4" condition="zofar.asNumber(vausbja)==3               and (zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_42" condition="(zofar.asNumber(vausbja)==2 or zofar.asNumber(vausbja)==3)                and (zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                 or zofar.asNumber(mastersplit)==13)"/>
        </zofar:transitions>

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

is: Mit „Erwerbstätigkeit(en)“ sind sämtliche Tätigkeiten gemeint, mit denen Sie im aktuellen Semester Geld verdienen.

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_43" condition="zofar.asNumber(eaktsens)==2                or zofar.asNumber(eaktsens)==3                or zofar.asNumber(eaktsens)==4"/>
            <zofar:transition target="A_44" condition="zofar.asNumber(eaktsens)==1                and zofar.asNumber(mastersplit)==13"/>
            <zofar:transition target="A_44" condition="zofar.isMissing(eaktsens)               and zofar.asNumber(mastersplit)==13"/>
            <zofar:transition target="D3_20" condition="zofar.asNumber(eaktsens)==1                 and (sformberu.value or sformdua.value)                 and (zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                               or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D3_20" condition="zofar.isMissing(eaktsens)                 and (sformberu.value or sformdua.value)                 and (zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                               or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D3_22" condition="zofar.asNumber(eaktsens)==1                 and (!sformberu.value or !sformdua.value)                 and (zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                               or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D3_22" condition="zofar.isMissing(eaktsens)                 and (!sformberu.value or !sformdua.value)                 and (zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                               or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D1_9" condition="zofar.asNumber(eaktsens)==1               and (zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8)"/>
            <zofar:transition target="D1_9" condition="zofar.isMissing(eaktsens)               and (zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8)"/>
        </zofar:transitions>

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

ao2: 2: ja, an meiner aktuellen Hochschule

ao3: 3: ja, an einer anderen Hochschule 

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
            <zofar:transition target="A_49a" condition="zofar.asNumber(sabsja)==1               and zofar.asNumber(sabser)==1"/>
            <zofar:transition target="A_49b" condition="zofar.asNumber(sabsja)==1               and zofar.asNumber(sabser)!=1"/>
            <zofar:transition target="A_45" condition="zofar.asNumber(sabsja)==2"/>
            <zofar:transition target="A_49a" condition="zofar.isMissing(sabsja) and               zofar.asNumber(sabser)==1"/>
            <zofar:transition target="A_49b" condition="zofar.isMissing(sabsja) and               zofar.asNumber(sabser)!=1"/>
        </zofar:transitions>
    
hi:

\------------------------------------------------------------

A_45
===========

tc: sabsja=2 OR sbsja=3

vn: sabszp; sabszp2

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Wann haben Sie diesen Abschluss erworben?

is:

it1: (sabszp): [infield = Monat; Januar - Februar - März - ... - Dezember] (Dropdown)

it2: (sabszp2): [infield = Jahr; 2020 - 2019 - 2018 - ... - 2009 und früher] (Dropdown)

st:

ao: 

aox: (sabszp): Monat

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


aox: (sabszp2): Jahr

ao1: (sabszp2): 1: 2020

ao2: (sabszp2): 2: 2019

ao3: (sabszp2): 3: 2018

ao4: (sabszp2): 4: 2017

ao5: (sabszp2): 5: 2016

ao6: (sabszp2): 6: 2015

ao7: (sabszp2): 7: 2014

ao8: (sabszp2): 8: 2013

ao9: (sabszp2): 9: 2012

ao10: (sabszp2): 10: 2011

ao11: (sabszp2): 11: 2010

ao12: (sabszp2): 12: 2009 und früher

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Dropdowns bitte nebeneinander programmieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_46"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_46
=========

tc: sabsja=2 OR sbsja=3

vn: sabser

qt: Einfachauswahl

hl:

in:

q: Welchen Abschluss haben Sie bereits erworben?

is: Bei mehreren Hochschulabschlüssen bitte den zuletzt erworbenen angeben.

it:

st:

ao1: 1: Bachelor

ao2: 2: Master

ao3: 3: Staatsexamen

ao4: 4: Diplom

ao5: 5: Promotion (Dr., PhD)

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_47"/>
        </zofar:transitions>
        
hi:

\------------------------------------------------------------

A_47
========

tc: sabsja=2 OR sbsja=3

vn: sabsla

qt: Einfachauswahl

hl:

in:

q: Handelt es sich hierbei um ein Lehramtsstudium?

is:

it:

st:

ao1: 1: nein

ao2: 2: … Grundschulen (Primarstufe)

ao3: 3: … Haupt-, Real- und Sekundar-/Mittelschulen (Sekundarstufe I)

ao4: 4: … Gymnasien und Gesamtschulen (Sekundarstufe II)

ao5: 5: … beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: … Förderschulen/Sonderpädagogik

mv:

ka: (ao2 TO ao6): Ja, und zwar Lehramt an …

vc:

av:

kh:

fv:

hv:

fo: Bitte über ao2 "Ja, und zwar:" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="A_48"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_48
=========

tc: sabsja=2 OR sbsja=3

vn: sabsernot

qt: offene Angabe

hl:

in:

q: Welche Abschlussnote haben Sie in Ihrem vorherigen Studium erhalten?

is: Punktzahl bitte in Note umrechnen.

it:

st:

ao: (sabsernot): Präfix: Abschlussnote (z. B. 2,5): [offene Angabe, NUMBER, 3-stellig mit einer Dezimalstelle]

mv:

ka:

vc:

av: NUMBER, 3-stellig mit einer Dezimalstelle (1,0 bis 4,0)

kh: Bitte geben Sie Ihre Abschlussnote an (1,0 bis 4,0).

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D1_10a" condition="(zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10                 or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_49a" condition="(zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                 or zofar.asNumber(mastersplit)==13)               and (zofar.asNumber(sabsan)==1 or zofar.isMissing(sabsan))"/>
            <zofar:transition target="A_49b" condition="(zofar.asNumber(mastersplit)==5                 or zofar.asNumber(mastersplit)==6                 or zofar.asNumber(mastersplit)==11                 or zofar.asNumber(mastersplit)==12                 or zofar.asNumber(mastersplit)==13)               and zofar.asNumber(sabsan)!=1"/>
        </zofar:transitions>

hi: Bitte als NUMBER, 3-stellig mit einer Dezimalstelle (1,0 bis 4,0) programmieren.

\------------------------------------------------------------

A_49a
=========

tc:

vn: mastplan; promoplan

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie wahrscheinlich ist es, dass Sie …

is:

it1: (mastplan): … ein Masterstudium aufnehmen?

It2: (promoplan) … eine Promotion (Dr., PhD) aufnehmen?

st:

ao1: 1: sehr unwahrscheinlich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wahrscheinlich

mv:

ka:

vc: SHOW it1 (mastplan) IF sabsano==1 

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="KSM-anf01" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(sabsan)==1)             and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="KSM-anf01" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(vsbdeba)==1              or zofar.asNumber(imausl)==1)             and (zofar.asNumber(sabsan)==1)             and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="KSM-ma01" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(sabsan)==1)             and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="KSM-ma01" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(vsbdeba)==1               or zofar.asNumber(imausl)==1)             and (zofar.asNumber(sabsan)==1)             and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="KSM-phd01" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(sabsan)==2             or zofar.asNumber(sabsan)==3             or zofar.asNumber(sabsan)==4             or zofar.asNumber(sabsan)==6             or zofar.asNumber(sabsan)==7             or zofar.asNumber(sabsan)==8           or zofar.isMissing(sabsan))"/>
            <zofar:transition target="KSM-phd01" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(vsbdeba)==1              or zofar.asNumber(imausl)==1)             and (zofar.asNumber(sabsan)==2             or zofar.asNumber(sabsan)==3             or zofar.asNumber(sabsan)==4             or zofar.asNumber(sabsan)==6             or zofar.asNumber(sabsan)==7             or zofar.asNumber(sabsan)==8           or zofar.isMissing(sabsan))"/>
            <zofar:transition target="A_50" condition="zofar.asNumber(zusatzsplit)==1             or zofar.asNumber(zusatzsplit)==3             or zofar.asNumber(zusatzsplit)==4"/>
            <zofar:transition target="A_50" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(vsbdeba)==2              or zofar.asNumber(imausl)==2)"/>
            <zofar:transition target="A_50" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.isMissing(vsbdeba)              or zofar.isMissing(imausl))"/>
            <zofar:transition target="A_50"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_50
=========

tc:

vn: ssweja; saweja; shwja; ssuja

qt: Einfachauswahl Dropdown

hl:

in:

q: Haben Sie seit Ihrer Erstimmatrikulation …

is: Nicht gemeint sind Veränderungen bzw. Unterbrechungen beim Übergang vom Bachelor- ins Masterstudium.

it1: (ssweja): … das Studienfach gewechselt? [infield = Anzahl; keinmal - einmal - ... - fünfmal] (Dropdown)

it2: (saweja): … den Abschluss gewechselt? [infield = Anzahl; keinmal - einmal - ... - fünfmal] (Dropdown)

it3: (shwja): … die Hochschule gewechselt? [infield = Anzahl; keinmal - einmal - ... - fünfmal] (Dropdown)

it4: (ssuja): … das Studium zwischenzeitlich unterbrochen? [infield = Anzahl; keinmal - einmal - ... - fünfmal] (Dropdown)

st:

aox: Anzahl

ao1: (ssweja TO ssuja): 0: keinmal

ao2: (ssweja TO ssuja): 1: einmal

ao3: (ssweja TO ssuja): 2: zweimal

ao4: (ssweja TO ssuja): 3: dreimal

ao5: (ssweja TO ssuja): 4: viermal

ao6: (ssweja TO ssuja): 5: fünfmal

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
            <zofar:transition target="D1_14" condition="(zofar.asNumber(ssweja)==1             or zofar.asNumber(saweja)==1             or zofar.asNumber(shwja)==1             or zofar.asNumber(ssuja)==1)             and (zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_51a" condition="(zofar.asNumber(ssweja)==1             or zofar.asNumber(saweja)==1             or zofar.asNumber(shwja)==1             or zofar.asNumber(ssuja)==1)             and (zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)           and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_51b" condition="(zofar.asNumber(ssweja)==1             or zofar.asNumber(saweja)==1             or zofar.asNumber(shwja)==1             or zofar.asNumber(ssuja)==1)             and (zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13)           and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="A_51a" condition="(zofar.asNumber(ssweja)==2             and zofar.asNumber(saweja)==2             and zofar.asNumber(shwja)==2             and zofar.asNumber(ssuja)==2)             and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_51b" condition="(zofar.asNumber(ssweja)==2             and zofar.asNumber(saweja)==2             and zofar.asNumber(shwja)==2             and zofar.asNumber(ssuja)==2)             and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="A_51a" condition="(zofar.isMissing(ssweja)             and zofar.isMissing(saweja)             and zofar.isMissing(shwja)             and zofar.isMissing(ssuja))             and zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_51b" condition="(zofar.isMissing(ssweja)             and zofar.isMissing(saweja)             and zofar.isMissing(shwja)             and zofar.isMissing(ssuja))             and zofar.asNumber(h_split)==2"/>
            <zofar:transition target="A_51a"/>
        </zofar:transitions>

hi: Bitte für den Infield-Text nicht die "0" als Wert vergeben, da diese bereits für die erste Antwortoption "keinmal" vorgehalten ist.

\------------------------------------------------------------

A_51b
=========

tc:

vn: ssa (ssahswe; ssafawe; ssaunt; ssaaja)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit denken Sie zurzeit daran …

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
            <zofar:transition target="D1_20" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_52" condition="zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_52
=========

tc:

vn: wohnfo

qt: Einfachauswahl

hl:

in:

q1: Wie wohnen Sie während der Vorlesungszeit des aktuellen Semesters hauptsächlich?

is: Wenn Sie ++überwiegend++ bei Ihren Eltern oder Verwandten wohnen, geben Sie bitte die Wohnform Ihrer Eltern bzw. der Verwandten/Bekannten an.

it:

st:

ao1: 1: zur Miete (auch Wohngemeinschaft). 

ao2: 2: zur Untermiete.

ao3: 3: als (Mit-)Eigentümer\*in.

ao4: 4: im Einzelzimmer (Flurgemeinschaft).

ao5: 5: im Einzelzimmer (in einer Wohngruppe).

ao6: 6: im Einzelappartement.

ao7: 7: in einer Mehrzimmerwohnung (für Paare oder Studierende mit Kind).

mv:

ka1: (ao1 TO ao3): In einer Wohnung, einem Zimmer oder einem Haus

ka2: (ao4 TO ao7): Im Studierendenwohnheim

vc: 

av:

kh:

fv:

hv:

fo1: Bitte über ao1 "In einer Wohnung, einem Zimmer oder einem Haus" linksbündig positionieren.

fo2: Bitte über ao4 "Im Studierendenwohnheim" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D3_1" condition="(zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_53" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==13"/>
        </zofar:transitions>

  
hi:

\------------------------------------------------------------

A_53
=========

tc:

vn: wohn (wohnal; wohnwg; wohnel; wohnpar; wohnkin; wohnfam; wohnsons)

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q1: Mit wem wohnen Sie während der Vorlesungszeit überwiegend zusammen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (wohnal): ... alleine. [Exklusivkategorie]

ao2: (wohnwg): ... mit Mitbewohner\*innen in einer Wohngemeinschaft.

ao3: (wohnel): ... bei/mit meinen Eltern (bzw. einem Elternteil)

ao4: (wohnpar): ... mit meinem/meiner (Ehe-) Partner\*in.

ao5: (wohnkin): ... mit meinem Kind/meinen Kindern.

ao6: (wohnfam): ... mit anderen Familienangehörigen.

ao7: (wohnsons): ... mit anderen Personen.

mv:

ka: (ao1 TO ao7):  Ich wohne …

vc:

av:

kh:

fv:

hv:

fo: "Ich wohne …" bitte linksbündig über die erste ao positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D3_2" condition="!wohnal.value and             (zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="D3_4" condition="wohnal.value and             (zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="B2_5" condition="zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==13"/>
            <zofar:transition target="B1_5" condition="zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2"/>
        </zofar:transitions>
  
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

tr:

        <zofar:transitions>
            <zofar:transition target="A_55"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_55
=========

tc:

vn: auslandint

qt: Einfachauswahl

hl:

in:

q1: Haben Sie vor, künftig einen studienbezogenen Auslandsaufenthalt durchzuführen?

q2: Haben Sie vor, künftig einen weiteren studienbezogenen Auslandsaufenthalt durchzuführen?

is:

it:

st:

ao1: 1: nein, kein Interesse

ao2: 2: nein, sehe keine Realisierungschance

ao3: 3: weiß ich noch nicht

ao4: 4: ja, geplant

ao5: 5: ja, bereits in Vorbereitung

mv:

ka:

vc: 

SHOW q1 if ainfaus=1 OR ainfaus=k.A

SHOW q2 if ainfaus=2 OR ainfaus=3 OR ainfaus=4

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="F1_1" condition="zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14"/>
            <zofar:transition target="E1_1" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==1"/>
            <zofar:transition target="KSM-pol01" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==3"/>
            <zofar:transition target="KSM-fai01" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==4"/>
            <zofar:transition target="A_56" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==13)             and zofar.asNumber(zusatzsplit)==2"/>
            <zofar:transition target="A_56" condition="(zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==12             or zofar.asNumber(mastersplit)==14)             and zofar.asNumber(zusatzsplit)==2             and (zofar.asNumber(vsbdeba)==1              or zofar.asNumber(imausl)==1)"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_56
=========

tc:

vn: zlv (zlvwo, zlvwo2); zses (zseswo, zseswo2); zer (zerwo, zerwo2); zcar (zcarwo, zcarwo2); zkb (zkbwo, zkbwo2)

qt: Comparison, offene Angaben-Matrix

hl:

in:

q: Wie viele Stunden wenden Sie in einer für Sie typischen Woche für folgende Aktivitäten auf?

is: Bitte runden Sie Ihre Zeitangaben jeweils auf volle Zeitstunden und unterscheiden Sie bitte zwischen der Vorlesungszeit/Studienphase und der vorlesungsfreien Zeit/Praxisphase.

ita: während Vorlesungszeit/Studienphase

itb: während vorlesungsfreier Zeit/Praxisphase

st:

ao1a: (zlvwo): Lehrveranstaltungen [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao1b: (zlvwo2): Lehrveranstaltungen [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao2a: (zseswo): Selbststudium [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao2b: (zseswo2): Selbststudium [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao3a: (zerwo): Erwerbstätigkeit [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao3b: (zerwo2): Erwerbstätigkeit [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao4a: (zcarwo): Pflege- und Betreuungsarbeiten [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao4b: (zcarwo2): Pflege- und Betreuungsarbeiten [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao5a: (zkbwo): Kinderbetreuung [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao5a: (zkbwo2): Kinderbetreuung [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

mv:

ka:

vc1: SHOW ao3a (zerwo) IF eaktsens=2 OR eaktsens=3 OR eaktsens=4

vc2: SHOW ao3b (zerwo2) IF eaktsens=2 OR eaktsens=3 OR eaktsens=4

vc3: SHOW ao4a (zcarwo) IF pflegang1=1 OR pflegang2=1

vc4: SHOW ao4b (zcarwo2) IF pflegang1=1 OR pflegang2=1

av: NUMBER, 2-stellig (0 bis 99)

kh: Bitte geben Sie volle Zeitstunden an (0 bis 99).

fv:

hv:

fo: Bitte anhand der Unterteilung in a und b die Zuordnung der Items zu den beiden Kategorien ita und itb vornehmen. ita und itb bilden die Spalten und in den Zeilen werden dann die einzelnen Bereiche noch einmal unterteilt (bspw. Lehrveranstaltungen: ao1a -> ita; ao1b -> itb).

tr:

        <zofar:transitions>
            <zofar:transition target="N_1" condition="zofar.asNumber(zusatzsplit)==1"/>
            <zofar:transition target="N_13" condition="zofar.asNumber(zusatzsplit)==4"/>
            <zofar:transition target="N_5" condition="zofar.asNumber(zusatzsplit)==3"/>
            <zofar:transition target="A_57" condition="zofar.asNumber(zusatzsplit)==2"/>
        </zofar:transitions>

hi: Bitte als NUMBER, 2-stellig (0 bis 99) programmieren.


\------------------------------------------------------------

N_1
=========
tc: IF NRW / zusatzsplit ==1

vn: nrwstudium; nrwfach

qt: Einfachauswahlmatrix mit horizontalen ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_2"/>
        </zofar:transitions>

hi:


\------------------------------------------------------------

N_2
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwstudium2

qt: Einfachauswahl mit vertikaler ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_3"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_3
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwfach2

qt: Einfachauswahl mit vertikaler ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_4"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_4
=========

tc: IF NRW / zusatzsplit ==1

vn: nrwregel

qt: Einfachauswahl mit vertikaler ao

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_57"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_5
=========

tc: IF zusatzsplit == 3

vn: nrwdigbed

qt: Einfachauswahl mit vertikaler ao

hl:

in:

q: Wie schätzen Sie Ihren Bedarf an digitalen Studienangeboten in Ihrem Studiengang ein?

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_6"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_6
=========

tc:

vn: nrwdigged

qt: Einfachauswahl mit vertikaler ao

hl:

in:

q: In welchem Maße wird Ihr Bedarf an digitalen Selbstlernangeboten durch die Hochschule abgedeckt?

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_7"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_7
=========

tc:

vn: nrwselbtest

qt: Einfachauswahl mit vertikaler ao

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

ao6: -13: Test nicht durchgeführt/angeboten

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo: ao6 (missing) bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="N_8"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_8
=========

tc:

vn: nrwstudipor

qt: Einfachauswahl mit vertikaler ao

hl:

in:

q: Haben Sie zu Studienbeginn die E-Learning-Angebote im landesweiten Onlineportal "Studiport" genutzt? Halten Sie rückblickend diese 
E-Learning-Angebote für hilfreich?

is:

it:

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in sehr hohem Maße

ao6: -13: Angebot nicht bekannt/nicht genutzt

mv: ao6 

ka:

vc:

av:

kh:

fv:

hv:

fo: ao6 (missing) bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="N_9"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_9a 
==========

tc:

vn: digosa

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor bzw. zu Beginn des Studiums einen Selbsttest zur fachlichen Eignung durchgeführt (z. B. Online-Self-Assessment)?

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

tr:

hi:

\------------------------------------------------------------

N_9
=========

tc:

vn: digorg (digorg1; digorg2; digorg3; digorg4; digorg5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie viele Ihrer Lehrveranstaltungen werden über digitale Plattformen organisiert (z. B. StudIP, Moodle, Ilias, Olat)?

is:

it1: (digorg1): An-/Abmeldung zu Lehrveranstaltungen

it2: (digorg2): An-/Abmeldung zu Prüfungen, Ergebniseinsicht

it3: (digorg3): Kommunikation innerhalb der Lehrveranstaltungen

it4: (digorg4): Bereitstellung von Literatur und Lehrmaterialien

it5: (digorg5): Erbringung von Leistungsnachweisen/elektronische Prüfungen

st:

ao1: 1: keine

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: alle 

ao6: -12: weiß ich nicht  

mv: ao6

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="N_10"/>
        </zofar:transitions>

hi: ao6 (missing) bitte etwas absetzen.

\------------------------------------------------------------

N_9b
=========

tc:

vn: digfor (digfor1; digfor2; digfor3; digfor4; digfor5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie viele Ihrer Lehrveranstaltungen werden in folgender Form organisiert?

is:

it1: (digfor1): als reine Online-Veranstaltung (z. B. Online-Vorlesung, Online-Seminar) 

it2: (digfor2): als Online-Selbststudium mit einzelnen Präsenzterminen

it3: (digfor3): als Präsenzveranstaltung mit einzelnen Online-Terminen

it4: (digfor4): als reine Präsenzveranstaltung

st:

ao1: 1: keine

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: alle 

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

N_10
=========

tc:

vn: diglehr (diglehr1; diglehr2; diglehr3; diglehr4; diglehr5; diglehr6; diglehr7; diglehr8; diglehr9; diglehr9o)

qt: Einfachauswahlmatrix mit horizontalen ao; offene Angabe

hl:

in:

q: Wie häufig kommen folgende digitale Elemente und Lehrformate im Rahmen der von Ihnen besuchten Lehrveranstaltungen zum Einsatz?

is:

it1: (diglehr1): Podcasts, Blogs, Videos

it2: (diglehr2): Abstimmungsmedien (Clicker-Abfrage, Voting-Tool)

it3: (diglehr3): Game-Based-Learning (auf Lernspielen basierende Lehr- und Lernformate)

it4: (diglehr4): Mobiles Lernen (virtuelle Lernorte/Labore)

it5: (diglehr5): Augmented- und Virtual-Reality

it6: (diglehr6): E-Portfolio (digitales Lerntagebuch)

it7: (diglehr7): Videoaufzeichnungen von Vorlesungen

it8: (diglehr8): digitale Prüfungsformate/E-Assessment

it12: (diglehr9): Etwas anderes und zwar: [(diglehr9o), offene Angabe, 80 Zeichen] 

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

tr:

        <zofar:transitions>
            <zofar:transition target="N_11"/>
        </zofar:transitions>

hi: ao6 (missing) bitte etwas absetzen.

\------------------------------------------------------------

N_10a
=========

tc:

vn: diggeso (diggeso1; diggeso2; diggeso3; diggeso4; diggeso5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig werden die folgenden Geräte bzw. Software in eine typische Lehrveranstaltung eingebunden?

is:

it1: (diggeso1): Laptop und Beamer der Hochschule

it2: (diggeso2): Smart-Board

it3: (diggeso3): eigener Laptop, Tablet, Smartphone

it4: (diggeso4): Präsentationssoftware (PowerPoint, Prezi)

it5: (diggeso5): fachspezifische Software

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

\------------------------------------------------------------

N_10b
=========

tc:

vn: digflehr (digflehr1; digflehr2; digflehr3)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig nutzen Sie die folgenden Formen des digitalen Lernens?

is:

it1: (digflehr1): im Internet zugängliche Lehr- und Lernmaterialien

it2: (digflehr2): Lehr- und Lernvideos

it3: (digflehr3): digitale Selbstlernprogramme (z. B. Simulation, Lernapps, Lernspiele)

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

\------------------------------------------------------------

N_11
=========

tc:

vn: digkom (digkom1; digkom2; digkom3; digkom4; digkom5; digkom6)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit nutzen Sie die folgenden digitalen Möglichkeiten bei der Zusammenarbeit mit Ihren Kommiliton\*innen? 

is:

it1: (digkom1): Instant Messaging-Dienste (z. B. WhatsApp, Telegram)

it2: (digkom2): Soziale Netzwerke (z. B. Facebook, Instagram)

it3: (digkom3): Online Verwaltungstools (z. B. Doodle, Trello)

it4: (digkom4): Tools der Lernmanagementsysteme (z. B. Peer-Feedback, Foren)

it5: (digkom5): Clouddienste zum gemeinsamen Schreiben (z.B. Etherpad, Google docs)

it6: (digkom6): Clouddienste zum Dateienaustausch (z. B. Dropbox)

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
            <zofar:transition target="N_12"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_12
=========

tc:

vn: digan (digan1; digan2; digan3; digan4; digan5; digan6; digan7; digan8; digan9; digan10; digan11)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie leicht würde es Ihnen fallen, …

is:

it1: (digan1): … einen Text nach bestimmten Vorgaben zu formatieren (z. B. mit Word, Latex)? 

it2: (digan2): … eine animierte Präsentation zu gestalten (z. B. mit Power Point, Prezi)

it3: (digan3): … eine Tabellenkalkulation durchzuführen (z. B. Excel, Open Office Calc)

it4: (digan4): … eine Literaturdatenbank anzulegen (z. B. mit Citavi, EndNote)?

it5: (digan5): … zentrale Literatur zu einem wissenschaftlichen Thema online zu recherchieren? 

it6: (digan6): … wissenschaftliche von nicht-wissenschaftlichen Internetquellen zu unterscheiden?

it7: (digan7): … von Ihnen genutzte digitale Medien miteinander zu synchronisieren?

it8: (digan8): … sich in ein neues Computerprogramm einzuarbeiten?

it9: (digan9): … eine Programmiersprache sicher anzuwenden (z. B. Python, Java)?

it10: (digan10): … digitale Gruppen/Netzwerke zu recherchieren und sich zu beteiligen?

it11: (digan11): … sich in einer virtuellen oder simulierten Umgebung zu bewegen und zu handeln?

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_57"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_13
=========

tc: IF zusatzsplit ==4

vn: diskjane (diskjaneno; diskjane1; diskjane2; diskjane3; diskjane4; diskjane5; diskjane6; diskjane7; diskjane8; diskjane9; 
diskjane10; diskjane11; diskjane12; diskjane13; diskjane14; diskjane15; diskjane16; diskjane16o)

qt: Mehrfachauswahl mit Exklusivkategorie und offener Angabe

hl:

in: Nun geht es um das Thema Diskriminierung. Diskriminierung bedeutet, dass eine Person aus bestimmten Gründen schlechter behandelt wird als andere Menschen, ohne dass es dafür eine sachliche Rechtfertigung gibt.

q: Haben Sie selbst bereits diskriminierende Erfahrungen im Rahmen Ihres Studiums gemacht?

is:

it:

st:

ao1: (diskjaneno): nein [Exklusivkategorie]

ao2: (diskjane1): Leistungen wurden mir nicht zugetraut.

ao3: (diskjane2): Von mir erbrachte Leistungen wurden herabgesetzt (z. B. ungerecht bewertet).

ao4: (diskjane3): Regeln/Verfahren wurden so gestaltet, dass ich benachteiligt wurde. 

ao5: (diskjane4): Mir wurden Rechte/Informationen vorenthalten.

ao6: (diskjane5): Mein Antrag wurde abgelehnt oder mir wurde eine Leistung verwehrt. 

ao7: (diskjane6): Ich wurde durch Barrieren eingeschränkt (z. B. Hindernisse, Erreichbarkeit von Räumen). 

ao8: (diskjane7): Ich wurde ausgegrenzt oder übergangen (z. B. in Arbeitsgruppen).

ao9: (diskjane8): Menschen wie ich wurden stereotyp/herabwürdigend dargestellt.

ao10: (diskjane9): Mir sind unangebrachte Bemerkungen zu meinem Privatleben begegnet. 

ao11: (diskjane10): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

ao12: (diskjane11): Ich wurde beleidigt oder beschimpft. 

ao13: (diskjane12): Ich habe unerwünschte sexualisierte Kommentare erlebt.

ao14: (diskjane13): Ich habe sexualisierte körperliche Übergriffe erlebt. 

ao15: (diskjane14): Ich wurde körperlich bedroht.

ao16: (diskjane15): Ich wurde körperlich angegriffen. 

ao17: (diskjane16): Anderes, und zwar: [(diskjane16o), offene Angabe, 250 Zeichen] 

mv:

ka: (ao2 TO ao17): Ja, und zwar: 

vc:

av:

kh:

fv:

hv:

fo1: Bitte über ao2 "Ja, und zwar:" linksbündig positionieren.

fo2: "Haben Sie selbst bereits diskriminierende Erfahrungen im Rahmen Ihres Studiums gemacht?" bitte etwas von den Einleitungssätzen absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="N_14" condition="!diskjane.value"/>
            <zofar:transition target="A_57" condition="diskjane.value"/>
        </zofar:transitions>
    
hi:

\------------------------------------------------------------

N_14
=========

tc:

vn: diskanza (diskanza1; diskanza2; diskanza3; diskanza4; diskanza5; diskanza6; diskanza7; diskanza8; diskanza9; diskanza10; 
diskanza11; diskanza12; diskanza13; diskanza14; diskanza15; diskanza16)

qt: Einfachauswahlmatrix mit horizontalen ao

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

it9: (diskanza9): Mir sind unangebrachte Bemerkungen zu meinem Privatleben begegnet.

it10: (diskanza10): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

it11: (diskanza11): Ich wurde beleidigt oder beschimpft.

it12: (diskanza12): Ich habe unerwünschte sexualisierte Kommentare erlebt.

it13: (diskanza13): Ich habe sexualisierte körperliche Übergriffe erlebt.

it14: (diskanza14): Ich wurde körperlich bedroht.

it15: (diskanza15): Ich wurde körperlich angegriffen.

it16: (diskanza16): Anderes

st:

ao1: 1: einmal

ao2: 2: mehrmals

ao3: 3: regelmäßig

ao4: -12: weiß ich nicht

mv: ao4

ka:

vc1: SHOW it1 (diskanza1) IF diskjane1=1

vc2: SHOW it2 (diskanza2) IF diskjane2=1

vc3: SHOW it3 (diskanza3) IF diskjane3=1

vc4: SHOW it4 (diskanza4) IF diskjane4=1

vc5: SHOW it5 (diskanza5) IF diskjane5=1

vc6: SHOW it6 (diskanza6) IF diskjane6=1

vc7: SHOW it7 (diskanza7) IF diskjane7=1

vc8: SHOW it8 (diskanza8) IF diskjane8=1

vc9: SHOW it9 (diskanza9) IF diskjane9=1

vc10: SHOW itq10 (diskanza10) IF diskjane10=1

vc11: SHOW it11 (diskanza11) IF diskjane11=1

vc12: SHOW it12 (diskanza12) IF diskjane12=1

vc13: SHOW it13 (diskanza13) IF diskjane13=1

vc14: SHOW it14 (diskanza14) IF diskjane14=1

vc15: SHOW it15 (diskanza15) IF diskjane15=1

vc16: SHOW it16 (diskanza16) IF diskjane16=1

av:

kh:

fv:

hv:

fo: ao4 bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="N_15"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_15
=========

tc:

vn: diskwem (diskwem1; diskwem2; diskwem3; diskwem4; diskwem5; diskwem6; diskwem7; diskwem8; diskwem8o)

qt:  Mehrfachauswahl; offene Angabe

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

ao7: (diskwem7): keine Angabe

ao8: (diskwem8): Andere, und zwar: [(diskwem8o), offene Angabe, 250 Zeichen]

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
            <zofar:transition target="A_57"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------



D3_1
=========

tc:

vn: wohnplz; wohnplzort

qt: Einfachauswahl mit vertikalen ao und offener Angabe

hl:

in:

q1: Wo wohnen Sie während der Vorlesungszeit hauptsächlich?

q2: Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an.
is:

it:

st:

ao1: (wohnplz): [infield = PLZ; number, 5-stellig: 01000 TO 99999] 

ao2: (wohnplzort): [infield = Ort; 60 Zeichen]

mv:

ka:

vc:

av:

kh: (wohnplz): Bitte geben Sie Ihre Postleitzahl an (01000 bis 99999).

fv:

hv:

fo: SHOW q2 and ao2 IF wohnplz = k. A. (--> soft forcing)

tr:

      <zofar:transitions>
            <zofar:transition target="D3_3"/>
        </zofar:transitions>

hi: Bitte q1 und ao1 zusammen oberhalb von q2 und ao2 darstellen.

\------------------------------------------------------------

F3_23
=========

tc:

vn: wohnemin; wohnemino

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Wie viel Zeit benötigen Sie für den einfachen Weg von Ihrer Wohnung zur Hochschule?

is: Bitte geben Sie die Dauer „von Tür zu Tür“ an.

it:

st:

ao1: 1: Präfix: Dauer: [wohnemino] (infield=Minutenangabe; NUMBER; 3-Stellen)

ao2: -12: weiß ich nicht

mv: ao2

ka:

vc:

av: number: 3-Stellen: 1 TO 999

kh: Bitte geben Sie die Dauer des einfachen Weges von Ihrer Wohnung zu Ihrer Hochschule an (1 bis 999).

fv:

hv:

fo:

tr:

       <zofar:transitions>
            <zofar:transition target="F3_24"/>
        </zofar:transitions>

hi:
 
\------------------------------------------------------------

F3_24
=========

tc:

vn: mobregmittel

qt: Einfachauswahl

hl:

in:

q: Welches Verkehrsmittel nutzen Sie überwiegend um an Ihre Hochschule zu gelangen?

is: Bei kombinierter Nutzung geben Sie bitte das Verkehrsmittel an, mit dem Sie die längste Wegstrecke zurücklegen.

it:

st:

ao1: 1: zu Fuß

ao2: 2: Fahrrad

ao3: 3: Öffentliche Verkehrsmittel

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

       <zofar:transitions>
            <zofar:transition target="F3_25"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

N_17
=========

tc:

vn: diskwoh (diskwoh1; diskwoh2; diskwoh3)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Ihre persönlichen Erfahrungen bei der Wohnungssuche zu?

is: 

it1: (diskwoh1): Ich habe mich oft vergeblich um eine Wohnung beworben.

it2: (diskwoh2): Für die Wohnungssuche sind soziale Kontakte sehr wichtig.

it3: (diskwoh3): Eine Wohnung zu einem günstigen Mietpreis zu finden, ist fast aussichtslos.

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

hi:
 
\------------------------------------------------------------

N_16
=========

tc:

vn: lftaus (lftaus1; lftaus2; lftaus3; lftaus4);
    lftzei (lftzei1; lftzei2; lftzei3; lftzei4) 
       

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Ihre Lebensführung zu?

is: 

it1: (lftaus1): Ich pflege einen gehobenen Lebensstandard.

It2: (lftaus2): Es ist mir zu teuer, regelmäßig große Urlaube im Ausland zu machen.

It3: (lftaus3): In Kunst und Kultur kenne ich mich sehr gut aus.

It4: (lftaus4): Ich lese gern anspruchsvolle Bücher.

It5: (lftzei1): Mein Leben gefällt mir dann besonders gut, wenn ständig etwas los ist.

It6: (lftzei2): Ich suche immer wieder nach neuen Herausforderungen und Erfahrungen.

It7: (lftzei3): Sicherheit und Beständigkeit sind das oberste Gebot in meinem Leben.

It8: (lftzei4): Ich halte an Traditionen und Bräuchen meiner Familie fest.

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

hi:

\------------------------------------------------------------

B2_5
=========

tc:

vn: frei (freispor; freikunst; freikult; freiparty; freifreu; freipc; freifimu; freiehr; freidiswiss; freidispol; freinix)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig gehen Sie in Ihrer Freizeit folgenden Tätigkeiten nach?

is:

it1: (freispor): sportlich betätigen

it2: (freikunst): künstlerisch betätigen (zeichnen,  musizieren)

it3: (freikult): Kulturveranstaltungen besuchen (Konzerte, Theater, Poetry-Slam etc.)

it4: (freiparty): feiern, auf Partys gehen

it5: (freifreu): Freunde treffen

it6: (freipc): Videospiele, Computer spielen

it7: (freifimu): Filme/Serien schauen, Musik hören

it8: (freiehr): ehrenamtlich tätig sein

it9: (freidiswiss): über wissenschaftliche Themen reden

it10: (freidispol): über soziale und politische Fragen diskutieren

it11: (freinix): einfach nichts tun

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
            <zofar:transition target="B2_4"/>
        </zofar:transitions>

hi:

\------------------------------------------------------------

A_57
=========

tc:

vn: sdkzei (sdkzei1; sdkzei2; sdkzei3; sdkzei5; sdkzei7; sdkzei8; sdkzei9; sdkzei12; sdkzei13; sdkzei14; sdkzei15; sdkzei16)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie wichtig sind Ihnen die folgenden Aspekte Ihres weiteren Berufs- und Lebensweges?

is:

it1: (sdkzei1): hohes Einkommen

it2: (sdkzei2): prestigeträchtige Berufsposition

it3: (sdkzei3): sicherer Arbeitsplatz

it5: (sdkzei5): flexible Arbeitszeiten

it7: (sdkzei7): verantwortungsvolle Aufgaben übernehmen

it8: (sdkzei8): eigene Ideen verwirklichen

it9: (sdkzei9): selbstständig Entscheidungen treffen

it12: (sdkzei12): anderen Menschen helfen zu können

it13: (sdkzei13): ein Beruf, in dem ich Nützliches für die Allgemeinheit tun kann

it14: (sdkzei14): Vereinbarkeit von Privatleben und Beruf

it15: (sdkzei15): eine glückliche Beziehung führen

it16: (sdkzei16): eine Familie gründen

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

tr:

        <zofar:transitions>
           <zofar:transition target="end"/>
        </zofar:transitions>

hi:
