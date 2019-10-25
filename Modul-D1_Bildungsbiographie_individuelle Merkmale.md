D1_1
=

tc1:

vn: vtrae; vtraeo

qt: Einfachauswahl, offene Angabe

hl:

in:

q: An welcher Art von Schule haben Sie Ihre Studienberechtigung erworben?

is:

it:

st:

ao1: 1: : staatliche Schule

ao2: 2: : private Schule

ao3: 3: : kirchliche Schule

ao4: 4: : Andere Schule, und zwar: (offene Angabe: Präfix [vtraeo], 50
Zeichen)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_2

hi:

\--------------------------------

D1_2 
==

tc1:

vn: prffach1; prffach2; prffach3; prffach4; prffach5; stdfach1, stdfach2,
stdfach3, stdfach4, stdfach5; notefach1, notefach2, notefach3, notefach4,
notefach5, gesfach1, gesfach2, gesfach3, gesfach4, gesfach5

qt: offene Angabe / Einfachauswahl mit Dropdown-Menü

hl:

in:

q: Bitte nennen Sie uns Ihre schulischen Prüfungsfächer inklusive der jeweiligen wöchentlichen Stundenzahl, der Abschlussnote und des Geschlechts des/der Lehrer*/in.

is: Beziehen Sie Ihre Angaben bitte auf Ihr Abschlussjahr.

it:

st:

ao1: offene Angabe, Präfix: [infield = 1. Prüfungsfach; prffach1], 50 Zeichen

ao2: offene Angabe, Präfix: [infield = 2. Prüfungsfach; prffach2], 50 Zeichen

ao3: offene Angabe, Präfix: [infield = 3. Prüfungsfach; prffach3], 50 Zeichen

ao4: offene Angabe, Präfix: [infield = 4. Prüfungsfach; prffach4], 50 Zeichen

ao5: offene Angabe, Präfix: [infield = 5. Prüfungsfach; prffach5], 50 Zeichen

ao6: stdfach1: : [infield =  Std. je Woche; 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std.] (Dropdown)

ao7: stdfach2: : [infield =  Std. je Woche; 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std.] (Dropdown)

ao8: stdfach3: : [infield =  Std. je Woche; 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std.] (Dropdown)

ao9: stdfach4: : [infield =  Std. je Woche; 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std.] (Dropdown)

ao10: stdfach5: : [infield =  Std. je Woche; 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std.] (Dropdown)

ao11: notefach1: : [infield = Note; sehr gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend] (Dropdown)

ao12: notefach2: : [infield = Note; sehr gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend] (Dropdown)

ao13: notefach3: : [infield = Note; sehr gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend] (Dropdown)

ao14: notefach4: : [infield = Note; sehr gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend] (Dropdown)

ao15: notefach5: : [infield = Note; sehr gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend] (Dropdown)

ao16: gesfach1: : [infield = Geschlecht; männlich \| weiblich] (Dropdown)

ao17: gesfach2: : [infield = Geschlecht; männlich \| weiblich] (Dropdown)

ao18: gesfach3: : [infield = Geschlecht; männlich \| weiblich] (Dropdown)

ao19: gesfach4: : [infield = Geschlecht; männlich \| weiblich] (Dropdown)

ao20: gesfach5: : [infield = Geschlecht; männlich \| weiblich] (Dropdown)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_3

hi:

\--------------------------------

D1_3 
==

tc:

vn: inklnein; inklja; inklschu

qt: Mehrfachauswahl

hl:

in:

q: Unabhängig davon, ob bei Ihnen selbst ein Förderbedarf bestand oder nicht: Wurden Sie jemals in einer integrativ arbeitenden Klasse/Inklusionsklasse unterrichtet oder haben Sie eine Förderschule besucht?

is: Kennzeichnend für eine integrativ arbeitende Klasse/Inklusionsklasse ist
der gemeinsame Unterricht von Schüler\*innen mit und ohne sonderpädagogischen
Förderbedarf.
Bitte alles Zutreffende auswählen.

it: 

st:

ao1: inklnein: : nein, weder noch [Exklusivkategorie]

ao2: inklja: : Ja, ich wurde in einer integrativ arbeitenden
Klasse/Inklusionsklasse unterrichtet.

ao3: inklschu: : Ja, ich war auf einer Förderschule.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_40

hi:

\--------------------------------

D1_4 
==

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausbzpjo; vausbzpmo

