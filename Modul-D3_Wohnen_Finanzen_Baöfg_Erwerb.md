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

vn: wohnami, wohnamio

qt: offene Frage

hl:

in:

q: Zu wie vielen Personen wohnen Sie insgesamt – also Sie selbst mit
eingeschlossen – zusammen?

is:

it:

st:

ao1: : (wohnami) Eingaabefeld, 2 Stellen, Präfix: [infield = Personenzahl; (wohnamio)]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_4

hi: 

\--------------------------------

D3_3
====

tc:

vn: wohnplz; wohnplzo; wohnplzort; wohnplzorto

qt: offene Angabe

hl:

in:

q1: Bitte geben Sie die Postleitzahl Ihres derzeitigen Wohnortes am Hochschulort an.

q2: Bitte geben Sie die Postleitzahl Ihres derzeitigen Wohnortes außerhalb des Hochschulortes an.

q3: Falls Sie die Postleitzahl nicht kennen, geben Sie bitten den Ort an.

is:

it:

st:

ao1: : (wohnplz), Präfix [infield = PLZ; 5 Stellen; number (wohnplzo)] 

ao2: : (wohnplzort), Präfix [infield = Ort; 100 Zeichen (wohnplzorto)]

mv:

ka:

vc1: SHOW q1 and ao1 IF wohnort = 1 | 3

vc1: SHOW q2 and ao1 IF wohnort = 2

av1: ao1 (wohnplz) number: 01000 TO 99999

kh1: (wohnplzo): Bitte geben Sie Ihre Postleitzahl an (01000 bis 99999).

fv:

hv:

fo: SHOW q3 and ao2 IF wohnplzo = k. A. (--> soft forcing, also danach geht es normal weiter)

tr: GOTO A_53

hi:

\--------------------------------

D3_4
====

tc:

vn: wohnqmw; wohnqmwo; wohnqmz; wohnqmzo

qt: offene Angabe

hl:

in:

q1: Wie groß ist Ihre Wohnung/Ihr Haus?

q2: Wie groß ist das von Ihnen genutzte Zimmer?

is:

it:

st:

ao1: (wohnqmw),  Präfix: [infield = qm²; 3 Stellen; number (wohnqmwo)]

ao2: (wohnqmz), Präfix: [infield = qm²; 2 Stellen; number (wohnqmzo)]

mv:

ka:

vc: SHOW q2, ao2 IF wohnel=1 OR wohnwg=1 

av1: number: 3 stellig : 1 TO 999

av2: number: 2 stellig : 1 TO 99

kh:

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

vn: feinelto; feinkino; feinparo; feinjobdso; feinjobo; feinspao; feinbafo; feinkredo; feinstio; feinekio; feinbest1; feinbest2; feinandq; feinandqo; feininsg; feininsgo

qt: offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich pro Monat
während des Sommersemesters 2020 zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst
verfügen. Berücksichtigen Sie hier bitte ++nicht++, was z. B. Ihre Eltern
oder Ihr(e) Partner\*in für Sie direkt an Dritte zahlen (z. B. direkte
Überweisung der Miete an Ihren Vermieter).

Leerzeile

Sollten Sie Ihren Lebensunterhalt auch mit unregelmäßigen Einnahmen oder durch
früher erworbenes Geld (z. B. Ersparnisse) bestreiten, geben Sie bitte nur den
Betrag an, den Sie davon aktuell monatlich im Durchschnitt einsetzen.

it1: (feinelto): Eltern (bar auf die Hand/per Überweisung auf Ihr Konto)

it2: (feinkino): Kindergeld für Sie selbst (sofern nicht bereits bei
Geldbeträgen von den Eltern angegeben)

it3: ( feinparo): Partner*in (bar auf die Hand/per Überweisung auf Ihr Konto)

it4: (feinjobdso): Ausbildungsvergütung für Duales Studium

it5: (feinjobo): Erwerbstätigkeit

it6: (feinjobo): Verdienst aus weiteren Tätigkeiten außerhalb der Ausbildungsinstitution während des Dualen Studiums

