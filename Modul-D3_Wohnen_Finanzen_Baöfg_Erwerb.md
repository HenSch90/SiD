\--------------------------------

D3_1
====

tc:

vn: wohnort

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wo wohnen Sie während der Vorlesungszeit?

is:

it:

st:

ao1: 1: ausschließlich am Hochschulort

ao2: 2: ausschließlich außerhalb des Hochschulortes

ao3: 3: am Hochschulort und außerhalb des Hochschulortes

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_3

hi:

\--------------------------------

D3_2
====

tc:

vn: wohnamio

qt: offene Frage

hl:

in:

q: Mit wie vielen Personen wohnen Sie insgesamt – also Sie selbst mit
eingeschlossen – zusammen?

is:

it:

st:

ao1: : (wohnamio), Präfix: [infield = Personenzahl; number]

mv:

ka:

vc:

av: (wohnamio): number 2 Stellen; 2 TO 15

kh: (wohnamio): Bitte geben Sie an, zu wie vielen Personen Sie insgesamt zusammenwohnen (2 bis 15).

fv:

hv:

fo:

tr: GOTO D3_4

hi: 

\--------------------------------

D3_3
====

tc:

vn: wohnplz; wohnplzort

qt: offene Angabe

hl:

in:

q1: Bitte geben Sie die Postleitzahl Ihres derzeitigen Hauptwohnsitzes an.

q2: Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an.

is:

it:

st:

ao1: : (wohnplz), Präfix [infield = PLZ; number] 

ao2: : (wohnplzort), Präfix [infield = Ort; 100 Zeichen]

mv:

ka:

vc:

av: (wohnplz): number 5 Stellen; 01000 TO 99999

kh: (wohnplz): Bitte geben Sie Ihre Postleitzahl an (01000 bis 99999).

fv:

hv:

fo: SHOW q2 and ao2 IF wohnplz = k. A. (--> soft forcing, also danach geht es normal weiter)

tr: GOTO A_53

hi: Bitte q1 und ao1 zusammen oberhalb von q2 und ao2 darstellen.

\--------------------------------

D3_4
====

tc:

vn: wohnqmw; wohnqmz

qt: offene Angabe

hl:

in:

q1: Wie groß ist Ihre Wohnung/Ihr Haus?

q2: Wie groß ist das von Ihnen genutzte Zimmer?

is:

it:

st:

ao1: : (wohnqmw), Präfix: [infield = qm²; number]

ao2: : (wohnqmz), Präfix: [infield = qm²; number]

mv:

ka:

vc: SHOW q2, ao2 IF wohnel=1 OR wohnwg=1 

av1: (wohnqmw): number 3 Stellen; 1 TO 999

av2: (wohnqmz): number 2 Stellen; 1 TO 99

kh1: (wohnqmw): Bitte geben Sie die Größe Ihrer Wohnung/Ihres Hauses an (1 bis 999).

kh1: (wohnqmz): Bitte geben Sie die Größe Ihres Zimmers an (1 bis 99).

fv:

hv:

fo:

tr: GOTO D3_5

hi:

\--------------------------------

D3_5
====

tc:

vn: wohnzust

qt: Einfachauswahl/5er-Skala mit horizontalen ao

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

vn: fein (feinelto / feinkino / feinparo / feinjobdso / feinjobo1 / feinjobo2 / feinspao / feinbafo / feinkredo / feinstio / feinekio / feinbest1 / feinbest2 / feinandq / feinandqo / feininsg)

qt: offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich pro Monat
während des Sommersemesters 2020 zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst
verfügen. Berücksichtigen Sie hier bitte ++nicht++, was z. B. Ihre Eltern
oder Ihr\*e Partner\*in für Sie direkt an Dritte zahlen (z. B. direkte
Überweisung der Miete an Ihre\*n Vermieter\*in).

#{layout.BREAK}#{layout.BREAK}