qt: offene Angabe (nebeneinander)

hl:

in:

q: Wann haben Sie Ihre (letzte) Berufsausbildung abgeschlossen (Zeitpunkt der Zeugnisübergabe)?

is:

it:

st:

ao1: (vausbzpjo) Eingabefeld, 4 Stellen; 1950-2020; Präfix: [infield = Jahr; number]

ao2: (vausbzpmo): Textfeld, 15 Zeichen; Präfix: [infield = Monat]

mv:

ka:

vc:

av: number: vierstellig : 1950 TO 2020

kh: (vausbzpjo) Bitte geben Sie das Jahr des Abschlusses Ihrer (letzten) Berufsausbildung an (1950 bis 2020).

fv:

hv:

fo:

tr:

GOTO D1_5

hi:

\--------------------------------

D1_5 
==

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausberuf, vausberufo

qt: offene Angabe

hl:

in:

q: Welchen Beruf haben Sie (zuletzt) erlernt?

is:

it:

st:

ao1: (vausberuf): 75 Zeichen; Präfix: [Infield = gelernter Beruf; (vausberufo)];

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_6

hi:

\--------------------------------

D1_6
=

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausbnote; vausbnoteo

qt: Einfachauswahl / offene Angabe

hl:

in:

q: Mit welcher Note haben Sie Ihre (letzte) Berufsausbildung abgeschlossen?

is:

it:

st:

ao1: (vausbnote): : Eingabefeld; 3 Stellen; Präfix: [infield = Note (z. B. 2,5); (vausbnoteo); number]

ao2: -11: : Ich habe keine Note erhalten.

mv:

ka:

vc:

av: number: dreistellig : 1,0 TO 4,0

kh: Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr:

GOTO A_42

hi:

\--------------------------------

D1_7 
==

tc: IF ssemhs=1 \| 2 \| 01 \| 02 (nur Studierende im 1. + 2. Fachsemester)

vn: stfwint; stfwent; stfwein; stfwber; stfwsoz; stfwarb; stfwalt; stfwwiss;
stfwfam; stfwzeit; stfwzul; stfwhelf; stfwver; stfwand; stfwando

qt: Einfachauswahlmatrix / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen
Studienfaches?

is:

it1: (stfwint): spezielles Fachinteresse

it2: (stfwent): persönliche Entfaltung

it3: (stfwein): Einkommenschancen im späteren Beruf

it4: (stfwber): fester Berufswunsch

it5: (stfwsoz): spätere hohe soziale Position

it6: (stfwart): gute Aussichten auf sicheren Arbeitsplatz

it7: (stfwalt): Ausweichlösung, da keine Zulassung im gewünschten Studienfach

it8: (stfwwiss): Erhalt einer guten wissenschaftlichen Ausbildung

it9: (stfwfam): Eltern/Familie haben mir dazu geraten

it10: (stfwzeit): kurze Studienzeiten

it11: (stfwzul): niedrige Hürden bei der Zulassung (z. B. keine
Zulassungsbeschränkung)

it12: (stfwhelf): Möglichkeit anderen Menschen helfen zu können

it13: (stfwver): Vereinbarkeit meiner Beeinträchtigung mit späteren
Beschäftigungsmöglichkeiten

it14: (stfwand): Anderes, und zwar:

it15: (offene Angabe) 120 Zeichen; Präfix: [stfwando]; Suffix: weiterer Grund:

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc: SHOW stfwver IF gartmob – gartka=1

av:

kh: Bitte geben Sie einen weiteren Grund an.

fv:

hv:

fo:

tr:

GOTO D1_8

hi: Items bitte zufällig rotieren

\--------------------------------

D1_8 
==

tc: IF ssemhs=1 \| 2 \| 01 \| 02 (nur Studierende im 1. + 2. Fachsemester)

vn: hswzul; hswtrad; hswkont; hswatt, hswreg; hswbed; hswruf; hswfach; hswrank;
hswint; hsweng; hswsupp; hswbarr; hswtz, hswand; hswando

qt: Einfachauswahlmatrix / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen
Hochschule?

is:

it1: (hswzul): keine Zulassung an Wunschhochschule

it2: (hswtrad): Tradition und Ruf der Hochschule

it3: (hswkont): persönlicher Kontakt zu Freunden und/oder Familie vor Ort

it4: (hswatt): Attraktivität von Stadt und Umgebung

