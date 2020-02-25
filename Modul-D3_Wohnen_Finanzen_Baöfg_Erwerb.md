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

kh2: ao14: Bitte geben Sie Ihre jeweiligen monatlichen Gesamteinnahmen an (0 bis 99999).

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

ao8: (festipartsons): anderes: [(festipartsonso); Eingabefeld: 50 Zeichen]

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

it1: (fausgmieto; feindmieto): Warmmiete inkl. Nebenkosten

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

kh3: ao15: Bitte geben Sie Ihre jeweiligen monatlichen Gesamtausgaben an (0 bis 99999).

kh4: ao15: Bitte geben Sie an, was andere monatlich insgesamt für Sie bezahlen (0 bis 99999).

fv:

hv:

fo1: “ich bezahle selbst” und “andere bezahlen für mich” bitte als Spaltenüberschriften über die erste bzw. zweite Spalte mit den Eingabefeldern setzen (und dabei bitte kleingeschrieben anfangen).

fo2: Bitte etwas Abstand zwischen den beiden Spalten.

fo3: Bitte Leerzeile/Abstand vor den Gesamtausgaben einziehen. 

tr: GOTO D3_9

hi1: Bitte kh1 für die Einzelausgabeposten der Spalte "Ich bezahle selbst" nutzen und kh2 für die Einzelausgabeposten der Spalte "Andere bezahlen für mich".

hi2: Bitte kh3 für die Gesamtausgaben der Spalte "Ich bezahle selbst" nutzen und kh4 für die Gesamtausgaben der Spalte "Andere bezahlen für mich".

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

ao1: (fmineinko): [number, 4-stellig: 1 TO 9999], Postfix: € 

mv:

ka:

vc:

av: 

kh: (fmineinko): Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 9999).

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

vn: etat (etat1 / etat2 / etat3)

qt: Tableau (Drop Down)

hl:

in: 

q1: Bitte geben Sie die Art Ihrer Erwerbstätigkeit an, der Sie im aktuellen Semester nachgehen.

q2: Bitte geben Sie die Art Ihrer Erwerbstätigkeit an, der Sie im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb nachgehen.

q3: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten nachzugehen. 
Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

q4: Sie haben angegeben, im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb mehreren Erwerbstätigkeiten nachzugehen. Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

is: 
it1: (etat1): [infield = Tätigkeit; Dropdown-Menü] 
it2: (etat2): [infield = Tätigkeit; Dropdown-Menü] 
it3: (etat3): [infield = Tätigkeit; Dropdown-Menü] 

st:
ao1: 1: Tätigkeit als studentische/ wissenschaftliche Hilfskraft im Bereich Forschung und Lehre
ao2: 2: Tätigkeit als studentische/ wissenschaftliche Hilfskraft im Bereich Verwaltung
ao3: 3: Jobben (z. B. in einer Fabrik, einem Büro, einer Kneipe, Babysitten, Nachhilfeunterricht)
ao4: 4: Tätigkeit, die einen Hochschulabschluss voraussetzt (ohne Hilfskraft)
ao5: 5: Tätigkeit, die einen beruflichen Ausbildungsabschluss voraussetzt
ao6: 6: Tätigkeit als Praktikant\*in 

mv: 

ka1: (it1): Art der Tätigkeit (Tätigkeit A)
ka2: (it2): Art der Tätigkeit (Tätigkeit B)
ka3: (it3): Art der Tätigkeit (Tätigkeit C)

vc1: SHOW q1 IF eaktsens = 2 AND sformdua != 1
vc2: SHOW q2 IF eaktsens = 2 AND sformdua = 1
vc3: SHOW q3 IF eaktsens = 3 | 4 AND sformdua != 1
vc4: SHOW q4 IF eaktsens = 3 | 4 AND sformdua = 1

