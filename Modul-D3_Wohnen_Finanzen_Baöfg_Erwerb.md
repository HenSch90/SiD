\--------------------------------

D3_2
====

tc:

vn: wohnamio; wohnqmw; wohnqmz

qt: offene Angaben

hl:

in:

q1: Mit wie vielen Personen wohnen Sie insgesamt – also Sie selbst mit eingeschlossen – zusammen?

q2: Wie groß ist Ihre Wohnung/Ihr Haus?

q3: Wie groß ist das von Ihnen genutzte Zimmer?

q4: Wie groß ist Ihr Einzelzimmer/-appartment?

is:

it:

st:

ao1: (wohnamio): [number, 2-stellig: 1 To 15], Postfix: Person(en)

ao2: (wohnqmw): [number, 3-stellig: 1 TO 999], Postfix: m²

ao3: (wohnqmz): [number, 2-stellig: 1 TO 99], Postfix: m²

mv:

ka:

vc1: SHOW q2, ao2 IF wohnal == 1 & (wohnfo != 4 | wohnfo !=5 | wohnfo !=6)

vc2: SHOW q4, ao2 IF wohnal == 1 & (wohnfo == 4 | wohnfo ==5 | wohnfo ==6)

vc3: SHOW q1, q2, q3, ao1, ao2, ao3 IF (wohnwg==1 | wohnel == 1 |wohnfam == 1 | wohnsons == 1) & (wohnfo != 4 | wohnfo !=5 | wohnfo !=6)

vc4: SHOW q1, q4, ao1, ao2, ao3 IF (wohnwg==1 | wohnel == 1 |wohnfam == 1 | wohnsons == 1) & (wohnfo == 4 | wohnfo ==5 | wohnfo ==6)

vc5: SHOW  q1, q2, ao1, ao2 IF (wohnpar == 1 | wohnkin ==1) & (wohnfo != 4 | wohnfo !=5 | wohnfo !=6)

vc6: SHOW q1, q4, ao1, ao2 IF (wohnpar == 1 | wohnkin ==1) & (wohnfo == 4 | wohnfo ==5 | wohnfo ==6)

av: 

kh1: (wohnamio): Bitte geben Sie die Anzahl an Personen an, mit denen Sie zusammenwohnen (1 bis 15).

kh2: (wohnqmw): Bitte geben Sie die Größe Ihrer Wohnung/Ihres Hauses an (1 bis 999).

kh3: (wohnqmz): Bitte geben Sie die Größe Ihres Zimmers an (1 bis 99).


fv:

hv:

fo: Auf der Seite als erstes q1/ao1 zusammen darstellen. Darunter dann q2/ao2 zusammen darstellen und darunter dann ggf. q3/ao3 zusammen einblenden.

tr:

        <zofar:transitions>
            <zofar:transition target="D3_5"/>
        </zofar:transitions>

hi: 

\--------------------------------


D3_5
====

tc:

vn: wohnzust (wohnzustallg / wohnzustlaut / wohnzustrüzu / wohnzustinet / wohnzusttech)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie würden Sie Ihre Wohnsituation hinsichtlich der folgenden Aspekte bewerten?

is:

it1: (wohnzustallg): Allgemeinzustand der Wohnung

it2: (wohnzustlaut): Lautstärke

it3: (wohnzustrüzu): Rückzugsmöglichkeiten

it4: (wohnzustinet): Internetverbindung

it5: (wohnzusttech): technische Ausstattung (z. B. Monitor, Drucker)

st:

ao1: 1: sehr schlecht

ao2: 2

ao3: 3

ao4: 4

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
           <zofar:transition target="B2_7" condition="(zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12)" />
            <zofar:transition target="B1_5" condition="(zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6)"/>
        </zofar:transitions>


hi:

\--------------------------------

D3_6
====

tc:

vn: fein (feinelto / feinekio / feinparo / feinjobo1 /  feinspao / feinbafo / feinkredo / feinstio /  feinbest / feinandq / feinandqo / feininsg)

qt: offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich ++pro Monat++
während des Sommersemesters 2021 zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst
verfügen. ++Nicht++ gemeint sind Beträge, die z. B. von Ihren Eltern für Sie direkt 
an Dritte überwiesen werden (z. B. Überweisung der Miete durch Ihre Eltern).

it1: (feininsg): !!Gesamteinnahmen!!:

#{layout.BREAK}#{layout.BREAK } 

it2: (feinelto): Eltern und Verwandte

it3: (feinekio): Kindergeld/Unterhalt für Ihr(e) Kind(er)

it4: (feinparo): Partner\*in 

it5: (feinjobo1): Erwerbstätigkeit (auch Ausbildungsvergütung)

it6: (feinspao): eigene Mittel (z. B. Ersparnisse, Erbe)

it7: (feinbafo): BAföG

it8: (feinkredo): Kredit(e)

it9: (feinstio): Stipendium

it10: (feinbest): Sozialleistungen im Zusammenhang mit Ihrer gesundheitlichen Beeinträchtigung

it11: (feinandq): Weitere Finanzierungsquelle(n), und zwar: 

st:

ao1: (feininsg), [infield = € pro Monat; number, 5-stellig: 0 TO 99999]

#{layout.BREAK}#{layout.BREAK } 

ao2: (feinelto): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3: (feinekio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4: (feinparo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5: (feinjobo1): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6: (feinspao): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao7: (feinbafo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao8: (feinkredo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao9: (feinstio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao10: (feinbest): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao11: (feinandq; feinandqo): [50 Zeichen] [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

mv:

ka: (it2 TO it11): !!davon entfallen auf:!!

vc1: SHOW it3/ao3 (feinekio) IF dkinja = 2

vc2: SHOW it5/ao5 (feinjobo1) IF sformdua == 1 | sformberu==1 | eaktsens>1

vc3: SHOW it10/ao10 (feinbest) IF  h_gartcount >= 1 

av: 

kh1: ao2 TO ao11: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (0 bis 9999).

kh2: ao1: Bitte geben Sie Ihre monatlichen Gesamteinnahmen an (0 bis 99999).

fv:

hv:

fo: Bitte ka linksbündig.

tr:

	<zofar:transitions>
            <zofar:transition target="D3_6b" condition="feinkredo.value”/>
            <zofar:transition target="D3_7"/>
        </zofar:transitions>


hi: 

\--------------------------------

D3_6b
====

tc:

vn: fekreart (fekreartbil / fekreartkfw / fekreartsons / fekreartsonso)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Sie haben angegeben, über einen Kredit Ihr Studium zu finanzieren: Welchen Kredit nutzen Sie aktuell? 

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (fekreartbil): Bildungskredit der Bundesregierung

ao2: (fekreartkfw): KfW-Studienkredit

ao3: (fekreartsonso): Anderer Studienkredit, und zwar: [(fekreartsonso); 50 Zeichen]   

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
            <zofar:transition target="D3_7"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_7
====

tc:

vn: festipart (festipartnein1 / festipartnein2 / festipartnein3 / festipartdeut / festipartbegabt / festipartweitbil / festipartaufstieg / festipartandstaat / festipartprivat / festipartsons / festipartsonso)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Erhalten Sie aktuell ein Stipendium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (festipartnein1): nein, nicht beantragt

ao2: (festipartnein2): nein, Antrag wurde nicht bewilligt

ao3: (festipartnein3): nein, Antragsverfahren läuft noch 

ao4: (festipartdeut): Deutschlandstipendium

ao5: (festipartbegabt): Stipendium eines Begabtenförderungswerkes

ao6: (festipartweitbil): Weiterbildungsstipendium

ao7: (festipartaufstieg): Aufstiegsstipendium der Stiftung Begabtenförderung berufliche Bildung gGmbH

ao8: (festipartandstaat): anderes mit staatlichen Mitteln finanziertes Stipendium (z. B. Hochschule, Land)

ao9: (festipartprivat): Stipendium eines privaten Geldgebers (z. B. Industrie, privater Stifter)

ao10: (festipartsons): Anderes, und zwar: [(festipartsonso); 50 Zeichen]

mv:

ka: (ao4 TO ao10): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: "Ja, und zwar:" zwischen ao3 und ao4 setzen.

tr:

        <zofar:transitions>
            <zofar:transition target="D3_8"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_8
====

tc:

vn1: fausg (fausgmieto / fausgerno / fausgkomo / fausgkleio / fausglerno / fausggeso / fausgmobo / fausgsemo / fausgstuo / fausgfreio / fausgkitaso / fausgkindso / fausgasso / fausandq / fausandqo) 

vn2: feind (feindmieto / feinderno / feindkomo / feindkleio / feindlerno / feindgeso / feindmobo / feindgsemo / feindstuo / feindfreio / feindkitaso / feindkindso / feindasso / feinandquo2)

vn3: fausinsg; feininsg2



qt: offene Angabe

hl:

in:

q: Bitte geben Sie an, welche Ausgaben Sie bzw. andere für Sie im Sommersemester 2021 ++monatlich++ haben.

is1: "Andere bezahlen für mich" meint bspw. die Überweisung der Miete durch Ihre Eltern. 

is2: Bitte geben Sie nur den jeweils auf Sie persönlich bezogenen Betrag an.

it1: (fausinsg; feininsg2): ++Gesamtausgaben++:

#{layout.BREAK}#{layout.BREAK}

it2: (fausgmieto; feindmieto): Warmmiete (inkl. Nebenkosten)

it3: (fausgerno; feinderno): Ernährung 

it4: (fausgkomo; feindkomo): Telefon, Internet

it5: (fausgkleio; feindkleio): Kleidung

it6: (fausglerno; feindlerno): Lernmittel (z. B. Fachliteratur)

it7: (fausggeso; feindgeso): Gesundheitskosten (z. B. Krankenversicherung, Medikamente, Therapien)

it8: (fausgsemo; feindgsemo): Semesterbeitrag (inkl. Semesterticket)

it9: (fausgstuo; feindstuo): Studiengebühren 

it10: (fausgmobo; feindmobo): Mobilitätskosten (z. B. Auto, Bahn)

it11: (fausgfreio; feindfreio): Freizeit, Kultur und Sport

it12: (fausgkitaso; feindkitaso): Ausgaben für Kinderbetreuung

it13: (fausgkindso; feindkindso): kinderbezogene Ausgaben (Drogerieartikel, Kleidung usw.)

it14: (fausgasso; feindasso): Ausgaben für personelle Assistenzen im Zusammenhang mit einer Beeinträchtigung (z. B. Pflegeassistenz, Mitschreibkraft)

it15: (fausandq): weitere Ausgaben, und zwar:






st:

ao1: (fausinsg; feininsg2): [infield = € pro Monat; number, 5-stellig: 0 TO 99999]

#{layout.BREAK}#{layout.BREAK}

ao2: (fausgmieto; feindmieto): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3: (fausgerno; feinderno): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4: (fausgkomo; feindkomo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5: (fausgkleio; feindkleio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6: (fausglerno; feindlerno): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao7: (fausggeso; feindgeso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao8: (fausgsemo; feindgsemo): [infield = € pro Semester; number, 4-stellig: 0 TO 9999]

ao9: (fausgstuo; feindstuo): [infield = € pro Semester; number, 4-stellig: 0 TO 9999]

ao10: (fausgmobo; feindmobo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao11: (fausgfreio; feindfreio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao12: (fausgkitaso; feindkitaso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao13: (fausgkindso; feindkindso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao14: (fausgasso; feindasso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao15: (fausandqo; feinandqo2): [50 Zeichen] [infield = € pro Monat; number, 4-stellig: 0 TO 9999]


mv:

ka: (it2 TO it15): !!davon entfallen auf:!!

vc1: SHOW it11/ao11 TO it12/ao12 IF dkinja = 2

vc2: SHOW it13/ao13 IF h_gartcount >= 1 

vc3: SHOW is2 IF wohnal=!1

av: 

kh1: ao2 TO ao15: Bitte geben Sie Ihre jeweiligen monatlichen Ausgaben an (0 bis 9999).

kh2: ao2 TO ao15: Bitte geben Sie an, was andere monatlich jeweils für Sie bezahlen (0 bis 9999).

kh3: ao1: Bitte geben Sie Ihre monatlichen Gesamtausgaben an (0 bis 99999).

kh4: ao1: Bitte geben Sie an, was andere monatlich insgesamt für Sie bezahlen (0 bis 99999).

fv:

hv:

fo1: “ich bezahle selbst” und “andere bezahlen für mich” bitte als Spaltenüberschriften über die erste bzw. zweite Spalte mit den Eingabefeldern setzen.

fo2: Bitte etwas Abstand zwischen den beiden Spalten.

fo3: Bitte Leerzeile/Abstand nach den Gesamtausgaben einziehen. 

fo4: Bitte ka "davon entfallen auf" zwischen It1 "Gesamtausgaben" und den nachfolgenden einfügen.

tr:

	<zofar:transitions>
            <zofar:transition target="D3_8a" condition=" zofar.asNumber(feininsg2) gt 0 or zofar.asNumber(feindmieto) gt 0 or zofar.asNumber(feinderno) gt 0 or zofar.asNumber(feindkomo) gt 0  or zofar.asNumber(feindkleio) gt 0 or zofar.asNumber(feindlerno) gt 0  or zofar.asNumber(feindgeso) gt 0 or zofar.asNumber(feindmobo) gt 0 or zofar.asNumber(feindgsemo) gt 0 or zofar.asNumber(feindstuo) gt 0 or zofar.asNumber(feindfreio) gt 0 or zofar.asNumber(feindkitaso) gt 0 or zofar.asNumber(feindkindso) gt 0 or zofar.asNumber(feindasso) gt 0 or zofar.asNumber(feinandquo2) gt 0 "/>
		<zofar:transition target="D3_9"/>        
	</zofar:transitions>


hi1: Bitte kh1 für die Einzelausgabeposten der Spalte "ich bezahle selbst" nutzen und kh2 für die Einzelausgabeposten der Spalte "andere bezahlen für mich".

hi2: Bitte kh3 für die Gesamtausgaben der Spalte "ich bezahle selbst" nutzen und kh4 für die Gesamtausgaben der Spalte "andere bezahlen für mich".

\--------------------------------

D3_8a
====

tc:

vn: feind1 ( feind1eltern / feind1partner / feind1verwandt / feind1arbeitg / feind1sons / feind1sonso)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Sie haben angegeben, dass ein Teil Ihrer Ausgaben von anderen bezahlt wird: Von wem werden Sie unterstützt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (feind1eltern): Eltern/-teil

ao2: (feind1partner): Partner\*in

ao3: (feind1verwandt): andere Verwandte

ao4: (feind1arbeitg): Arbeitgeber\*in

ao10: (feind1sons): Andere, und zwar: [(feind1sonso); 50 Zeichen]

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
            <zofar:transition target="D3_9"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_9
=====

tc:

vn: fmineinko

qt: offene Angabe

hl:

in:

q: Wie viel Geld benötigen Sie mindestens pro Monat, um finanziell zurecht zu kommen?

is:

it:

st:

ao1: (fmineinko): [infield = € pro Monat; number, 5-stellig: 1 TO 99999], Postfix: € 

mv:

ka:

vc:

av: 

kh: (fmineinko): Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 99999).

fv:

hv:

fo:

tr:

	<zofar:transitions>
            <zofar:transition target="D3_11"/>
        </zofar:transitions>



hi:

\--------------------------------

D3_11
=====

tc:

vn: fsit (fsitzum1 / fsitzum2 / fsitzum3 / fsitzum4)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie und Ihre finanzielle Situation zu?

is:

it1: (fsitzum1): Die Finanzierung meines Lebensunterhalts während des Studiums ist sichergestellt.

it2: (fsitzum3): Im Großen und Ganzen gelingt es mir, mit meinem Geld auszukommen.

it3: (fsitzum2): Ich habe zurzeit finanzielle Schwierigkeiten.

it4: (fsitzum4): Aufgrund der Corona-Pandemie kann ich mein Studium ohne zusätzliche finanzielle Unterstützung nicht fortführen. 

st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2

ao3: 3

ao4: 4

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
            <zofar:transition target="A_54"/>
        </zofar:transitions>

hi: Rotation der ITems bitte entfernen

\--------------------------------

D3_13
=====

tc:

vn: fbafja

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Werden Sie im Sommersemester 2021 nach dem BAföG gefördert?

is:

it:

st:

ao1: 1: Nein, ich habe keinen Antrag gestellt.

ao2: 2: Nein, mein aktueller Antrag wurde endgültig abgelehnt.

ao3: 3: Über meinen Antrag (bzw. Widerspruch) ist noch nicht entschieden.

ao4: 4: ja

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
            <zofar:transition target="D3_13b"/>
        </zofar:transitions> 

hi:


\--------------------------------

D3_13b
=====

tc:

vn: fbafber

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie bereits eine Beratung zum Thema BAföG in Anspruch genommen?

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
            <zofar:transition target="D3_14" condition="zofar.asNumber(fbafja)==1"/>
            <zofar:transition target="D3_15" condition="zofar.asNumber(fbafja)==2"/>
            <zofar:transition target="D3_17" condition="zofar.asNumber(fbafja)==4"/>
            <zofar:transition target="D3_6" condition="zofar.asNumber(fbafja)==3        or zofar.isMissing(fbafja)"/>
        </zofar:transitions>



hi:


\--------------------------------

D3_14
=====

tc: IF fbafja = 1 

vn: fbafex

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie während Ihres Studiums früher einmal einen Antrag auf BAföG gestellt?

is:

it:

st:

ao1: 1: nein

ao2: 2: Ja, ich habe einen Antrag gestellt, der wurde aber abgelehnt.

ao3: 3: Ja, in früheren Semestern wurde ich gefördert, ein Antrag auf
Weiterförderung wurde abgelehnt.

ao4: 4: Ja, in früheren Semestern wurde ich gefördert, habe dann aber
keinen Antrag auf Weiterförderung gestellt.

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
            <zofar:transition target="D3_16"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_15
=====

tc:IF fbafja = 2 

vn: fbafabg

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie bereits früher schon einmal einen Antrag auf BAföG gestellt?

is:

it:

st:

ao1: 1: nein

ao2: 2: Ja, ich habe früher einen Antrag gestellt, der wurde aber abgelehnt.

ao3: 3: Ja, in früheren Semestern wurde ich gefördert.

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
            <zofar:transition target="D3_16"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_16
=====

tc: IF fbafja = 1 \| 2 

vn: fbaf (fbafkelt / fbafkein / fbafkfhd / fbafktw / fbafkleis / fbafkrsz/ fbafkalt / fbafkzwei / fbafkweni / fabfkschu / fbafand / fbafando)

qt: Mehrfachnennung/offene Angabe mit vertikalen ao

hl:

in:

q1: Aus welchen Gründen haben Sie bisher keinen BAföG-Antrag gestellt?

q2: Aus welchen Gründen wurde Ihr aktueller Antrag abgelehnt?

q3: Aus welchen Gründen wurde Ihr Antrag damals abgelehnt?

q4: Aus welchen Gründen haben Sie keinen Antrag auf Weiterförderung mehr gestellt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (fbafkelt): Das Einkommen der Eltern bzw. des Ehepartners/der Ehepartnerin ist zu hoch.

ao2: (fbafkein): Das eigene Einkommen/Vermögen ist zu hoch.

ao3: (fbafkfhd): Die Förderungshöchstdauer wurde überschritten.

ao4: (fbafktw): Das Studienfach wurde gewechselt.

ao5: (fbafkleis): Die notwendigen Leistungsbescheinigungen konnten nicht erbracht werden.

ao6: (fbafkrsz): Die Regelstudienzeit wurde überschritten.

ao7: (fbafkalt): Bei Studienbeginn war die maßgebliche Altersgrenze bereits überschritten.

ao8: (fbafkzwei): Das jetzige Studium ist eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium).

ao9: (fbafkweni): Der zu erwartende Förderbetrag ist so gering, dass es sich nicht lohnt.

ao10: (fbafkschu): Ich will keine Schulden machen.

ao11: (fbafand): Andere Gründe, und zwar: [(fbafando) 50 Zeichen] 

mv:

ka:

vc1: SHOW q1 AND ao1, ao2, ao3, ao4, ao5, ao6, ao7, ao8, ao09, ao10, ao11 IF (fbafja = 1) AND (fbafex = 1 | k. A.)

vc2: SHOW q2 AND ao1, ao2, ao3, ao4, ao5, ao6, ao7, ao8, ao11 IF (fbafja = 2)

vc3: SHOW q3 AND ao1, ao2, ao3, ao4, ao5, ao6, ao7, ao8, ao11 IF (fbafja = 1) AND (fbafex = 2 | 3) 

vc4: SHOW q4 AND ao1, ao2, ao3, ao4, ao5, ao6, ao7, ao8, ao9, ao10 ao11 IF (fbafja = 1) AND (fbafex = 4)

av:

kh:

fv:

hv:

fo:

        <zofar:transitions>
            <zofar:transition target="D3_6"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_17
=====

tc: IF fbafja = 4 

vn: fbafunab

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wird das BAföG unabhängig vom Einkommen Ihrer Eltern gewährt?

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
            <zofar:transition target="D3_18"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_18
=====

tc: IF fbafja = 4 

vn: fbabf (fbafkv / fbafkin)

qt: Mehrfachauswahl

hl:

in:

q1: Ist in Ihrem Förderungsbetrag ein Zuschlag enthalten für …

is: Bitte alles Zutreffende auswählen.

it: 

st:

ao1: (fbafkv): … Ihre Kranken- und Pflegeversicherung?

ao2: (fbafkin): … die Betreuung Ihres Kindes/Ihrer Kinder?

ao3: (fbafkin): … die Betreuung Ihres Kindes?

ao4: (fbafkin): … die Betreuung Ihrer Kinder?

mv:

ka:

vc1: SHOW is AND ao2 IF dkinanz = k. A.

vc2: SHOW is AND ao3 IF dkinanz = 1

vc3: SHOW is AND ao4 IF dkinanz >= 1 

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D3_6"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_19
=====

tc: IF eaktsens = 2 | 3 | 4 

vn1: etat (etat1 / etat2 / etat3); fachn (fachn1 / fachn2 / fachn3)

qt: Tableau/Einfachauswahl

hl:

in: 

q1: Sie haben angegeben, im aktuellen Semester einer Erwerbstätigkeit nachzugehen.

q2: Sie haben angegeben, im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb einer Erwerbstätigkeit nachzugehen.

q3: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten nachzugehen.

q4: Sie haben angegeben, im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb mehreren Erwerbstätigkeiten nachzugehen. 

is1: Bitte geben Sie die Art Ihrer Erwerbstätigkeit und die inhaltliche Nähe zu den Studieninhalten an.

is2: Bitte geben Sie die Art Ihrer jeweiligen Erwerbstätigkeiten und die inhaltliche Nähe zu den Studieninhalten an. Sollten Sie mehr als drei Erwerbstätigkeiten ausüben, dann beziehen Sie Ihre Angaben bitte auf die drei Haupttätigkeiten.


it1: (etat1): !!1. Erwerbstätigkeit!!

ao1: 1: studentische Hilfskraft an der Hochschule
ao2: 2: studentische Hilfskraft außerhalb der Hochschule
ao3: 3: Jobben 
ao4: 4: Selbstständigkeit/freiberufliche Tätigkeit
ao5: 5: Erwerbstätigkeit im gelernten Beruf
ao6: 6: Berufsausbildung
ao7: 7: Praktikum

it2: (fachn1): !!Fachnähe!!

ao8:  1: fachfern
ao9:  2
ao10: 3
ao11: 4
ao12: 5: fachnah


it3: (etat2): !!2. Erwerbstätigkeit!!

ao13: 1: studentische Hilfskraft an der Hochschule
ao14: 2: studentische Hilfskraft außerhalb der Hochschule
ao15: 3: Jobben 
ao16: 4: Selbstständigkeit/freiberufliche Tätigkeit
ao17: 5: Erwerbstätigkeit im gelernten Beruf
ao18: 6: Berufsausbildung
ao19: 7: Praktikum

it4: (fachn2): !!Fachnähe!!

ao20: 1: fachfern
ao21: 2
ao22: 3
ao23: 4
ao24: 5: fachnah


it5: (etat3): !!3. Erwerbstätigkeit!!

ao25: 1: studentische Hilfskraft an der Hochschule
ao26: 2: studentische Hilfskraft außerhalb der Hochschule
ao27: 3: Jobben 
ao28: 4: Selbstständigkeit/freiberufliche Tätigkeit
ao29: 5: Erwerbstätigkeit im gelernten Beruf
ao30: 6: Berufsausbildung
ao31: 7: Praktikum

it6: (fachn3): !!Fachnähe!!

ao32: 1: fachfern
ao33: 2
ao34: 3
ao35: 4
ao36: 5: fachnah

st:

mv: 

vc1: SHOW q1 IF eaktsens = 2 AND sformdua != 1
vc2: SHOW q2 IF eaktsens = 2 AND sformdua = 1
vc3: SHOW q3 IF eaktsens = 3 | 4 AND sformdua != 1
vc4: SHOW q4 IF eaktsens = 3 | 4 AND sformdua = 1

vc5: SHOW is1 IF eaktsens = 2
vc6: SHOW is2 IF eaktsens = 3 | 4

vc7: SHOW it1-it2/ao1-ao12 IF eaktsens = 2 | 3 | 4
vc8: SHOW it3-it4/ao13-ao24 IF eaktsens = 3 | 4 
vc9: SHOW it5-it6/ao25-ao36 IF eaktsens = 4 

av: 

kh: 

fv: 

hv: 

fo: Die Abfrage der Erwerbstätigkeit und Fachnähe soll bitte jeweils zusammen erfolgen. Das heißt "1. Erwerbstätigkeit" (it1) soll als Überschrift in fett programmiert werden und darunter vertikel die entsprechenden ao1-ao7 folgen. Anschließend/darunter soll "Fachnähe" (it2) fett programmiert werden und in derselben Zeile/horizontal die ao8-ao12 folgen. Damit wäre der erste Abschnitt für die erste Erwerbstätigkeit beendet. Der ggf. folgende zweite/dritte Abschnitt würden äquivalent umgesetzt werden, sofern die Einblendbedingungen erfüllt sind.

tr:

	<zofar:transitions>
            <zofar:transition target="D3_20" condition="sformberu.value or sformdua.value"/>
            <zofar:transition target="D3_21" condition="!sformberu.value and !sformdua.value and zofar.asNumber(eaktsens) gt 1"/>
            <zofar:transition target="D3_22" condition="!sformberu.value and !sformdua.value and zofar.asNumber(eaktsens)== 1 or zofar.isMissing(eaktsens)"/>
        </zofar:transitions>



hi: 



\--------------------------------

D3_20
=====

tc: sformberu = 1 | sformdua = 1 

vn1: jobbbdso 

qt: offene Angabe

hl:

in:

q: Welchen Beruf üben Sie aktuell aus?

is: Falls Sie aktuell nicht erwerbstätig sind, geben Sie bitte den jeweils zuletzt ausgeübten Beruf an. 
#{layout.BREAK}
#{layout.BREAK}
Bitte tragen Sie Ihre Berufsbezeichnung möglichst genau ein. Zum Beispiel:
#{layout.BREAK}
#{layout.BREAK}

\-   Bankkauffrau bzw. -mann (nicht: Angestellte\*r)

\-   Zollbeamtin bzw. -beamter (nicht: Beamtin bzw. Beamter)

\-   Maschinenbauingenieur\*in (nicht: Ingenieur\*in)

it:

st:

ao1: (jobbbdso): [infield = Berufsbezeichnung; 100 Zeichen]

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
            <zofar:transition target="D3_22" condition="zofar.asNumber(eaktsens)==1 or zofar.isMissing(eaktsens) or sformberu.value or sformdua.value"/>
            <zofar:transition target="D3_21" condition="zofar.asNumber(eaktsens) gt 1 and zofar.asNumber(acht_c)==2" />
        </zofar:transitions>


hi:

\--------------------------------

D3_21
=====

tc: IF eaktsens = 2 \|3 \|4

vn: egr (egrfin1; egrkar2; egrkar1; /  egrerf1 / egralt1; egrfin3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters einer Erwerbstätigkeit nach, …

q2: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters neben meiner Tätigkeit im Ausbildungsbetrieb einer Erwerbstätigkeit nach, …

q3: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters mehreren Erwerbstätigkeiten nach, …

q4: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters neben meiner Tätigkeit im Ausbildungsbetrieb mehreren Erwerbstätigkeiten nach, …

is:

it1: (egrfin1): ... weil es zur Finanzierung meines Lebensunterhalts unbedingt notwendig ist.

it2: (egrkar2): ... um mich neben dem Studium weiter zu qualifizieren.

it3: (egrkar1): ... um Kontakte für eine spätere Beschäftigung zu knüpfen.

it4: (egrerf1): ... um praktische Erfahrungen zu sammeln.

it5: (egralt1): ... um einen Beitrag zur Gesellschaft zu leisten.

it6: (egrfin3): ... damit ich mir etwas Zusätzliches leisten kann.



st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc:

SHOW q1 IF eaktsens = 2 AND sformdua != 1

SHOW q2 IF eaktsens = 2 AND sformdua = 1

SHOW q3 IF eaktsens =  3 | 4 AND sformdua != 1

SHOW q4 IF eaktsens = 3 | 4 AND sformdua = 1

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D3_22"/>
        </zofar:transitions>

hi: Rotation der Items bitte entfernen

\--------------------------------

D3_22
=====

tc:

vn: zufr (zufrwohn /zufrlstand / zufrfinsit / zufrvstelt / zufrvstbe / zufrvsterw / zufrvstpfl /zufrleb)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie aktuell mit …

is:

it1: (zufrwohn): ... Ihrer Wohnsituation?

it2: (zufrlstand): ... Ihrem Lebensstandard?

it3: (zufrfinsit): ... Ihrer finanziellen Situation?

it4: (zufrvstelt) ... der Vereinbarkeit von Studium und Elternschaft?

it5: (zufrvstbe) ... der Vereinbarkeit von Studium und gesundheitlicher Beeinträchtigung?

it6: (zufrvsterw) ... der Vereinbarkeit von Studium und Erwerbstätigkeit?

it7: (zufrvstpfl) ... der Vereinbarkeit von Studium und Pflegeaufgaben?

it8: (zufrleb): ... Ihrem Leben insgesamt?

st:

ao1: 1: gar nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc1: SHOW it4 IF dkinja = 2 

vc2: SHOW it5 IF h_gartcount >= 1 | gartka = 1

vc3: SHOW it6 IF eaktsens = 2 |3 | 4

vc4: SHOW it7 IF pflegang1 = 1 | pflegang2 = 1

av:

kh:

fv:

hv:

fo:

tr:

	<zofar:transitions>
            <zofar:transition target="D3_23"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_23
====

tc:

vn: allges

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Wie schätzen Sie Ihren Gesundheitszustand im Allgemeinen ein?

is:

it:

st:

ao1: 1: sehr schlecht

ao2: 2

ao3: 3

ao4: 4

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
            <zofar:transition target="D1_27"/>
        </zofar:transitions>


hi:

\--------------------------------

D1_27 
===

tc:

vn: feel (feelstress / feellast / feelglueck / feelschwer )

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig fühlten Sie sich in den letzten vier Wochen …

is:

it1: (feelstress): … gestresst?

it2: (feellast): … überlastet?

it3: (feelglueck): … glücklich?

it4: (feelschwer): … schwermütig? 

st:

ao1: 1: nie

ao2: 2

ao3: 3

ao4: 4

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
            <zofar:transition target="D1_28"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_28 
===

tc: IF NOT gartpsy=1

vn: dep (depausgel / depmuede / depbelast )

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1: (depausgel): Durch mein Studium fühle ich mich ausgelaugt.

it2: (depmuede):Ich fühle mich schon müde, wenn ich morgens aufstehe und wieder einen Tag an der Hochschule vor mir habe.

it3: (depbelast): Das Studium ist eine hohe Belastung für mich.

st:

ao1: 1: nie

ao2: 2

ao3: 3

ao4: 4

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
                <zofar:transition target="D1_7" condition="(zofar.asNumber(ssemfs) le 3 and (zofar.asNumber(sabsan)==1 or (zofar.asNumber(sabsan)ge 3 and zofar.asNumber(sabsan)le 7)))     and (zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10)"/>
                <zofar:transition target="D2_2" condition="(zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12)"/>
                <zofar:transition target="A_44"
        </zofar:transitions>


hi: Itemrotation, falls vorhanden, bitte entfernen.

\--------------------------------

D3_24
====

tc:

vn: koerpbeschw

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Wie häufig hatten Sie in den letzten vier Wochen körperliche Beschwerden?

is:

it:

st:

ao1: 1: nie

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:       <zofar:transitions>
            <zofar:transition target="D3_25"/>
        </zofar:transitions>

hi:

\--------------------------------

D3_25
===

tc: 

vn: belast ( belast1 / belast2 / belast3 / belast4)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Inwiefern stimmen Sie den folgenden Aussagen zu?

is:

it1: (belast1): Ich brauche nicht viel Zeit, um mich von einem stressigen Ereignis zu erholen.

it2: (belast2): Es fällt mir schwer zur Normalität zurückzukehren, wenn etwas Schlimmes passiert ist.

it3: (belast3): Normalerweise überstehe ich schwierige Zeiten ohne größere Probleme.

it4: (belast4): Ich brauche tendenziell lange, um über Rückschläge hinwegzukommen.

st:

ao1: 1: stimme überhaupt nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: stimme vollkommen zu

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
               <zofar:transition target="CO_21" condition="zofar.asNumber(PRELOADhs_co)==1"/>
		<zofar:transition target="CO_21" condition="zofar.asNumber(vier_b)==1"/>
            <zofar:transition target="A_15"/>        
	</zofar:transitions>


hi:

\--------------------------------