it5: (hswreg): regionale Nähe zum Heimatort

it6: (hswbed): günstige Lebensbedingungen am Hochschulort (Wohnen,
Lebenshaltung)

it7: (hswruf): guter Ruf der Lehrenden in meinem Fachgebiet

it8: (hswfach): gewünschte Fachrichtung

it9: (hswrank): gute Platzierung meines Fachs in Rankings

it10: (hswint): internationale Ausrichtung des Studienangebotes

it11: (hsweng): Wunschstudiengang wird auf Englisch angeboten

it12: (hswsupp): hochschulspezifische Unterstützungsangebote (Beratung,
psychologische Betreuung, Vorsorge, “Brückenkurse”)

it13: (hswbarr): gute Ausstattung/Barrierefreiheit

it14: (hswtz): Möglichkeit, in Teilzeit studieren zu können

it15: (hswand): Anderes, und zwar:

it16: (offene Angabe) 100 Zeichen; Präfix: [hswando]; Suffix: weiterer Grund:

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc:

av:

kh: Bitte geben Sie einen weiteren Grund an.

fv:

hv:

fo:

tr:

GOTO D2_6 IF mastersplit=1, 2, 7, 8, 14
GOTO A_44 IF mastersplit=3, 4, 9, 10


hi: Items bitte zufällig rotieren

\--------------------------------

D1_9 
==

tc:

vn: sartzeit

qt: Einfachauswahl

hl:

in:

q: Betreiben Sie Ihr Studium in Vollzeit oder Teilzeit?

is:

it:

st:

ao1: 1: : Vollzeit

ao2: 2: : Teilzeit

ao3: 3: : Vollzeitstudiengang mit individueller Teilzeitregelung.

ao4: 4: : Vollzeitstudiengang inoffiziell als Teilzeitstudium

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_7 IF (ssemhs=1 OR ssemhs=2) OR (ssemhs=01 OR ssemhs=02)
    GOTO D1_7 IF ssemhs=MISSING
    GOTO D2_6 IF (ssemhs>2 OR ssemhs>02) AND (mastersplit=1, 2, 7, 8, 14)
    GOTO A_44 IF (ssemhs>2 OR ssemhs>02) AND (mastersplit=3, 4, 9, 10)
       

hi:

\--------------------------------

D1_10 
===

tc: IF sabsja=2 (nur Studierende mit vorherigem Hochschulabschluss)

vn: sabserbl

qt: Drop-Down

hl:

in:

q: In welchem Bundesland liegt die Hochschule, an der Sie Ihren letzten
Hochschulabschluss erworben haben?

is:

it1: (sabserbl): : [infield = Bundesland] (Dropdown)

st:

ao1 (sabserbl): 1: : Baden-Württemberg

ao2 (sabserbl): 2: : Bayern

ao3 (sabserbl): 3: : Berlin

ao4 (sabserbl): 4: : Brandenburg

ao5 (sabserbl): 5: : Bremen

ao6 (sabserbl): 6: : Hamburg

ao7 (sabserbl): 7: : Hessen

ao8 (sabserbl): 8: : Mecklenburg-Vorpommern

ao9 (sabserbl): 9: : Niedersachsen

ao10 (sabserbl): 10: : Nordrhein-Westfalen

ao11 (sabserbl): 11: : Rheinland-Pfalz

ao12 (sabserbl): 12: : Saarland

ao13 (sabserbl): 13: : Sachsen

ao14 (sabserbl): 14: : Sachsen-Anhalt

ao15 (sabserbl): 15: : Schleswig-Holstein

ao16 (sabserbl): 16: : Thüringen

ao17 (sabserbl): 17: : im Ausland

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_11a IF sabserbl = 1 – 16
GOTO D1_11b IF sabserbl = 17


\--------------------------------

D1_11a 
====

tc: IF sabserbl = 1 – 16 

vn: sabserhs

qt: Dropdown-Menü

hl:

in:

q: An welcher Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao (sabserhs): : [infield = Hochschule] (Dropdown)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_13

hi: Bitte mit nachfolgender Frage auf einer Seite programmieren.

\--------------------------------

D1_11b 
====

tc1: IF sabserbl= 1 – 16

tc2: IF sabserbl= 17

vn: sabserhs2

qt: Offene Nennung

hl:

in:

q1: Sollte die Hochschule nicht aufgeführt sein, tragen Sie diese bitte in das
dafür vorgesehene Feld ein.

q2: An welcher Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao1: (offene Nennung): 100 Stellen; Präfix: [infield = Hochschule; sabserhs2]; 
mv:

ka:

vc1: SHOW q1 IF sabserbl= 1 - 16

vc2: SHOW q2 IF sabserbl=17

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_12

hi:

\--------------------------------

D1_12 
===

tc: IF sabsja=1 

vn: sabserfacho

qt: offene Nennung

hl:

in:

q: In welchem Fach haben Sie diesen Abschluss erworben?

is:

it:

st:

ao1: (offene Nennung): 60 Stellen; Präfix: [infield =  Studienfach; sabserfacho]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_49a IF sabser=1
    GOTO A_49b IF sabser>1
    GOTO A_49a IF sabser=MISSING
    
hi:

\--------------------------------

D1_13 
===

tc:

vn: absterm

qt: Dropdown-Menü

hl:

in:

q: Wann werden Sie Ihr derzeitiges Studium voraussichtlich abschließen?

is:

it:

st:

ao1: (absterm): : [infield = Semester; Sommersemester 2020 \| Wintersemester 2020/21 \| Sommersemester
2021 \|Wintersemester 2021/22 \| Sommersemester 2022 \| … \| Sommersemester 2030] (Drop-Down)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_27

hi:

\--------------------------------

D1_14 
===

tc: IF ssweija=1 und/oder saweija=1 und/oder shwija=1 und/oder ssuja=1 (nur
Studierende mit vorherigem Studienfachwechsel, Abschlusswechsel,
Hochschulwechsel und/oder Studienunterbrechung)

vn: ssweijaaz; saweijaaz, sshwjaaz; ssujaaz

qt: Dropdown-Menü

hl:

in:

q: Wie häufig haben Sie seit Ihrer Erstimmatrikulation …

is: Nicht gemeint sind Wechsel oder Unterbrechungen beim Übergang vom Bachelor-
ins Masterstudium.

it1: (ssweijaaz): … das Studienfach gewechselt?

it2: (sawejaaz): ... den angestrebten Abschluss gewechselt?

it3: (shwjaaz): … die Hochschule gewechselt?

it4: (ssujaaz): … das Studium zwischenzeitlich unterbrochen?

st:

ao1: 0: : keinmal

ao2: 1: : einmal

ao3: 2: : zweimal

ao4: 3: : dreimal

ao5: 4: : viermal

ao6: 5: : fünfmal und mehr

(ao1 bis ao5 als Dropdown; infield = Anzahl)

mv:

ka:

vc1: SHOW ssweijaaz IF ssweija=1

vc2: SHOW sawejaaz IF saweija=1

vc3: SHOW shwjaaz IF shwja=1

vc4: SHOW ssujaaz IF ssuja=1

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_15 IF ssweja=1 OR saweja=1 OR shwja=1
    GOTO D1_16 IF ssweja=0 AND saweja=0 AND shwja=0 AND ssuja=1
    
    
hi:

\--------------------------------

D1_15 
===

tc:

vn: beginn01 – beginn05; ende01 – ende05; hs01 – hs05; fach01 – fach05; abs01 –
abs05; stand01 – stand05; techepi

qt: Dropdown-Menü / offene Angaben

hl:

in:

q: Bitte tragen Sie die wesentlichen Stationen Ihres Studienverlaufs in das
nachfolgende Tableau ein.

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit
Studienbeginn. Sollten die vorgegebenen 5 Episoden nicht ausreichen, so können
Sie weitere Episoden aktivieren.

it1 (beginn01 – beginn05, ende01 – ende05): Beginn und Ende (Semester)

it2 (hs01 – hs05): Hochschule

it3 (fach01 – fach05): Studienfach

it4 (abs01 – abs05): angestrebter Abschluss

it5 (stand01 – stand05): letzter Stand

it6: techepi): Benötigen Sie weitere Episoden?

st:

ao1: (Dropdown bitte absteigend - beginn01 – beginn05): Sommersemester 2020 \|
Wintersemester 2019/2020 \| Sommersemester 2019 \| Wintersemester 2018/2019 \| …
\| Wintersemester 2020

ao2: -12: : weiß ich noch nicht

ao3: (offene Angabe): 100 Stellen; Präfix: [hs01 – hs05]; Suffix: Hochschule