vc5: SHOW it1 IF eaktsens = 2 | 3 | 4
vc6: SHOW it2 IF eaktsens = 3 | 4 
vc7: SHOW it3 IF eaktsens = 4 

vc8: SHOW ka1 TO ka2 IF eaktsens = 3 
vc9: SHOW ka1 TO ka3 IF eaktsens = 4   
av: 
kh: 

fv: 

hv: 

fo: 

tr: GOTO D3_20 IF sformberu=1 | sformdua=1;  
    GOTO D3_21 IF sformberu=0 | sformdua=0

hi: 



\--------------------------------

D3_20
=====

tc: sformberu = 1 | sformdua = 1 

vn1: jobbbds1; jobbbdso1; jobbbds2; jobbbdso2; 

qt: offene Abfrage / Einfachauswahl im Spaltenformat

hl:

in:

q: Welchen Beruf üben Sie aktuell aus? Bitte erläutern Sie die Tätigkeit kurz.

is: Falls Sie zurzeit nicht erwerbstätig sind, geben Sie bitte die Ihre zuletzt ausgeübte Tätigkeit an. 
#{layout.BREAK}
Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive Führungsaufgaben ein. Zum Beispiel:
-   Bankkaufmann/-frau (nicht: Angestellte/r) Beratung, Verkauf von Finanzprodukten, Abteilungsleitung
-   Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in) Zollfahndung, Einsatzplanung
-   Maschinenbauingenieur(in) (nicht: Ingenieur/in) Konstruktion, Optimierungsprozesse, Produktionsleitung

it:

st:

ao1: (jobbbdso1): Präfix: [infield = Berufsbezeichnung; 100 Zeichen]

ao2: (jobbbdso2): Präfix: [infield = Tätigkeitsbeschreibung; 100 Zeichen]

mv1: (jobbbds1): -11: nie berufstätig gewesen

mv2: (jobbbds2): -12: weiß ich nicht [EK]

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

vn: egr (egrfin1 / egrfin2 / egrfin3 / egrkar1 / egrkar2 / egrper1 / egrper2 / egrper3 / egrerf1 / egrerf2 / egralt1 / egralt2)

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

it2: (egrfin2): ... um mir mein Studium finanzieren zu können.

it3: (egrfin3): ... damit ich mir (etwas) mehr leisten kann.

it4: (egrkar1): ... um Kontakte für eine spätere Beschäftigung zu knüpfen.

it5: (egrkar2): ... um mich neben dem Studium weiter zu qualifizieren.

it6: (egrper1): ... damit ich meinen Horizont erweitern kann.

it7: (egrper2): ... um mehr über meine Stärken und Schwächen zu erfahren.

it8: (egrper3): ... um mich persönlich weiter zu entwickeln.

it9: (egrerf1): ... um praktische Erfahrungen zu sammeln.

it10: (egrerf2): ... um etwas Neues zu lernen und mich fortzubilden.

it11: (egralt1): ... um einen Beitrag zur Gesellschaft zu leisten.

it12: (egralt2): ... um anderen zu helfen.

st:

ao1: 1: trifft gar nicht zu

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

vn: zufr (zufrwohn /zufrlstand / zufrfinsit / zufrerw / zufrleb)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie aktuell mit …

is:

it1: (zufrwohn): ... Ihrer Wohnsituation?

it2: (zufrlstand): ... Ihrem Lebensstandard?

it3: (zufrfinsit): ... Ihrer finanziellen Situation?

it4: (zufrerw): ... Ihrer/Ihren Erwerbstätigkeit/en?

it5: (zufrleb): ... Ihrem Leben insgesamt?

st:

ao1: 1: gar nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc:

SHOW it4 IF eaktsens = 2 |3 | 4

av:

kh:

fv:

hv:

fo:

tr:  GOTO D1_9 IF mastersplit=3, 4, 9, 10, 14
     GOTO D2_6 IF mastersplit=5, 6, 11, 12

hi: Items bitte zufällig rotieren.