it7: (feinspao): eigene Mittel (z. B. Ersparnisse, Erbe)

it8: (feinbafo): BAföG

it9: (feinkredo): Kredit(e)

it10: (feinstio): Stipendium

it11: (feinekio): Kindergeld/Unterhalt für Ihr(e) Kind(er)

it12: (feinbest1): Krankenversicherungsleistungen für technische Hilfsmittel

it13: (feinbest2): weitere spezifische Sozialleistungen im Zusammenhang mit meiner gesundheitlichen Beeinträchtigung

it14: (feinandq): Weitere Finanzierungsquelle(n), und zwar: (offene Angabe: [feinandqo] 50 Zeichen) 

[Trennlinie]

it15: (feininsg): Gesamteinnahmen: (offene Angabe: [feininsgo] 5 Zeichen) 


st:

ao1: 4 Stellen, Präfix infield = Betrag [feinelto] Suffix: [number] € pro Monat

ao2: 4 Stellen, Präfix infield = Betrag [feinkino] Suffix: [number]€ pro Monat

ao3: 4 Stellen, Präfix infield = Betrag [feinparo] Suffix: [number]€ pro Monat

ao4: 4 Stellen, Präfix infield = Betrag [feinjobdso] Suffix: [number]€ pro Monat

ao5: 4 Stellen, Präfix infield = Betrag [feinjobo] Suffix: [number]€ pro Monat

ao6: 4 Stellen, Präfix infield = Betrag [feinspao] Suffix: [number]€ pro Monat

ao7: 4 Stellen, Präfix infield = Betrag [feinbafo] Suffix: [number]€ pro Monat

ao8: 4 Stellen, Präfix infield = Betrag [feinkredo] Suffix: [number]€ pro Monat

ao9: 4 Stellen, Präfix infield = Betrag [feinstio] Suffix: [number]€ pro Monat

ao10: 4 Stellen, Präfix infield = Betrag [feinekio] Suffix: [number]€ pro Monat

ao11: 4 Stellen, Präfix infield = Betrag [feinbest1] Suffix: [number]€ pro Monat

ao12: 4 Stellen, Präfix infield = Betrag [feinbest2] Suffix: [number]€ pro Monat

ao13: 4 Stellen, Präfix infield = Betrag [feinandqo] Suffix: [number]€ pro Monat

ao14: 5 Stellen, Präfix infield = Betrag [feininsgo] Suffix: [number]€ pro Monat

mv:

ka:

vc1: SHOW it4 (feinjobdso) if sformdua = 1 

vc2: SHOW it5 (feinjobo) if sformdua != 1

vc3: SHOW it6 (feinjobo) IF  sformdua = 1 

vc3: SHOW it11 (feinekio) if dkinja=2

vc4: SHOW it12 – it13 (feinbest1 – feinbest2) if [gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1] 

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (1 bis 9999)

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

ao8 (festipartsons): Ja, anderes und zwar: [festipartsonso] (Eingabefeld; 50 Zeichen)

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

vn1: „Ich bezahle selbst“ [fausg]: (fausgmiet; fausgmieto; fausgerno; fausgerno; fausgkomo; fausgkleio; fausglerno; fausgmobo; fausggeso; fausgsemo; fausgstuo; fausffreio; fausgkitaso; fausgkindso; fausgasso; fausgthilfo; fausandqo) 

vn2: „Dritte (Eltern, Partner\*in etc) bezahlen direkt [feind]: (feindmieto; feinderno, feindkomo; feindkleio; feindlerno; feindgmobo, feindgeso; feindgsemo; feindgstuo; feindgfreio; feindkitaso; feindkindso; feindgasso; feindgthilfo; feinandquo2)

vn3: fausinsg



qt: offene Angabe

hl:

in:

q: Bitte geben Sie an, welche Ausgaben Sie bzw. Dritte für Sie (z. B. Eltern
bezahlen Ihre Miete direkt an den Vermieter) im Sommersemester 2020 monatlich
haben.

is1: "Dritte bezahlen direkt" meint bspw. Ihre Eltern, die Ihre Miete direkt an den Vermieter bezahlen. 