Sollten Sie Ihren Lebensunterhalt auch mit unregelmäßigen Einnahmen oder durch
früher erworbenes Geld (z. B. Ersparnisse) bestreiten, geben Sie bitte nur den
Betrag an, den Sie davon aktuell monatlich im Durchschnitt einsetzen.

it1: (feinelto): Eltern (bar auf die Hand/per Überweisung auf Ihr Konto)

it2: (feinkino): Kindergeld für Sie selbst (sofern nicht bereits bei
Geldbeträgen von den Eltern angegeben)

it3: (feinparo): Partner\*in (bar auf die Hand/per Überweisung auf Ihr Konto)

it4: (feinjobdso): Ausbildungsvergütung für Duales Studium

it5: (feinjobo1): Erwerbstätigkeit

it6: (feinjobo2): Verdienst aus weiteren Tätigkeiten außerhalb der Ausbildungsinstitution während des Dualen Studiums

it7: (feinspao): eigene Mittel (z. B. Ersparnisse, Erbe)

it8: (feinbafo): BAföG

it9: (feinkredo): Kredit(e)

it10: (feinstio): Stipendium

it11: (feinekio): Kindergeld/Unterhalt für Ihr(e) Kind(er)

it12: (feinbest1): Krankenversicherungsleistungen für technische Hilfsmittel

it13: (feinbest2): weitere spezifische Sozialleistungen im Zusammenhang mit einer gesundheitlichen Beeinträchtigung

it14: (feinandqo): Weitere Finanzierungsquelle(n), und zwar: 

#{layout.BREAK}#{layout.BREAK}

it15: (feininsg): ++Gesamteinnahmen++:


st:

ao1: : (feinelto), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao2: : (feinkino), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao3: : (feinparo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao4: : (feinjobdso), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao5: : (feinjobo1), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao6: : (feinjobo2), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao7: : (feinspao), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao8: : (feinbafo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao9: : (feinkredo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao10: : (feinstio), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao11: : (feinekio), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao12: : (feinbest1), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao13: : (feinbest2), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao14: : (feinandq; feinandqo), [50 Zeichen] Präfix [infield = Betrag; number] Suffix: € pro Monat

#{layout.BREAK}#{layout.BREAK}

ao15: : (feininsg), Präfix [infield = Betrag; number] Suffix: € pro Monat

mv:

ka:

vc1: SHOW it4/ao4 (feinjobdso) IF sformdua = 1 

vc2: SHOW it5/ao5 (feinjobo1) IF sformdua != 1

vc3: SHOW it6/ao6 (feinjobo2) IF  sformdua = 1 

vc3: SHOW it11/ao11 (feinekio) IF dkinja = 2

av1: ao1 TO ao14: number 4 Stellen; 0 TO 9999

av2: ao15: number 5 Stellen; 0 TO 99999

kh1: ao1 TO ao14: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (0 bis 9999)

kh2: ao15: Bitte geben Sie Ihre jeweiligen monatlichen Gesamteinnahmen an (0 bis 99999)

fv:

hv:

fo:

tr:

GOTO D3_7

hi: 

\--------------------------------

D3_7
====

tc:

vn: festipart (festipartnein / festipartdeut / festipartstuvolk / festipartpartei / festipartbegabt / festipartandstaat / festipartprivat / festipartsons / festipartsonso)

qt: Mehrfachauswahl

hl:

in:

q: Erhalten Sie aktuell ein Stipendium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (festipartnein): nein

ao2 (festipartdeut): ja, Deutschlandstipendium

ao3 (festipartstuvolk): ja, Stipendium der Studienstiftung des deutschen Volkes e. V.

ao4 (festipartpartei): ja, Stipendium einer parteinahen Stiftung

ao5 (festipartbegabt): ja, Stipendium eines anderen Begabtenförderungswerks

ao6 (festipartandstaat): ja, anderes mit staatlichen Mitteln finanziertes Stipendium (Geldgeber: Land, Kommune, Hochschule)

ao7 (festipartprivat): ja, Stipendium eines privaten Geldgebers (Industrie, Firma, privater Stifter)

ao8 (festipartsons): Ja, anderes und zwar: [(festipartsonso); Eingabefeld; 50 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_8

hi:

\--------------------------------

D3_8
====

tc:

vn1: fausg (fausgmieto / fausgerno / fausgkomo / fausgkleio / fausglerno / fausgmobo / fausggeso / fausgsemo / fausgstuo / fausgfreio / fausgkitaso / fausgkindso / fausgasso / fausgthilfo / fausandq / fausandqo) 

vn2: feind (feindmieto / feinderno / feindkomo / feindkleio / feindlerno / feindgmobo / feindgeso / feindgsemo / feindgstuo / feindgfreio / feindkitaso / feindkindso / feindgasso / feindgthilfo / feinandqu2 / feinandquo2)

vn3: fausinsg; feininsg2



qt: offene Angabe

hl:

in:

q: Bitte geben Sie an, welche Ausgaben Sie bzw. Dritte für Sie im Sommersemester 2020 monatlich
haben.

is1: "Dritte" meint bspw. Ihre Eltern, die Ihre Miete direkt an den Vermieter bezahlen. 

is2: Bitte geben Sie nur den jeweils auf Sie persönlich bezogenen Betrag an.

it1: (fausgmieto; feindmieto): Miete inkl. Nebenkosten (Strom, Heizung, (Ab-)Wasser usw.)

it2: (fausgerno; feinderno): Ernährung (Lebensmittel und Getränke, auch außer Haus)

it3: (fausgkomo; feindkomo): (Mobil)Telefon, Internet, Audio-/Videostreaming

it4: (fausgkleio; feindkleio): Kleidung

it5: (fausglerno; feindlerno): Lernmittel (z. B. Fachliteratur; aber nicht: einmalige Anschaffungskosten für PC, Instrument o. ä.)

it6: (fausgmobo; feindgmobo): Mobilität (z. B. Semesterticket, laufende Ausgaben für Kfz, öff. Verkehrsmittel)

it7: (fausggeso; feindgeso): Gesundheitskosten (z. B. Krankenversicherung, Medikamente, Therapiemaßnahmen)

it8: (fausgsemo; feindgsemo): Semesterbeitrag (ohne Semesterticket)

it9: (fausgstuo; feindgstuo): Studiengebühren (z. B. privates Studium, Langzeitgebühren, Zweitstudium)

it10: (fausgfreio; feindgfreio): Freizeit, Kultur und Sport

it11: (fausgkitaso; feindkitaso): Ausgaben Kinderbetreuung

it12: (fausgkindso; feindkindso): kinderbezogene Ausgaben für Drogerieartikel, Kleidung, Spielzeug

it13: (fausgasso; feindgasso): Ausgaben für personelle Assistenzen (z. B. Pflegeassistenz, Mitschreibkraft, Haushaltshilfe)

it14: (fausgthilfo; feindgthilfo): Ausgaben für technische Hilfsmittel (z. B. Screen Reader, Braille-Zeile, FM-Anlage)

it15: (fausandqo; feinandqo2): Weitere Ausgaben, und zwar:

#{layout.BREAK}#{layout.BREAK}

it16: (fausinsg; feininsg2): ++Gesamtausgaben++:


st:

ao1: : (fausgmieto; feindmieto), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao2: : (fausgerno; feinderno), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao3: : (fausgkomo; feindkomo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao4: : (fausgkleio; feindkleio), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao5: : (fausglerno; feindlerno), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao6: : (fausgmobo; feindgmobo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao7: : (fausggeso; feindgeso), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao8: : (fausgsemo; feindgsemo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao9: : (faugstuo; feindgstuo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao10: : (fausgfreio; feindgfreio), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao11: : (fausgkitaso; feindkitaso), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao12: : (fausgkindso; feindkindso), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao13: : (fausgasso; feindgasso), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao14: : (fausgthilfo; feindgthilfo), Präfix [infield = Betrag; number] Suffix: € pro Monat

ao15: : (fausandq; fausandqo; feinandq2; feinandqo2), [50 Zeichen] Präfix [infield = Betrag; number] Suffix: € pro Monat

#{layout.BREAK}#{layout.BREAK}

ao16: : (fausinsg; feininsg2), Präfix [infield = Betrag; number] Suffix: € pro Monat

mv:

ka:

vc1: SHOW it11 TO 12 IF dkinja = 2

vc2: SHOW is2 IF wohnal=!1

av1: ao1 TO ao15: number 4 Stellen; 0 TO 9999

av2: ao16: number 5 Stellen; 0 TO 99999

kh1: ao1 TO ao15: Bitte geben Sie Ihre jeweiligen monatlichen Ausgaben an (0 bis 9999)

kh2: ao16: Bitte geben Sie Ihre jeweiligen monatlichen Gesamtausgaben an (0 bis 99999)

fv:

hv:

fo:

tr: GOTO D3_9

hi1: “Ich bezahle selbst” und “Andere bezahlen für mich” bitte als Spaltenüberschriften.
hi2: Bitte etwas Abstand zwischen den beiden Spalten.
hi3: Bei "fausinsg" und "feininsg2" (Gesamtausgaben) bitte ebenfalls 2 offene Angabefelder in der Zeile. 

\--------------------------------

D3_9
=====

tc:

vn: fmineinko

qt: offene Angabe

hl:

in:

q: Wieviel Geld benötigen Sie mindestens pro Monat, um finanziell zurecht zu kommen?

is:

it:

st:

ao1: : (fmineinko), Präfix [infield = €; number] 

mv:

ka:

vc:

av: (fmineinko): number 4 stellig; 0 TO 9999

kh: Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (0 bis 9999).

fv:

hv:

fo:

tr: GOTO D3_10  IF feindgsemo > 0 OR feindgstuo > 0;  
    GOTO D3_11  IF feindgsemo = 0 AND feindgstuo = 0
    GOTO D3_11  IF feindgsemo = k. A. AND feindgstuo = k. A.

hi:

\--------------------------------

D3_10
=====

tc: IF feindgsemo > 0 | feindgstuo > 0

vn: fausgst (fausgstkelto / fausgstkparto / fausgstkarbo / fausgstkando)

qt: offene Angabe

hl:

in: 

q: Sie haben angegeben, dass Dritte Ihre Studienkosten (Semesterbeitrag bzw. Studiengebühren) übernehmen oder sich daran beteiligen.
#{layout.BREAK}
Davon bezahlen durchschnittlich im Monat …

is:

it1: ... meine Eltern für mich:

it2: ... mein*/e Partner*/in für mich:

it3: ... mein Arbeitgeber für mich:

it4: ... andere für mich:

st:

ao1: : (fausgstkelto), Präfix [infield = €; number] 

ao2: : (fausgstkparto), Präfix [infield = €; number] 

ao3: : (fausgstkarbo), Präfix [infield = €; number] 

ao4: : (fausgstkando), Präfix [infield = €; number] 

mv: 

ka: 

vc: 

av: ao1 TO ao4: number 4 stellig; 0 TO 9999

kh: Bitte geben Sie den Betrag an, mit dem Sie bei Ihren Studienkosten unterstützt werden (0 bis 9999).

fv: 

hv: 

fo: 

tr: GOTO D3_11

hi: 

\--------------------------------

D3_11
=====

tc:

vn: fsit (fsitzum1 / fsitzum2 / fsitzum3 / fsitelt1 / fsitelt2 / fsitelt3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen Sie und Ihre finanzielle
Situation zu?

is:

it1: (fsitzum1): Ich verfüge zurzeit über ausreichend finanzielle Mittel, um
meine monatlichen Ausgaben zu decken.

it2: (fsitzum2): Ich habe zurzeit finanzielle Schwierigkeiten.

it3: (fsitzum3): Die Finanzierung meines Lebensunterhalts während meines
Studiums ist sichergestellt.

it4: (fsitelt1): Meine Eltern unterstützen mich finanziell so gut sie können.

it5: (fsitelt2): Ich habe den Eindruck, meine Eltern finanziell zu überfordern.

it6: (fsitelt3): Ich will finanziell nicht auf meine Eltern angewiesen sein.

st:

ao1: 1: trifft gar nicht zu

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

tr: GOTO D3_12

hi: Items bitte zufällig rotieren.

\--------------------------------

D3_12
=====

tc:

vn: feinstf (feinstf1 / feinstf2 / feinstf3 / feinstf4 / feinstf5 / feinstf6 / feinstf7 / feinstf8)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao
hl:

in:

q: Inwieweit treffen die folgenden Aussagen zum Umgang mit Geld auf Sie zu?

is:

it1: (feinstf1): Ich gebe Geld lieber sofort aus, als es für einen späteren
Zeitpunkt zu sparen.

it2: (feinstf2): Ich kümmere mich sorgfältig um meine finanziellen
Angelegenheiten.

it3: (feinstf3): Es gelingt mir, mit meinem Geld auszukommen.

it4: (feinstf4): Es belastet mich, mir Gedanken über meine finanzielle Zukunft
zu machen.

it5: (feinstf5): Bevor ich etwas kaufe, vergleiche ich immer die Preise.

it6: (feinstf6): Ich achte darauf, dass ich Geld für schlechte Zeiten habe.

it7: (feinstf7): Ich empfinde es als sehr anstrengend, den Überblick über meine
Finanzen zu behalten.

it8: (feinstf8): Ich neige dazu, im Hier und Jetzt zu leben und lasse die
Zukunft auf mich zukommen.

st:

ao1: 1: trifft gar nicht zu

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

qt: Einfachauswahl

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

qt: Einfachauswahl

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

qt: Einfachauswahl

hl:

in:

q: Haben Sie früher schon einmal einen Antrag auf BAföG gestellt?

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

qt: Mehrfachnennung/offene Angabe 

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

ao2: (fbafkelt): Das Einkommen der Eltern bzw. des Ehepartners/der Ehepartnerin war zu hoch.

ao3: (fbafkein): Das eigene Einkommen/Vermögen ist zu hoch.

ao4: (fbafkein): Das eigene Einkommen/Vermögen war zu hoch.

ao5: (fbafkfhd): Die Förderungshöchstdauer wurde überschritten.

ao6: (fbafktw): Das Studienfach wurde gewechselt.

ao7: (fbafkleis): Die notwendige Leistungsbescheinigung konnte nicht erbracht werden.

ao8: (fbafkalt): Bei Studienbeginn war die maßgebliche Altersgrenze bereits überschritten.

ao9: (fbafkzwei): Das jetzige Studium ist eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium).

ao10: (fbafkzwei): Das  Studium war eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium).

ao11: (fbafkweni): Der zu erwartende Förderbeitrag ist so gering, dass es sich nicht lohnt.

ao12: (fbafkweni): Der zu erwartende Förderbeitrag war so gering, dass es sich nicht lohnte.

ao13: (fbafkschu): Ich will keine Schulden machen.

ao14: (fbafkschu): Ich wollte keine Schulden machen.

ao15: (fbafand): Andere Gründe, und zwar: [(fbafando) 50 Zeichen] 

mv:

ka:

vc1: SHOW q1 IF (fbafja = 1) AND (fbafex = 1 | k. A.)

vc2: SHOW q2 IF (fbafja = 2)

vc3: SHOW q3 IF (fbafja = 1) AND (fbafex = 2 | 3)

vc4: SHOW q4 IF (fbafja = 1) AND (fbafex = 4)

vc5: SHOW ao1, ao3, ao5, ao6, ao7, ao8, ao9, ao11, ao13, ao15 IF (fbafja = 1) AND (fbafex = 1 | k. A.)

vc6: SHOW ao1, ao3, ao5, ao6, ao7, ao8, ao9, ao15 IF (fbafja = 2)

vc7: SHOW ao2, ao4, ao5, ao6, ao7, ao8, ao10, ao15 IF (fbafja = 1) AND (fbafex = 2 | 3)

vc8: SHOW ao2, ao4, ao5, ao6, ao7, ao8, ao10, ao12, ao14, ao15 IF (fbafja = 1) AND (fbafex = 4)

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

qt: Einfachauswahl

hl:

in:

q: Wird das BAföG unabhängig vom Einkommen Ihrer Eltern gewährt?

is:

it:

st:

ao1: 0: nein

ao2: 1: ja

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

q2: Bitte geben Sie die Art Ihrer Erwerbstätigkeit an, der Sie im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb  nachgehen.

q3: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten nachzugehen. 
Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

q4: Sie haben angegeben, im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb mehreren anderen Erwerbstätigkeiten nachzugehen. Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

is: 
it1: (etat1), Präfix [infield = Art der Tätigkeit; Dropdown-Menü] 
it2: (etat2), Präfix [infield = Art der Tätigkeit; Dropdown-Menü] 
it3: (etat3), Präfix [infield = Art der Tätigkeit; Dropdown-Menü] 

st:
ao1: 1: : Tätigkeit als studentische/wissenschaftliche Hilfskraft im Bereich Forschung und Lehre
ao2: 2: : Tätigkeit als studentische/wissenschaftliche Hilfskraft im Bereich Verwaltung
ao3: 3: : Jobben (z. B. in einer Fabrik, einem Büro, einer Kneipe, Babysitten, Nachhilfeunterricht)
ao4: 4: : Tätigkeit, die einen Hochschulabschluss voraussetzt (ohne Hilfskraft)
ao5: 5: : Tätigkeit, die einen beruflichen Ausbildungsabschluss voraussetzt
ao6: 6: : Tätigkeit als Praktikant\*in 

mv: 

ka1: (it1): Tätigkeit A
ka2: (it2): Tätigkeit B
ka3: (it3): Tätigkeit C 

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
    GOTO D3_21 IF ELSE

hi: 



\--------------------------------

D3_20
=====

tc: sformberu = 1 | sformdua = 1 

vn1: jobbbds1, jobbbdso1, jobbbds2, jobbbdso2, 

qt: offene Abfrage / Einfachauswahl im Spaltenformat

hl:

in:

q: Welchen Beruf üben Sie aktuell aus? Bitte erläutern Sie die Tätigkeit kurz.

is: Falls Sie zurzeit nicht erwerbstätig sind, geben Sie bitte Ihre zuletzt ausgeübte Tätigkeit an. 
#{layout.BREAK}
Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive Führungsaufgaben ein. Zum Beispiel:
-   Bankkaufmann/-frau (nicht: Angestellte/r) Beratung, Verkauf von Finanzprodukten, Abteilungsleitung
-   Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in) Zollfahndung, Einsatzplanung
-   Maschinenbauingenieur\*in (nicht: Ingenieur\*in) Konstruktion, Optimierungsprozesse, Produktionsleitung

it:

st:

ao1: (jobbbdso1), Präfix: [infield = Berufsbezeichnung; 100 Zeichen]

ao2: (jobbbdso2), Präfix: [infield = Tätigkeitsbeschreibung; 100 Zeichen]

ao3: (jobbbds1), -11: : nie berufstätig gewesen [EK]

ao4: (jobbbds2), -12: : weiß ich nicht [EK]

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

ao3: 3:

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

hi:
