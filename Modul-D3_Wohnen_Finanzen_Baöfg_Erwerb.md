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

is:

it:

st:

ao1: (wohnamio): [number, 2-stellig: 1 To 15], Postfix: Person(en)

ao2: (wohnqmw): [number, 3-stellig: 1 TO 999], Postfix: m²

ao3: (wohnqmz): [number, 2-stellig: 1 TO 99], Postfix: m²

mv:

ka:

vc: SHOW q3, ao3 IF wohnel=1 OR wohnwg=1 

av: 

kh1: (wohnamio): Bitte geben Sie die Anzahl an Personen an, mit denen Sie zusammenwohnen (1 bis 15).

kh2: (wohnqmw): Bitte geben Sie die Größe Ihrer Wohnung/Ihres Hauses an (1 bis 999).

kh3: (wohnqmz): Bitte geben Sie die Größe Ihres Zimmers an (1 bis 99).


fv:

hv:

fo: Auf der Seite als erstes q1/ao1 zusammen darstellen. Darunter dann q2/ao2 zusammen darstellen und darunter dann ggf. q3/ao3 zusammen einblenden.

tr: GOTO D3_5

hi: 

\--------------------------------

D3_5
====

tc:

vn: wohnzust

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Wie würden Sie den Allgemeinzustand Ihrer Wohnung einschätzen?

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

tr: GOTO B2_5 if mastersplit=9, 10, 11, 12
    GOTO B1_5 if mastersplit=3, 4, 5, 6,
    GOTO D3_13 if mastersplit=14

hi:

\--------------------------------

D3_6
====

tc:

vn: fein (feinelto / feinekio / feinparo / feinjobo1 / feinjobdso / feinjobo2 / feinspao / feinbafo / feinkredo / feinstio /  feinwaiso / feinbest / feinandq / feinandqo / feininsg)

qt: offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich ++pro Monat++
während des Sommersemesters 2020 zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst
verfügen. ++Nicht++ gemeint sind Beträge, die z. B. von Ihren Eltern für Sie direkt 
an Dritte überwiesen werden (z. B. Überweisung der Miete durch Ihre Eltern).

it1: (feinelto): Eltern und Verwandte

it2: (feinekio): Kindergeld/Unterhalt für Ihr(e) Kind(er)

it3: (feinparo): Partner\*in 

it4: (feinjobo1): Erwerbstätigkeit

it5: (feinjobdso): Ausbildungsvergütung für Duales Studium

it6: (feinjobo2): Verdienst aus weiteren Tätigkeiten außerhalb der Ausbildung

it7: (feinspao): eigene Mittel (z. B. Ersparnisse, Erbe)

it8: (feinbafo): BAföG

it9: (feinkredo): Kredit(e)

it10: (feinstio): Stipendium

it11: (feinwaiso): Waisengeld/Waisenrente

it12: (feinbest): Sozialleistungen im Zusammenhang mit Ihrer gesundheitlichen Beeinträchtigung

it13: (feinandq): Weitere Finanzierungsquelle(n), und zwar: 

#{layout.BREAK}#{layout.BREAK } 

it14: (feininsg): ++Gesamteinnahmen++:


st:

ao1: (feinelto): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao2: (feinekio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3: (feinparo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4: (feinjobo1): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5: (feinjobdso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6: (feinjobo2): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao7: (feinspao): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao8: (feinbafo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao9: (feinkredo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao10: (feinstio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao11: (feinwaiso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao12: (feinbest): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao13: (feinandq; feinandqo): [50 Zeichen] [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

#{layout.BREAK}#{layout.BREAK } 

ao14: (feininsg), [infield = € pro Monat; number, 5-stellig: 0 TO 99999]

mv:

ka:

vc1: SHOW it2/ao2 (feinekio) IF dkinja = 2

vc2: SHOW it4/ao4 (feinjobo1) IF sformdua != 1

vc3: SHOW it5/ao5 (feinjobdso) IF sformdua = 1 

vc4: SHOW it6/ao6 (feinjobo2) IF  sformdua = 1 

vc5: SHOW it12/ao12 (feinbest) IF  h_gartcount >= 1 

av: 

kh1: ao1 TO ao13: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (0 bis 9999).

kh2: ao14: Bitte geben Sie Ihre monatlichen Gesamteinnahmen an (0 bis 99999).

fv:

hv:

fo1: “Betrag” bitte als Spaltenüberschrift über die Spalte mit den Eingabefeldern.

fo2: Bitte Leerzeile/Abstand vor den Gesamteinnahmen einziehen. 

tr:

GOTO D3_7

hi: 

\--------------------------------

D3_7
====

tc:

vn: festipart (festipartnein / festipartdeut / festipartstuvolk / festipartpartei / festipartbegabt / festipartandstaat / festipartprivat / festipartsons / festipartsonso)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Erhalten Sie aktuell ein Stipendium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (festipartnein): nein [EK]

ao2: (festipartdeut): Deutschlandstipendium

ao3: (festipartstuvolk): Stipendium der Studienstiftung des deutschen Volkes e. V.

ao4: (festipartpartei): Stipendium einer parteinahen Stiftung

ao5: (festipartbegabt): Stipendium eines anderen Begabtenförderungswerkes

ao6: (festipartandstaat): anderes mit staatlichen Mitteln finanziertes Stipendium (z. B. Hochschule, Land)

ao7: (festipartprivat): Stipendium eines privaten Geldgebers (z. B. Industrie, private\*r Stifter\*in)

ao8: (festipartsons): anderes: [(festipartsonso); 50 Zeichen]

mv:

ka: (ao2 TO ao8): ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: "ja, und zwar:" zwischen ao1 und ao2 setzen.

tr: GOTO D3_8

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

q: Bitte geben Sie an, welche Ausgaben Sie bzw. Andere für Sie im Sommersemester 2020 ++monatlich++ haben.

is1: "Andere" meint bspw. die Überweisung der Miete durch Ihre Eltern. 

is2: Bitte geben Sie nur den jeweils auf Sie persönlich bezogenen Betrag an.

it1: (fausgmieto; feindmieto): Warmmiete (inkl. Nebenkosten)

it2: (fausgerno; feinderno): Ernährung 

it3: (fausgkomo; feindkomo): Telefon, Internet

it4: (fausgkleio; feindkleio): Kleidung

it5: (fausglerno; feindlerno): Lernmittel (z. B. Fachliteratur)

it6: (fausggeso; feindgeso): Gesundheitskosten (z. B. Krankenversicherung, Medikamente, Therapien)

it7: (fausgmobo; feindmobo): Mobilitätskosten (z. B. Auto, Bahn)

it8: (fausgsemo; feindgsemo): Semesterbeitrag (inkl. Semesterticket)

it9: (fausgstuo; feindstuo): Studiengebühren 

it10: (fausgfreio; feindfreio): Freizeit, Kultur und Sport

it11: (fausgkitaso; feindkitaso): Ausgaben für Kinderbetreuung

it12: (fausgkindso; feindkindso): kinderbezogene Ausgaben (Drogerieartikel, Kleidung usw.)

it13: (fausgasso; feindasso): Ausgaben für personelle Assistenzen im Zusammenhang mit einer Beeinträchtigung (z. B. Pflegeassistenz, Mitschreibkraft)

it14: (fausandq): Weitere Ausgaben, und zwar:

#{layout.BREAK}#{layout.BREAK}

it15: (fausinsg; feininsg2): ++Gesamtausgaben++:


st:

ao1: (fausgmieto; feindmieto): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao2: (fausgerno; feinderno): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3: (fausgkomo; feindkomo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4: (fausgkleio; feindkleio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5: (fausglerno; feindlerno): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6: (fausggeso; feindgeso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao7: (fausgmobo; feindmobo): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao8: (fausgsemo; feindgsemo): [infield = € pro Semester; number, 4-stellig: 0 TO 9999]

ao9: (fausgstuo; feindstuo): [infield = € pro Semester; number, 4-stellig: 0 TO 9999]

ao10: (fausgfreio; feindfreio): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao11: (fausgkitaso; feindkitaso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao12: (fausgkindso; feindkindso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao13: (fausgasso; feindasso): [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao14: (fausandqo; feinandqo2): [50 Zeichen] [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

#{layout.BREAK}#{layout.BREAK}

ao15: (fausinsg; feininsg2): [infield = € pro Monat; number, 5-stellig: 0 TO 99999]

mv:

ka:

vc1: SHOW it11/ao11 TO it12/ao12 IF dkinja = 2

vc2: SHOW it13/ao13 IF h_gartcount >= 1 

vc3: SHOW is2 IF wohnal=!1

av: 

kh1: ao1 TO ao14: Bitte geben Sie Ihre jeweiligen monatlichen Ausgaben an (0 bis 9999).

kh2: ao1 TO ao14: Bitte geben Sie an, was andere monatlich jeweils für Sie bezahlen (0 bis 9999).

kh3: ao15: Bitte geben Sie Ihre monatlichen Gesamtausgaben an (0 bis 99999).

kh4: ao15: Bitte geben Sie an, was andere monatlich insgesamt für Sie bezahlen (0 bis 99999).

fv:

hv:

fo1: “ich bezahle selbst” und “andere bezahlen für mich” bitte als Spaltenüberschriften über die erste bzw. zweite Spalte mit den Eingabefeldern setzen (und dabei bitte kleingeschrieben anfangen).

fo2: Bitte etwas Abstand zwischen den beiden Spalten.

fo3: Bitte Leerzeile/Abstand vor den Gesamtausgaben einziehen. 

tr: GOTO D3_9

hi1: Bitte kh1 für die Einzelausgabeposten der Spalte "ich bezahle selbst" nutzen und kh2 für die Einzelausgabeposten der Spalte "andere bezahlen für mich".

hi2: Bitte kh3 für die Gesamtausgaben der Spalte "ich bezahle selbst" nutzen und kh4 für die Gesamtausgaben der Spalte "andere bezahlen für mich".

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

ao1: (fmineinko): [number, 5-stellig: 1 TO 99999], Postfix: € 

mv:

ka:

vc:

av: 

kh: (fmineinko): Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 99999).

fv:

hv:

fo:

tr: GOTO D3_11

hi:

\--------------------------------

D3_11
=====

tc:

vn: fsit (fsitzum1 / fsitzum2 / fsitzum3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie und Ihre finanzielle Situation zu?

is:

it1: (fsitzum1): Die Finanzierung meines Lebensunterhalts während des Studiums ist sichergestellt.

it2: (fsitzum2): Ich habe zurzeit finanzielle Schwierigkeiten.

it3: (fsitzum3): Im Großen und Ganzen gelingt es mir, mit meinem Geld auszukommen.

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

tr: GOTO A_54

hi: Items bitte zufällig rotieren.

\--------------------------------

D3_13
=====

tc:

vn: fbafja

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Werden Sie im Sommersemester 2020 nach dem BAföG gefördert?

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

tr: GOTO D3_13b

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
GOTO D3_14 IF fbafja = 1

GOTO D3_15 IF fbafja = 2

GOTO D3_17 IF fbafja = 4

GOTO D3_6 IF fbafja = 3 OR fbafja = k. A.

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

ao2: 2: Ja, ich habe einmal einen Antrag gestellt, der wurde aber abgelehnt.

ao3: 3: Ja, in früheren Semestern wurde ich auch gefördert, ein Antrag auf
Weiterförderung wurde dann aber abgelehnt.

ao4: 4: Ja, in früheren Semestern wurde ich auch gefördert, habe dann aber
keinen Antrag auf Weiterförderung mehr gestellt.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_16

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

ao3: 3: Ja, in früheren Semestern wurde ich auch gefördert.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_16

hi:

\--------------------------------

D3_16
=====

tc: IF fbafja = 1 \| 2 

vn: fbaf (fbafkelt / fbafkein / fbafkfhd / fbafktw / fbafkleis / fbafkalt / fbafkzwei / fbafkweni / fabfkschu / fbafand / fbafando)

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

ao6: (fbafkalt): Bei Studienbeginn war die maßgebliche Altersgrenze bereits überschritten.

ao7: (fbafkzwei): Das jetzige Studium ist eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium).

ao8: (fbafkweni): Der zu erwartende Förderbetrag ist so gering, dass es sich nicht lohnt.

ao9: (fbafkschu): Ich will keine Schulden machen.

ao10: (fbafand): Andere Gründe, und zwar: [(fbafando) 50 Zeichen] 

mv:

ka:

vc1: SHOW q1 IF (fbafja = 1) AND (fbafex = 1 | k. A.)

vc2: SHOW q2 IF (fbafja = 2)

vc3: SHOW q3 IF (fbafja = 1) AND (fbafex = 2 | 3)

vc4: SHOW q4 IF (fbafja = 1) AND (fbafex = 4)

vc5: DON’T SHOW ao8, ao9 IF (fbafja = 2)

vc6: DON’T SHOW ao8, ao9 IF (fbafja = 1) AND (fbafex = 2 | 3)


av:

kh:

fv:

hv:

fo:

GOTO D3_6

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

tr: GOTO D3_18

hi:

\--------------------------------

D3_18
=====

tc: IF fbafja = 4 

vn: fbabf (fbafkv / fbafkin)

qt: Mehrfachauswahl

hl:

in:

q: Ist in Ihrem Förderungsbetrag ein Zuschlag enthalten für …

is:

it:

st:

ao1: (fbafkv): … Ihre Kranken- und Pflegeversicherung?

ao2: (fbafkin): … die Betreuung Ihres Kindes/Ihrer Kinder?

ao3: (fbafkin): … die Betreuung Ihres Kindes?

ao4: (fbafkin): … die Betreuung Ihrer Kinder?

mv:

ka:

vc1: SHOW ao2 IF dkinanz = k. A.

vc2: SHOW ao3 IF dkinanz = 1

vc3: SHOW ao4 IF dkinanz \> 1 

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_6

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

is1: Bitte geben Sie die Art Ihrer Erwerbstätigkeit und deren inhaltliche Nähe zu den Studieninhalten an.

is2: Bitte geben Sie die Art Ihrer jeweiligen Erwerbstätigkeiten und deren inhaltliche Nähe zu den Studieninhalten an. Sollten Sie mehr als drei Erwerbstätigkeiten ausüben, dann beziehen Sie Ihre Angaben bitte auf die drei Haupttätigkeiten.


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

tr: GOTO D3_20 IF sformberu=1 | sformdua=1;  
    GOTO D3_21 IF sformberu=0 & sformdua=0 & eaktsens > 1
    GOTO D3_22 IF sformberu=0 & sformdua=0 & eaktsens = 1 | k. A.

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

\-   Bankkaufmann/-frau (nicht: Angestellte\*r)

\-   Zollbeamtin/-beamter (nicht: Beamtin bzw. Beamter)

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

tr: GOTO D3_21 IF (eaktsens > 1)
    GOTO D3_22 IF (eaktsens = 1 | k. A.)

hi:

\--------------------------------

D3_21
=====

tc: IF eaktsens = 2 \|3 \|4

vn: egr (egrfin1 / egrfin2 / egrfin3 / egrfin4 / egrkar1 / egrkar2 / egrkar3 / egrerf1 / egralt1 / egralt2)

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

it4: (egralt2): ... um anderen zu helfen.

it5: (egrfin2): ... um mir mein Studium finanzieren zu können.

it6: (egrerf1): ... um praktische Erfahrungen zu sammeln.

it7: (egrkar3) ... um meine Berufschancen zu verbessern.

it8: (egralt1): ... um einen Beitrag zur Gesellschaft zu leisten.

it9: (egrfin4) ... um finanziell unabhängig von den Eltern zu sein.

it10: (egrfin3): ... damit ich mir etwas mehr leisten kann.



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

tr: GOTO D3_22

hi: Items bitte zufällig rotieren.

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

vc2: SHOW it5 IF h_gartcount >= 1 

vc3: SHOW it6 IF eaktsens = 2 |3 | 4

vc4: SHOW it7 IF pflegang = 1 

av:

kh:

fv:

hv:

fo:

tr:  GOTO D3_23

hi:

\--------------------------------

D3_23
====

tc:

vn: allges

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Wie ist Ihr Gesundheitszustand im Allgemeinen?

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

tr: GOTO D1_27

hi:

\--------------------------------

D1_27 
===

tc:

vn: feel (feelstress / feellast)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie haben Sie sich in den letzten vier Wochen überwiegend gefühlt?

is:

it1: (feelstress): gestresst

it2: (feellast): überlastet

st:

ao1: 1: gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr stark

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_28

hi:

\--------------------------------

D1_28 
===

tc: IF NOT gartpsy=1

vn: dep (depspass / depglue / depschw / depgedr)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie fühlen Sie sich im Allgemeinen?

is:

it1: (depspass): Das Leben macht mir Spaß.

it2: (depglue): Ich bin glücklich.

it3: (depschw): Meine Stimmung ist schwermütig.

it4: (depgedr): Ich bin in gedrückter Stimmung.

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

tr: GOTO D1_9 IF mastersplit=3, 4, 9, 10, 14
    GOTO D2_6 IF mastersplit=5, 6, 11, 12

hi1: Items bitte zufällig rotieren.