is2: Bitte geben Sie nur den jeweils auf Sie persönlich bezogenen Betrag an.

it1: (fausgmieto; feindmieto): Miete inkl. Nebenkosten (Strom, Heizung, (Ab-)Wasser usw.)

it2: (fausgerno; feinderno): Ernährung (Lebensmittel und Getränke, auch außer Haus)

it3: (fausgkomo; feindkomo): (Mobil)Telefon, Internet, Audio-/Videostreaming

it4: (fausgkleio; feindkleio): Kleidung

it5: (fausglerno; feindlerno): Lernmittel (z. B. Fachliteratur; aber nicht: einmalige Anschaffungskosten für PC, Instrument o. ä.)

it6: (fausgmobo; feindgmobo): Mobilität (z. B. Semesterticket, laufende Ausgaben für Kfz, öff. Verkehrsmittel)

it7: (fausggeso; feindgeso): Gesundheitskosten (z. B. Krankenversicherung, Medikamente, Therapiemaßnahmen)

it8: (fausgsemo; feindgsemo): Semesterbeitrag (ohne Semesterticket)

it9: (faugstuo; feindgstuo): Studiengebühren (z. B. privates Studium, Langzeitgebühren, Zweitstudium)

it10: (fausgfreio; feindgfreio): Freizeit, Kultur und Sport

it11: (fausgkitaso; feindkitaso): Ausgaben Kinderbetreuung

it12: (fausgkindso; feindkindso): kinderbezogene Ausgaben für Drogerieartikel, Kleidung, Spielzeug

it13: (fausgasso; feindgasso): Ausgaben für personelle Assistenzen (z. B. Pflegeassistenz, Mitschreibkraft, Haushaltshilfe)

it14: (fausgthilfo; feindgthilfo): Ausgaben für technische Hilfsmittel (z. B. Screen Reader, Braille-Zeile, FM-Anlage)

it15: (fausandqo; feinandqo2): Weitere Ausgaben, und zwar:

Trennlinie

it16: (fausinsg): Gesamtausgaben:


st:

ao1: Präfix [infield = Betrag; fausgmieto; feindmieto] Suffix: [number] € pro Monat

ao2: Präfix [infield = Betrag; fausgerno; feinderno] Suffix: [number] € pro Monat

ao3: Präfix [infield = Betrag; fausgkomo; feindkomo] Suffix: [number] € pro Monat 

ao4: Präfix [infield = Betrag; fausgkleio; feindkleio] Suffix: [number] € pro Monat

ao5: Präfix [infield = Betrag; fausglerno; feindlerno] Suffix: [number] € pro Monat

ao6: Präfix [infield = Betrag; fausgmobo; feindgmobo] Suffix: [number] € pro Monat

ao7: Präfix [infield = Betrag; fausggeso; feindgeso] Suffix: [number] € pro Monat

ao8: Präfix [infield = Betrag; fausgsemo; feindgsemo] Suffix: [number] € pro Monat

ao9: Präfix [infield = Betrag; faugstuo; feindgstuo] Suffix: [number] € pro Monat

ao10: Präfix [infield = Betrag; fausgfreio; feindgfreio] Suffix: [number] € pro Monat

ao11: Präfix [infield = Betrag; fausgkitaso; feindkitaso] Suffix: [number] € pro Monat

ao12: Präfix [infield = Betrag; fausgkindso; feindkindso] Suffix: [number] € pro Monat

ao13: Präfix [infield = Betrag; fausgasso; feindgasso] Suffix: [number] € pro Monat

ao14: Präfix [infield = Betrag; fausgthilfo; feindgthilfo] Suffix: [number] € pro Monat

ao15: Präfix [infield = Betrag; fausandq; fausandqo; feinandq2; feinandqo2] Suffix: [number] (50 Zeichen)

ao16: Präfix [infield = Betrag; fausinsg] Suffix: [number] € pro Monat

mv:

ka:

vc1: SHOW it11 IF [dkinja = 2]

vc2: SHOW it12 IF [dkinja = 2]

vc3: SHOW it13 IF [gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1] 

vc4: SHOW it14 IF [ggartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1] 

vc5: SHOW is2 IF wohnal=!1

av1: number : 1 bis 4 stellig (1-9999)

av2: number : 50 Zeichen (hier nur für 2 Variablen x müssen noch eingetragen
werden, siehe unter ao14)

kh: Bitte geben Sie Ihre jeweiligen monatlichen Ausgaben an (1 bis 9999)

fv:

hv:

fo:

tr: GOTO D3_9

hi: “Ich bezahle selbst” und “Dritte (Eltern, Partner\*in etc.) bezahlen direkt”
als Spaltenüberschriften; Bei "fausinsg" (Gesamtausgaben) bitte Trennlinie und 2 offene Angabefelder (selbst vs. Dritte) 

\--------------------------------

D3_9
=====

tc:

vn: fmineink; fmineinko

qt: offene Angabe

hl:

in:

q: Wieviel Geld benötigen Sie mindestens pro Monat, um finanziell zurecht zu kommen?

is:

it:

st:

ao1: (fmineink) Eingabefeld; Präfix: [infield =  €; [number], (fmineinko)]  

mv:

ka:

vc:

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 9999).

fv:

hv:

fo:

tr: GOTO D3_10  IF feindgsemo > 0 OR feindgstuo > 0;  
    GOTO D3_11  IF feindgsemo = 0 AND feindgstuo = 0
    GOTO D3_11  IF feindgsemo = MISSING AND feindgstuo = MISSING

hi:

\--------------------------------

D3_10
=====

tc: IF (feindgsemo > 0 | feindgstuo > 0)

vn: fausgstkelt; fausgstkelto; fausgstkpart; fausgstkparto; fausgstkarb; fausgstkarbo; fausgstkand; fausgstkando

qt: offene Angabe

hl:

in: 

q: Sie haben angegeben, dass Dritte Ihre Studienkosten (Semesterbeitrag bzw. Studiengebühren) übernehmen oder sich daran beteiligen.
[Leerzeile]
Davon bezahlen durchschnittlich im Monat …

is:

it1: ... meine Eltern für mich direkt:

it2: ... mein*/e Partner*/in für mich direkt:

it3: ... mein Arbeitgeber für mich direkt:

it4: ... andere für mich direkt und zwar:

st:

ao1: Präfix [infield = €; [number] fausgstkelt; fausgstkelto] 

ao2: Präfix [infield = €; [number] fausgstkpart; fausgstkparto]  

ao3: Präfix [infield = €; [number] fausgstkarb; fausgstkarbo]

ao4: Präfix [infield = €; [number] fausgstkand; fausgstkando] 

mv: 

ka: 

vc: 

av: number : 1-4 stellig : 1 TO 9999

kh: 

fv: 

hv: 

fo: 

tr: GOTO D3_11

hi: 

\--------------------------------

D3_11
=====

tc:

vn: fsitzum1; fsitzum2; fsitzum3; fsitelt1; fsitelt2; fsitelt3

qt: Einfachauswahlmatrix

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

vn: feinstf1; feinstf2; feinstf3; feinstf4; feinstf5; feinstf6; feinstf7;
feinstf8

qt: Einfachauswahlmatrix (keine Mehrfachauswahl???)

hl:

in:

q: Inwieweit treffen die folgenden Aussagen zum Umgang mit Geld auf Sie zu?

is:

it1: (feinstf1): Ich gebe Geld lieber sofort aus als es für einen späteren
Zeitpunkt zu sparen.

it2: (feinstf2): Ich kümmere mich sorgfältig um meine finanziellen
Angelegenheiten.

it3: (feinstf3): Es gelingt mir, mit meinem Geld auszukommen.

it4: (feinstf4): Es belastet mich, mir Gedanken über meine finanzielle Zukunft
zu machen.

it5: (feinstf5): Bevor ich etwas kaufe, vergleiche ich immer die Preise

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

GOTO D3_6 IF fbafja = 3 OR fbafja = MISSING

hi:


\--------------------------------

D3_14
=====

tc: IF fbafja = 1 (kein Bafög-Antrag gestellt)

vn: fbafex

qt: Einfachauswahl

hl:

in:

q: Haben Sie während Ihres Studiums früher einmal einen Antrag auf BAföG
gestellt?

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

tc:IF fbafja = 2 (Bafög-Antrag abgelehnt)

vn: fbafabg

qt: Einfachauswahl

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

tc: IF fbafja = 1 \| 2 (im SS 2020 kein Bafög)

vn: fbafkelt; fbafkein; fbafkfhd; fbafktw; fbafkleis; fbafkalt; fbafkzwei;
fbafkweni; fabfkschu; fbafand; fbafando

qt: Mehrfachnennung und offene Angabe (ao11)

hl:

in:

q: Aus welchen Gründen [Individualisierung]:

IF fbafja = 1 AND fbafex = 1 \| kA: haben Sie bisher keinen BAföG-Antrag
gestellt?

IF fbafja = 2: wurde Ihr aktueller Antrag abgelehnt?

IF (fbafja = 1) AND (fbafex = 2 \| 3): wurde Ihr Antrag damals abgelehnt?

IF fbafja = 1 AND fbafex = 4: haben Sie keinen Antrag auf Weiterförderung mehr
gestellt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (fbafkelt): Das Einkommen der Eltern bzw. des Ehepartners/der Ehepartnerin
ist/war zu hoch.

ao2: (fbafkein): Das eigene Einkommen/Vermögen ist/war zu hoch.

ao3: (fbafkfhd): Die Förderungshöchstdauer wurde überschritten.

ao4: (fbafktw): Das Studienfach wurde gewechselt.

ao5: (fbafkleis): Die notwendige Leistungsbescheinigung konnte nicht erbracht werden.

ao6: (fbafkalt): Bei Studienbeginn war die maßgebliche Altersgrenze bereits
überschritten.

ao7: (fbafkzwei): Das jetzige Studium ist eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium).

ao8: (fbafkweni): Der zu erwartende Förderbeitrag ist/war so gering, dass es
sich nicht lohnt/e.

ao9: (fbafkschu): Ich will/wollte keine Schulden machen.

ao10: (fbafand): Andere Gründe, und zwar: (fbafando) 50 Zeichen 

mv:

ka:

vc:

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

tc: IF fbafja = 4 (Form der Bafög-Förderung I)

vn: fbafunab

qt: Einfachauswahl

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

tc: IF fbafja = 4 (Form der Bafög-Förderung II)

vn: fbafkv; fbafkin

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

tc: IF eaktsens = 2 | 3 | 4 (Studierende mit mind. einer Erwerbstätigkeit)

vn: etat (etat1 / etat2 / etat3)

qt: offene Angaben (Tableau – Drop Down)

hl:

in: 

q1: Bitte geben Sie die Art Ihrer Erwerbstätigkeit an, der Sie im aktuellen Semester nachgehen.

q2: Bitte geben Sie die Art Ihrer Erwerbstätigkeit an, der Sie im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb  nachgehen.

q3: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten nachzugehen. 
Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

q4: Sie haben angegeben, im aktuellen Semester neben Ihrer Tätigkeit im Ausbildungsbetrieb mehreren Erwerbstätigkeiten nachzugehen. Bitte geben Sie die jeweilige Art Ihrer Erwerbstätigkeiten an.

is: 
it1: (etat1): (Tätigkeit A)  [infield = Art der Tätigkeit; Dropdown-Menü] 
it2: (etat2): (Tätigkeit B)  [infield = Art der Tätigkeit; Dropdown-Menü] 
it3: (etat3): (Tätigkeit C)  [infield = Art der Tätigkeit; Dropdown-Menü] 

st:
ao1: 1: : Tätigkeit als studentische/wissenschaftliche Hilfskraft im Bereich Forschung und Lehre
ao2: 2: : Tätigkeit als studentische/wissenschaftliche Hilfskraft im Bereich Verwaltung
ao3: 3: : Jobben (z. B. in einer Fabrik, einem Büro, einer Kneipe, Babysitten, Nachhilfeunterricht)
ao4: 4: : Tätigkeit, die einen Hochschulabschluss voraussetzt (ohne Hilfskraft)
ao5: 5: : Tätigkeit, die einen beruflichen Ausbildungsabschluss voraussetzt
ao6: 6: : Tätigkeit als Praktikant*in 