ao4: (offene Angabe) 60 Stellen; Präfix: [fach01 – fach05]; Suffix: Studienfach

ao5: (Dropdown abs01 – abs05): Bachelor \| Bachelor (Lehramt) \| Master \|
Master (Lehramt) \| Staatsexamen \| Staatsexamen (Lehramt) \| Diplom, Promotion
\| kirchliche Abschlussprüfung \| künstlerische Abschlussprüfung \| anderer
Abschluss (bspw. Ausländischer Abschluss \| Magister) \| kein Studienabschluss

ao6: (Dropdown stand01 – stand05): begonnen \| abgeschlossen \| abgebrochen \|
unterbrochen

ao7: (techepi): 0: : nein

ao8: (techepi): 1: : ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_16 IF ssuja=1
    GOTO A_51a IF ssuja=0 AND h_split=1 (50%)
    GOTO A_51b IF ssuja=0 AND h_split=2 (50%)
    GOTO A_51a IF ssuja=MISSING AND h_split=1 (50%)
    GOTO A_51b IF ssuja=MISSING AND h_split=2 (50%)  
    
hi: Wenn techepi=1, bitte zwei weitere Zeilen einblenden.

Das Tableau passt nicht in die gängige Template-Vorlage!

\--------------------------------

D1_16 
===

tc: IF ssuja=1 (nur Studierende, die mindestens eine Studienunterbrechung
hatten)

vn: suzeitp01; suzeitp02; suzeit03; sudau01; sudau02; sudau03; subeur01;
subeur02; subeur03

qt: Tableau-Abfrage (Dropdown-Menü, offene Angabe, Einfachauswahl)

hl:

in:

Individualisierung:

q1: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q2: Bitte beschreiben Sie Ihre Studienunterbrechungen näher.

q3: Bitte beschreiben Sie Ihre letzten drei Studienunterbrechungen nächer.

is1 (nur für q2): Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.

is2 (nur für q3): Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.
Sollten Sie mehr als dreimal unterbrochen haben, beginnen Sie bitte mit Ihrer
drittletzten Unterbrechung.

it1: (suzeitp01 – sozeitp03): Zeitpunkt der Unterbrechung:

it2: (sudau01 – sudau03): Dauer der Unterbrechung

it3: (subeur01 – subeur03): mit Beurlaubung?

st:

ao1: (Dropdown suzeitp01 – suzeitp03): : Sommersemester 2020 \| Wintersemester
2019/2020 \| Sommersemester 2019 \| … \| Wintersemester 2004/2005

ao2: (offene Angabe): 2 Stellen (00-99); Präfix: [sudau01 – sudau03]; Suffix:
Monate

ao3: (subeur01 – subeur03) 1: : nein

ao4: (subeur01 – subeur03) 2: : ja

mv:

ka:

vc1: SHOW q1 AND suzeitp01 \| sudau01 \| subeur01 IF ssujaaz=1 \| kA

vc2: SHOW q2 AND suzeitp01 \| sudau01 \| subeur01 \| suzeitß02 \| sudau02 \|
subeur02 IF ssujaaz=2

vc3: SHOW q3 AND suzeitp01 \| sudau01 \| subeur01 \| suzeitp01 \| sudau01 \|
subeur01 \| suzeitp02 \| sudau02 \| subeur02 \| suzeitp03 \| sudau03 \| subeur03
IF ssujaaz= 3 \| 4 \| 5

av:

kh:

fv:

hv:

fo:

tr: GOTO A_51a IF h_split=1 (50%)
    GOTO A_51b IF h_split=2 (50%)
    
hi: In Abhängigkeit der Antworten auf Seite D1_14 erfolgt eine Einblendung von
bis zu drei Unterbrechungen, für die je Zeile anhand verschiedener
Antwortformate Informationen erhoben werden.

\--------------------------------

D1_17 
===

tc:

vn: sintaner; sintzur; sintfair; sinternst; sintkont; sintfach; sintsem

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (sintaner): Ich fühle mich von den Lehrenden anerkannt.

it2 (sintzur): Mit den Lehrenden meines Studiengangs komme ich gut zurecht.

it3 (sintfair): Die meisten Lehrenden behandeln mich fair.

it4 (sinternst): Die Lehrenden interessieren sich für das, was ich zu sagen
habe.

it5 (sintkont): Mir ist es während meines bisherigen Studiums gut gelungen,
Kontakte zu anderen Studierenden aufzubauen.

it6 (sintfach): Ich kenne viele Kommiliton\*innen, mit denen ich mich über
fachspezifische Fragen austauschen kann.

it7 (sintsem): Ich habe viele Kontakte zu Studierenden aus meinem Semester.

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

GOTO D1_18

hi: Items bitte zufällig rotieren.

\--------------------------------

D1_18 
===

tc:

vn: pakagern; pakafrem; pakaort; pakalost

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pakagern): Alles in allem bin ich gerne Student(in).

it2 (pakafrem): Die studentische Welt ist mir fremd.

it3 (pakaort): Die Hochschule ist genau der richtige Platz für mich.

it4 (pakalost): An der Hochschule fühle ich mich verloren.

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

GOTO D1_19

hi: Items bitte zufällig rotieren.

\--------------------------------

D1_19 
===

tc:

vn: sask1; sask2; sask3; sask4; sask5

qt: 5er Skala mit Bezeichnung der Endpunkte

hl:

in:

q: Bitte beantworten Sie die folgenden Fragen ohne lange nachzudenken.

is:

it1 (sask1): Ich halte meine Begabung für das Studium für

it2 (sask2): Im Studium Neues zu lernen fällt mir

it3 (sask3): Meiner Meinung nach bin ich

it4 (sask4): Meine studienbezogenen Fähigkeiten sind

it5 (sask5): Aufgaben im Rahmen des Studiums fallen mir

st:

ao1 (sask1) 1 : : niedrig

ao2 (sask1) 2

ao3 (sask1) 3

ao4 (sask1) 4

ao5 (sask1) 5: : hoch

ao6 (sask2) 1 : : schwer

ao7 (sask2) 2

ao8 (sask2) 3

ao9 (sask2) 4

ao10 (sask2) 5: : leicht

ao11 (sask3) 1 : : nicht intelligent

ao12 (sask3) 2

ao13 (sask3) 3

ao14 (sask3) 4

ao15 (sask3) 5: : sehr intelligent

ao16 (sask4) 1 : : niedrig

ao17 (sask4) 2

ao18 (sask4) 3

ao19 (sask4) 4

ao20 (sask4) 5: : hoch

ao21 (sask5) 1 : : schwer

ao22 (sask5) 2

ao23 (sask5) 3

ao24 (sask5) 4

ao25 (sask5) 5: : leicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D2_13 if mastersplit=1, 2, 7, 8, 14
    GOTO A_23 if mastersplit=3, 4, 9, 10

hi:

\--------------------------------

D1_20 
===

tc:

vn: kominter; kommeth; komwiss; komtext; komkrit; komsch; kommuen; komteam;
komvera; komkomm; komplan

qt: Einfachauswahlmatrix

hl:

in:

q: Bitte schätzen Sie ein, inwieweit Sie aktuell über die folgenden Fähigkeiten
und Kenntnisse verfügen.

is:

it1 (kominter): fachübergreifendes Wissen und Denken/Interdisziplinarität

it2 (kommeth): Anwendung fachbezogener Methoden

it3 (komwiss): Erarbeitung einer wissenschaftlichen Fragestellung

it4 (komtext): Verstehen von wissenschaftlichen Texten

it5 (komkrit): kritisches Denken (eigene Ideen/Ideen anderer in Frage stellen)

it6 (komsch): schriftlicher Ausdruck

it7 (kommuen): mündlicher Ausdruck

it8 (komteam): Teamfähigkeit/Zusammenarbeit in einer Gruppe

it9 (komvera): Übernahme von Verantwortung in einer Gruppe

it10 (komkomm): Kommunikation mit Professor\*innen

it11 (komplan): Planungs- und Organisationsfähigkeit

st:

ao1: 1: : gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : in hohem Maße

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_21

hi: Items bitte zufällig rotieren.

\--------------------------------

D1_21 
===

tc:

vn: ksprdeu; kspreng; ksprfra; ksprspa; ksprand; ksprando

qt: Einfachauswahlmatrix

hl:

in:

q: Wie gut beherrschen Sie die folgenden Sprachen?

is:

it1 (ksprdeu): Deutsch

it2 (kspreng): Englisch

it3 (ksprfra): Französisch

it4 (krprspa): Spanisch

it5 (ksprand): Andere Sprache, und zwar:

it6 (offene Angabe): 50 Stellen; Präfix: [ksprando]; Suffix: Andere Sprache:

st:

ao1: 1: : Grundkenntnisse

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr gute Kenntnisse

ao6: 6: : Muttersprache

ao7: 7: : Ich beherrsche diese Sprache nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_22 IF h_split=1 (50%)
GOTO D1_23 IF h_split=2 (50%)

hi:

\--------------------------------

D1_22 
===

tc:

vn: dpzufr; dpinter; dpfrag; dsmein; dswiss; dsfreiz; staufw; sfober; sfklaus;
ssverl; sswied; sszeit

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (dpzufr): Studieren gibt mir manchmal das Gefühl von tiefer persönlicher
Zufriedenheit.

it2 (dpinter): Ich habe das Gefühl, dass praktisch jedes Thema hochinteressant
sein kann, wenn ich mich erst einmal damit befasse.

it3 (dpfrag): In die meisten meiner Lehrveranstaltungen gehe ich mit Fragen, auf
die ich nach einer Antwort suche.

it4 (dsmein): Ich bin erst zufrieden, wenn ich mich intensiv genug in ein Thema
eingearbeitet habe, um mir eine eigene Meinung bilden zu können.

it5 (dswiss): Ich überprüfe mein Wissen zu wichtigen Themen, bis ich es wirklich
verstanden habe.

it6 (dsfreiz): Ich nutze meine Freizeit häufig dafür, mehr über interessante
Themen zu erfahren, die wir in Lehrveranstaltungen diskutiert haben.

it7 (sfaufw): Mein Ziel ist es, Lehrveranstaltungen mit so wenig Aufwand wie
möglich zu bestehen.

it8 (sfober): Ich finde es nicht hilfreich, Themen zu vertiefen. Es verwirrt nur
und ist verschwendete Zeit, wenn man nur oberflächliches Wissen benötigt.

it9 (sfklaus): Ich sehe keinen Grund darin Stoff zu lernen, der wahrscheinlich
nicht klausurrelevant ist.

it10 (ssverl): Ich lerne nur das ernsthaft, was in meinem Studium verlangt wird.

it11 (sswied): Manche Dinge wiederhole ich so lange, bis ich sie auswendig kann,
selbst wenn ich sie nicht verstehe.

it12 (sszeit): Lehrende sollten nicht erwarten, dass Studierende viel Zeit damit
verbringen Stoff zu lernen, von dem jeder weiß, dass er nicht geprüft wird.

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

GOTO D1_24

hi: Items bitte zufällig rotieren.

\--------------------------------

D1_23 
===

tc:

vn: kogorga; kogkrit1; kogkrit2; kogzus; kogwied; mkogplan1; mkogplan2;
mkogwach1; mkogwach2; mkogreg; ressanst1; ressanst2; sesskonz1; resskonz2;
resszeit; lernumg1; lernumg2; resskomm; lit

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (kogorga): Ich stelle mir aus Mitschrift, Skript oder Literatur kurze
Zusammenfassungen mit den wichtigsten Punkten zusammen.

it2 (kogkrit1): Beim Lernen hinterfrage ich die meisten Schlussfolgerungen
kritisch.

it3 (kogkrit2): Ich denke über Alternativen zu den Behauptungen oder
Schlussfolgerungen in den Lerntexten nach.

it4 (kogzus): Zu neuen Lerninhalten stelle ich mir praktische Anwendungen vor.

it5 (kogwied): Ich lerne den Lernstoff anhand von Skripten oder anderen
Aufzeichnungen möglichst auswendig.

it6 (mkogplan1): Ich überlege mir vorher, in welcher Reihenfolge ich den Stoff
durcharbeite.

it7 (mkogplan2): Ich versuche, mir vorher genau zu überlegen, welche Teile eines
bestimmten Themengebiets ich lernen muss und welche nicht.

it8 (mkogwach1): Ich bearbeite zusätzliche Aufgaben, um festzustellen, ob ich
den Stoff wirklich verstanden habe.

it9 (mkogwach2): Um Wissenslücken festzustellen, rekapituliere ich die
wichtigsten Inhalte, ohne meine Unterlagen zu Hilfe zu nehmen,

it10 (mkogreg): Wenn ich Lerninhalte nicht direkt verstehe, gehe ich den Text
noch einmal langsam durch.

it11 (ressanst1): Ich arbeite so lange, bis ich mir sicher bin, die Prüfung gut
bestehen zu können.

it12 (ressanst2): Ich lerne auch spätabends und am Wochenende, wenn es sein
muss.

it13 (resskonz1): Ich ertappe mich dabei, dass ich mit meinen Gedanken ganz
woanders bin.

it14 (resskonz2): Beim Lernen fällt es mir schwer, bei der Sache zu bleiben.

it15 (resszeit): Beim Lernen stelle ich einen Zeitplan auf, an den ich mich auch
halte.

it16 (lernumg1): Mein Arbeitsplatz ist so gestaltet, dass ich alles schnell
finden kann.

it17 (lernumg2): Wenn ich lerne, sorge ich dafür, dass ich in Ruhe arbeiten
kann.

it18 (resskomm): Ich lerne zusammen mit meinen Studienkolleg\*innen.

it19 (lit): Ich suche nach weiterführender Literatur, wenn mir bestimmte Inhalte
noch nicht ganz klar sind.

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

GOTO D1_24

hi: Die Items bitte zufällig rotieren.

\--------------------------------

D1_24 
===

tc:

vn: pbigintro; pbigextro; pbigtrau; pbigkrit; pbiggenau; pbigfaul; pbigruh;
pbignerv; pbigkrea; pbignoku

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pbigintro): Ich bin eher zurückhaltend, reserviert.

it2 (pbigextro): Ich gehe aus mir raus, bin gesellig.

it3 (pbigtrau): Ich schenke anderen leicht Vertrauen, glaube an das Gute im
Menschen.

it4 (pbigkrit): Ich neige dazu, andere zu kritisieren.

it5 (pbiggenau): Ich erledige Aufgaben gründlich.

it6 (pbigfaul): Ich bin bequem, neige zur Faulheit.

it7 (pbigruh): Ich bin entspannt, lasse mich durch Stress nicht aus der Ruhe
bringen.

it8 (pbignerv): Ich werde leicht nervös und unsicher.

it9 (pbigkrea): Ich habe eine aktive Vorstellungskraft, bin phantasievoll.

it10 (pbignoku): Ich habe nur wenig künstlerisches Interesse.

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

GOTO D1_25

hi: Items bitte zufällig rotieren

\--------------------------------

D1_25 
===

tc:

vn: pswskill; pswkraft; pswaufg

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pswskill): In schwierigen Situationen kann ich mich auf meine Fähigkeiten
verlassen.

it2 (pswkraft): Die meisten Probleme kann ich aus eigener Kraft gut meistern.

it3 (pswaufg): Auch anstrengende und komplizierte Aufgaben kann ich in der Regel
gut lösen.

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

GOTO D1_26

hi: Items bitte zufällig rotieren

\--------------------------------

D1_26 
===

tc:

vn: risk

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie risikobereit sind Sie im Allgemeinen?

is:

it:

st:

ao1 (risk) 1: : gar nicht risikobereit

ao2 (risk) 2

ao3 (risk) 3

ao4 (risk) 4

ao5 (risk) 5: : sehr risikobereit

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_27

hi:

\--------------------------------

D1_27 
===

tc:

vn: feelstress; feellast; feeldruck

qt: Einfachauswahlmatrix

hl:

in:

q: Wie haben Sie sich in den letzten vier Wochen überwiegend gefühlt?

is:

it1 (feelstress): gestresst

it2 (feellast): überlastet

it3 (feeldruck): unter Druck

st:

ao1: 1: : gar nicht

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

GOTO D1_28

hi: Items bitte zufällig rotieren.

\--------------------------------

D1_28 
===

tc: IF NOT partpsy=1

vn: depschw; depglue; depdep; deptrau; depverz; depgedr; depgut; depsich;
depruhe; depspass

qt: Einfachauswahlmatrix

hl:

in:

q: Wie fühlen Sie sich im Allgemeinen?

is:

it1 (depschw): Meine Stimmung ist schwermütig.

it2 (depglue): Ich bin glücklich.

it3 (depdep): Ich bin deprimiert.

it4 (deptrau): Ich bin traurig.

it5 (depverz): Ich bin verzweifelt.

it6 (depgedr): Ich bin in gedrückter Stimmung.

it7 (depgut): Ich fühle mich gut.

it8 (depsich): Ich fühle mich sicher.

it9 (depruhe): Ich bin ruhig und gelassen.

it10 (depspass): Das Leben macht mir Spaß.

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

GOTO A_52

hi: Items bitte zufällig rotieren.