mv: 
ka1 (it1): Tätigkeit A

ka2 (it2): Tätigkeit B

ka3 (it3): Tätigkeit C 

vc: 
SHOW q1 IF eaktsens = 2 AND sformdua != 1
SHOW q2 IF eaktsens = 2 AND sformdua = 1
SHOW q3 IF eaktsens = 3 | 4 AND sformdua != 1
SHOW q4 IF eaktsens = 3 | 4 AND sformdua = 1

SHOW it1 IF eaktsens = 2 | 3 | 4
SHOW it2 IF eaktsens = 3 | 4 
SHOW it3 IF eaktsens = 4 

SHOW ka1 TO ka2 IF eaktsens = 3 
SHOW ka1 TO ka3 IF eaktsens = 4   

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

tc: sformberu = 1 | sformdua = 1 Frage wird berufsbegleitend oder dual Studierenden gestellt

vn1: jobbbds1, jobbbdso1, jobbbds2, jobbbdso2, 

qt: offene Abfrage im Spaltenformat / Einfachauswahl im Spaltenformat

hl:

in:

q: Welchen Beruf üben Sie aktuell aus? Bitte erläutern Sie die Tätigkeit kurz.

is: Falls Sie zurzeit nicht erwerbstätig sind, geben Sie bitte die Ihre zuletzt
ausgeübte Tätigkeit an.

Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive
Führungsaufgaben ein. Zum Beispiel:

-   Bankkaufmann/-frau (nicht: Angestellte/r) Beratung, Verkauf von
    Finanzprodukten, Abteilungsleitung

-   Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in) Zollfahndung,
    Einsatzplanung

-   Maschinenbauingenieur(in) (nicht: Ingenieur/in) Konstruktion,
    Optimierungsprozesse, Produktionsleitung

it:

st:

ao1: (jobbbds1) Textfeld, 50 Zeichen; Präfix: [infield = Berufsbezeichnung; (jobbbdso1)]

ao2: (jobbbds2) Textfeld, 50 Zeichen; Präfix: [infield = Tätigkeitsbeschreibung (jobbbdso2)]

ao3: -11: : nie berufstätig gewesen

ao4: -12: : weiß ich nicht [EK]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D3_21

hi:

\--------------------------------

D3_21
=====

tc: IF eaktsens = 2 \|3 \|4

vn: egr (egrfin1 / egrfin2 / egrfin3 / egrkar1 / egrkar2 / egrper1 / egrper2 /
egrper3 / egrerf1 / egrerf2 / egralt1 / egralt2)

qt: Caroussel

hl:

in:

q1: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters einer Erwerbstätigkeit nach, …

q2: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters neben meiner Tätigkeit im
Ausbildungsbetrieb einer Erwerbstätigkeit nach, …

q3: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters mehreren Erwerbstätigkeiten nach, …

q4: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters neben meiner Tätigkeit
im Ausbildungsbetrieb mehreren Erwerbstätigkeiten nach, …

is:

it1: (egrfin1): ... weil es zur Finanzierung meines Lebensunterhalts unbedingt
notwendig ist.

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

SHOW q1 IF eaktsens = 2

SHOW q2 IF eaktsens = 2 AND sformdua == 1

SHOW q3 IF eaktsens =  3 \| 4

SHOW q4 IF eaktsens = 3 \| 4 AND sformdua == 1

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

vn: zufrwohn /zufrlstand / zufrfinsit / zufrerw / zufrleb

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q: Wie zufrieden sind Sie aktuell mit…

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

SHOW it4 IF eaktsens = 2 \|3 \|4

av:

kh:

fv:

hv:

fo:

tr:  GOTO D1_9 IF mastersplit=3, 4, 9, 10, 14
     GOTO D2_6 IF mastersplit=5, 6, 11, 12

hi:
