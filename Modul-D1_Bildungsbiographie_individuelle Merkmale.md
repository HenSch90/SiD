D1_1
=

tc1:

vn: vtrae / vtraeo

qt: Einfachauswahl / offene Angabe

hl:

in:

q: An welcher Schule haben Sie Ihre Studienberechtigung erworben?

is:

it:

st:

ao1: 1: : staatliche Schule

ao2: 2: : private Schule

ao3: 3: : kirchliche Schule

ao4: 4: : Andere Schule, und zwar: [(vtraeo)]

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

vn: prffach (prffach1 / prffach2 / prffach3 / prffach4 / prffach5)
    notefach (notefach1 / notefach2 / notefach3 / notefach4 / notefach5)

qt: Akkordeon / offene Angabe / Dropdown-Menü

hl:

in:

q: Bitte nennen Sie uns Ihre schulischen Prüfungsfächer inklusive der jeweiligen Abschlussnote.

is: Beziehen Sie Ihre Angaben bitte auf Ihr Abschlussjahr.

it:

st:

ao1: (prffach1), [infield = 1. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao2: (prffach2), [infield = 2. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao3: (prffach3), [infield = 3. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao4: (prffach4), [infield = 4. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao5: (prffach5), [infield = 5. Prüfungsfach; 60 Zeichen] (offene Angabe)


ao11: (notefach1), [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao12: (notefach2), [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao13: (notefach3), [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao14: (notefach4), [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao15: (notefach5), [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)


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

hi: Bitte Eingabefelder / Drop-downs linksbündig untereinander und die Zeilen ohne graue Schraffierung.

\--------------------------------

D1_3 
==

tc:

vn: inkl (inklnein / inklja / inklschu)

qt: Mehrfachauswahl vertikal

hl:

in:

q: Unabhängig davon, ob bei Ihnen selbst ein Förderbedarf bestand oder nicht: Wurden Sie jemals in einer Inklusionsklasse oder einer Förderschule unterrichtet?

is: Mit „Inklusionsklasse“ ist der gemeinsame Unterricht von Schüler\*innen mit und ohne sonderpädagogischen Förderbedarf gemeint.
#{layout.BREAK}
Bitte alles Zutreffende auswählen.

it: 

st:

ao1: (inklnein): nein, weder noch [Exklusivkategorie]

ao2: (inklja): Ja, ich wurde in einer integrativ arbeitenden (Inklusions-)Klasse unterrichtet.

ao3: (inklschu): Ja, ich war auf einer Förderschule.

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

tc: IF (vsbstyp= 10 | 11) | (vausbja=3)

vn: erlberuf; vausbzpjo; vausbzpmo; vausbzpnot; vausbzpnok

qt: offene Angabe und Einfachauswahl mit Dropdown

hl:

in:

q1: Welchen Beruf haben Sie (zuletzt) erlernt?

q2: Wann haben Sie die Berufsausbildung abgeschlossen?

q3: Mit welcher Note haben Sie Ihre Berufsausbildung abgeschlossen?

is1:

is2:

is3: Für den Fall, dass Sie keine Noten erhalten haben, sondern Ihre Leistungen mit Punkten, Prozentangaben o. Ä. bewertet wurden, rechnen Sie diese bitte in Noten um.

it:

st:

ao1 (erlberuf), [infield = erlernter Beruf; 80 Zeichen] (offene Angabe)

ao2a: (vausbzpjo), [infield = Jahr; 2020 - 2019 - 2018 - ... - 1950] (Dropdown)

ao2b: (vausbzpmo), [infield = Monat; Januar - Februar - März - ... - Dezember] (Dropdown)

ao3a: (vausbzpnot),[infield = Abschlussnote (z. B. 2,5); 3 Zeichen] (NUMBER, offene Angabe mit Dezimalstelle)

ao3b: (vausbzpnok): Ich habe keine Note erhalten. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_5

hi:

\--------------------------------

D1_5 
==

tc: IF (vsbstyp= 10 | 11) | (vausbja=3)

vn: vausberufo

qt: offene Angabe

hl:

in:

q: Welchen Beruf haben Sie (zuletzt) erlernt?

is:

it:

st:

ao1: (vausberufo), Präfix: [Infield = gelernter Beruf; 75 Zeichen]

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

tc: IF (vsbstyp= 10 | 11) | (vausbja=3)

vn: vausbnote / vausbnoteo

qt: offene Angabe / Einfachauswahl

hl:

in:

q: Mit welcher Note haben Sie Ihre (letzte) Berufsausbildung abgeschlossen?

is:

it:

st:

ao1: (vausbnoteo), Präfix: [infield = Abschlussnote (z. B. 2,5); number]

ao2: (vausbnote): Ich habe keine Note erhalten.

mv:

ka:

vc:

av: (vausbnoteo): 1,0 TO 4,0

kh: (vausbnoteo): Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr:

GOTO A_42

hi:

\--------------------------------

D1_7 
==

tc: IF (ssemhs <= 7 | isMissing(ssemhs)) 

vn: stfw (stfwint / stfwent / stfwein / stfwber / stfwsoz / stfwart / stfwalt / stfwwiss / stfwfam / stfwzeit / stfwzul / stfwhelf / stfwver / stfwand / stfwando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen Studienfaches?

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

it11: (stfwzul): niedrige Hürden bei der Zulassung (z. B. keine Zulassungsbeschränkung)

it12: (stfwhelf): Möglichkeit anderen Menschen helfen zu können

it13: (stfwver): Vereinbarkeit meiner Beeinträchtigung mit späteren Beschäftigungsmöglichkeiten

it14: (stfwand): Anderes, und zwar: [(stfwando)]

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc: SHOW it13 (stfwver) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh: 

fv:

hv:

fo:

tr:

GOTO D1_8

hi: Items bitte zufällig rotieren mit Ausnahme von it14 "Anderes und zwar"; it14 bitte am Ende der Itemliste verankern.

\--------------------------------

D1_8 
==

tc: IF (ssemhs <= 7 | isMissing(ssemhs)) 

vn: hsw (hswzul / hswtrad / hswkont / hswatt / hswreg / hswbed / hswruf / hswfach / hswrank / hswint / hsweng / hswsupp / hswbarr / hswtz / hswand / hswando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen Hochschule?

is:

it1: (hswzul): keine Zulassung an Wunschhochschule

it2: (hswtrad): Tradition und Ruf der Hochschule

it3: (hswkont): persönlicher Kontakt zu Freund\*innen und/oder Familie vor Ort

it4: (hswatt): Attraktivität von Stadt und Umgebung

it5: (hswreg): regionale Nähe zum Heimatort

it6: (hswbed): günstige Lebensbedingungen am Hochschulort (Wohnen, Lebenshaltung)

it7: (hswruf): guter Ruf der Lehrenden in meinem Fachgebiet

it8: (hswfach): gewünschte Fachrichtung

it9: (hswrank): gute Platzierung meines Fachs in Rankings

it10: (hswint): internationale Ausrichtung des Studienangebotes

it11: (hsweng): Wunschstudiengang wird auf Englisch angeboten

it12: (hswsupp): hochschulspezifische Unterstützungsangebote (Beratung, psychologische Betreuung, Vorsorge, “Brückenkurse”)

it13: (hswbarr): gute Ausstattung/Barrierefreiheit

it14: (hswtz): Möglichkeit, in Teilzeit studieren zu können

it15: (hswand): Anderes, und zwar: [(hswando)]

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

kh: 

fv:

hv:

fo:

tr:

GOTO D2_6 IF mastersplit=1, 2, 7, 8, 14
GOTO A_44 IF mastersplit=3, 4, 9, 10


hi: Items bitte zufällig rotieren mit Ausnahme von it15 "Anderes und zwar"; it15 bitte am Ende der Itemliste verankern.

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


\--------------------------------

D1_10a 
===

tc: IF sabsja=2 AND (mastersplit = 1, 2, 3, 4, 7, 8, 9, 10, 14)

vn: sabserbl1

qt: Einfachauswahl vertikal

hl:

in:

q: Haben Sie Ihren letzten Hochschulabschluss an Ihrer derzeitigen Hochschule erworben?

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

tr:

GOTO D1_10 IF sabserbl1 = 0
GOTO D1_12 IF sabserbl1 = 1
GOTO D1_12 IF ssemhs = k. A.


\--------------------------------



D1_10 
===

tc: IF sabserbl1 = 0 

vn: sabserbl

qt: Drop-Down-Menü

hl:

in:

q: In welchem Bundesland liegt die Hochschule, an der Sie Ihren letzten Hochschulabschluss erworben haben?

is:

it1: (sabserbl): [infield = Bundesland] (Drop-Down)

st:

aox: 0: Bundesland

ao1: 2: Baden-Württemberg

ao2: 3: Bayern

ao3: 4: Berlin

ao4: 5: Brandenburg

ao5: 6: Bremen

ao6: 7: Hamburg

ao7: 8: Hessen

ao8: 9: Mecklenburg-Vorpommern

ao9: 10: Niedersachsen

ao10: 11: Nordrhein-Westfalen

ao11: 12: Rheinland-Pfalz

ao12: 13: Saarland

ao13: 14: Sachsen

ao14: 15: Sachsen-Anhalt

ao15: 16: Schleswig-Holstein

ao16: 17: Thüringen

ao17: 18: im Ausland

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_11 IF (sabserbl = 2 – 17)
GOTO D1_11a IF (sabserbl = 18)
GOTO D1_12 IF (sabserbl = k. A. | 0)

\--------------------------------

D1_11 
====

tc: IF sabserbl = 2 – 17 

vn: sabserhs1 / sabserhs2

qt: Dropdown-Menü / offene Nennung

hl:

in:

q1: An welcher Hochschule haben Sie Ihren Abschluss erworben?

q2: Sollte die Hochschule nicht aufgeführt sein, tragen Sie diese bitte in das dafür vorgesehene Feld ein.

is:

it:

st:

ao1: (sabserhs1), [infield = Hochschule] (Drop-Down)

ao2: (sabserhs2), Präfix: [infield = Hochschule; 100 Zeichen] (offene Nennung)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_12

hi1: q1 und ao1 bitte oberhalb von q2 und ao2 platzieren.
hi2: Das Drop-Down wird mit einer von uns zu lieferenden Hochschulliste (vorgefiltert nach Bundesland) gefüllt.


\--------------------------------


D1_11a 
====

tc: IF sabserbl = 17

vn: sabserhs3 / sabserhs4

qt: offene Nennung

hl:

in:

q: An welcher ausländischen Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao1: (sabserhs3), Präfix: [infield = Land; 60 Zeichen] 

ao2: (sabserhs4), Präfix: [infield = Hochschule; 60 Zeichen] 

mv:

ka:

vc:

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

tc: IF sabsja=2 

vn: sabserfacho

qt: offene Nennung

hl:

in:

q: In welchem Fach haben Sie diesen Abschluss erworben?

is:

it:

st:

ao1: (sabserfacho), Präfix: [infield =  Studienfach; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_49a IF sabser=1
    GOTO A_49b IF (sabser!=1) OR (sabser = k. A.)
    
hi:

\--------------------------------

D1_13 
===

tc:

vn: absterm

qt: Drop-Down-Menü

hl:

in:

q: Wann werden Sie Ihr derzeitiges Studium voraussichtlich abschließen?

is:

it: (absterm): [infield = Semester] (Drop-Down)

st:

aox: 0: : Semester

ao1: 1: : Sommersemester 2020

ao2: 2: : Wintersemester 2020/21

ao3: 3: : Sommersemester 2021
.
.
.
ao21: 21: : Sommersemester 2030

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

tc: 

vn: ssweijaaz / sawejaaz / shwjaaz / ssujaaz

qt: Drop-Down-Menü

hl:

in:

q: Wie häufig haben Sie seit Ihrer Erstimmatrikulation …

is: Nicht gemeint sind Wechsel oder Unterbrechungen beim Übergang vom Bachelor- ins Masterstudium.

it1: (ssweijaaz): … das Studienfach gewechselt?

it2: (sawejaaz): … den angestrebten Abschluss gewechselt?

it3: (shwjaaz): … die Hochschule gewechselt?

it4: (ssujaaz): … das Studium zwischenzeitlich unterbrochen?

st:

aox: 0: Anzahl

ao1: 1: einmal

ao2: 2: zweimal

ao3: 3: dreimal

ao4: 4: viermal

ao5: 5: fünfmal und mehr

(ao1 bis ao5 als Drop-Down; infield = Anzahl)

mv:

ka:

vc1: SHOW ssweijaaz IF ssweja=1

vc2: SHOW sawejaaz IF saweja=1

vc3: SHOW shwjaaz IF shwja=1

vc4: SHOW ssujaaz IF ssuja=1

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_15
    
    
hi:

\--------------------------------

D1_15 
===

tc: IF ssweijaaz>=1 und/oder saweijaaz>=1 und/oder shwijaaz>=1 


vn: beginn01 – beginn05 / ende01 – ende05 / hs01 – hs05 / fach01 – fach05 / abs01 – abs05 / stand01 – stand05 / techepi

qt: Akkordeon/ Tableau / Dropdown-Menü / offene Angaben / Einfachauswahl

hl:

in:

q1: Bitte tragen Sie die wesentlichen Stationen Ihres Studienverlaufs in das nachfolgende Tableau ein.

q2: Benötigen Sie weitere Episoden?

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit Studienbeginn. Sollten die vorgegebenen 5 Episoden nicht ausreichen, so können Sie weitere Episoden aktivieren.

it1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): Präfix: Beginn: [infield = Semester] (Drop-Down)

it2: (ende01 / ende02 / ende03 / ende04 / ende05): Präfix: Ende: [infield = Semester] (Drop-Down)

it3: (hs01 / hs02 / hs03 / hs04 / hs05): Präfix: [infield = Hochschule; 100 Zeichen] (offene Angabe)

it4: (fach01 / fach02 / fach03 / fach04 / fach05): Präfix: [infield = Studienfach; 60 Zeichen] (offene Angabe)

it5: (abs01 / abs02 / abs03 / abs04 / abs05): [infield = angestrebter Abschluss] (Drop-Down)

it6: (stand01 / stand02 / stand03 / stand04 / stand05): [infield = letzter Stand] (Drop-Down)

it7: (techepi)

st:

ao1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): 1: : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao2: (ende01 / ende02 / ende03 / ende04 / ende05): 1 : : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao3: (hs01 / hs02 / hs03 / hs04 / hs05): Präfix: [infield = Hochschule; 100 Zeichen] 

ao4: (fach01 / fach02 / fach03 / fach04 / fach05): Präfix: [infield = Studienfach; 60 Zeichen] 

ao5: (abs01 / abs02 / abs03 / abs04 / abs05): 1: : Bachelor \ 2: :Bachelor (Lehramt) \ 3: : Master \ 4: :Master (Lehramt) \ 5: : Staatsexamen \ 6: : Staatsexamen (Lehramt) \ 7: : Diplom, Promotion \ 8: : künstlerische Abschlussprüfung \ 9: : anderer Abschluss (bspw. Ausländischer Abschluss, Magister) \ 10: : kein Studienabschluss

ao6: (stand01 / stand02 / stand03 / stand04 / stand05): 1: : begonnen \ 2: : abgeschlossen \ 3: : abgebrochen \ 4: : unterbrochen

ao7: (techepi): 1: : nein

ao8: (techepi): 2: : ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_15b IF techepi==2
    GOTO D1_16 IF ssuja=1  
    GOTO A_51a IF h_split=1 
    GOTO A_51b IF h_split=2 
    
hi1: Bitte 5 Akkordeons mit den Überschriften Episode 1, Episode 2, Episode 3, Episode 4, Episode 5 anlegen. 
hi2: Bitte die Drop-Downs und Eingabefelder pro Episode linksbündig untereinander anordnen.


\--------------------------------

D1_15b 
===

tc: IF ssweijaaz>=1 und/oder saweijaaz>=1 und/oder shwijaaz>=1 & techepi = 1


vn: beginn06 – beginn10 / ende06 – ende10 / hs06 – hs10 / fach06 – fach10 / abs06 – abs10 / stand06 – stand10 

qt: Akkordeon/ Tableau / Dropdown-Menü / offene Angaben 

hl:

in:

q1: Bitte tragen Sie die wesentlichen Stationen Ihres Studienverlaufs in das nachfolgende Tableau ein.

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit Studienbeginn. 

it1: (beginn06 / beginn07 / beginn08 / beginn09 / beginn10): Präfix: Beginn: [infield = Semester] (Drop-Down)

it2: (ende06 / ende07 / ende08 / ende09 / ende10): Präfix: Ende: [infield = Semester] (Drop-Down)

it3: (hs06 / hs07 / hs08 / hs09 / hs10): Präfix: [infield = Hochschule; 100 Zeichen] (offene Angabe)

it4: (fach06 / fach07 / fach08 / fach09 / fach10): Präfix: [infield = Studienfach; 60 Zeichen] (offene Angabe)

it5: (abs06 / abs07 / abs08 / abs09 / abs10): [infield = angestrebter Abschluss] (Drop-Down)

it6: (stand06 / stand07 / stand08 / stand09 / stand10): [infield = letzter Stand] (Drop-Down)

st:

ao1: (beginn06 / beginn07 / beginn08 / beginn09 / beginn10): 1: : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao2: (ende06 / ende07 / ende08 / ende09 / ende10): 1 : : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao3: (hs06 / hs07 / hs08 / hs09 / hs10): Präfix: [infield = Hochschule; 100 Zeichen] 

ao4: (fach06 / fach07 / fach08 / fach09 / fach10): Präfix: [infield = Studienfach; 60 Zeichen] 

ao5: (abs06 / abs07 / abs08 / abs09 / abs10): 1: : Bachelor \ 2: :Bachelor (Lehramt) \ 3: : Master \ 4: : Master (Lehramt) \ 5: : Staatsexamen \ 6: : Staatsexamen (Lehramt) \ 7: : Diplom, Promotion \ 8: : künstlerische Abschlussprüfung \ 9: : anderer Abschluss (bspw. Ausländischer Abschluss, Magister) \ 10: : kein Studienabschluss

ao6: (stand06 / stand07 / stand08 / stand09 / stand10): 1: : begonnen \ 2: : abgeschlossen \ 3: : abgebrochen \ 4: : unterbrochen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO D1_16 IF ssuja=1  
    GOTO A_51a IF h_split=1 
    GOTO A_51b IF h_split=2 
    
hi1: Bitte 5 Akkordeons mit den Überschriften Episode 6, Episode 7, Episode 8, Episode 9, Episode 10 anlegen. 
hi2: Bitte die Drop-Downs und Eingabefelder pro Episode linksbündig untereinander anordnen.


\--------------------------------

D1_16 
===

tc: IF ssujaaz>=1 

vn: suzeitp01 / suzeitp02 / suzeit03 / sudau01 / sudau02 / sudau03 / subeur01 / subeur02 / subeur03

qt: Akkordeon / Tableau / Drop-Down-Menü / offene Angabe / Einfachauswahl

hl:

in:

q1: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q2: Bitte beschreiben Sie Ihre Studienunterbrechungen näher.

q3: Bitte beschreiben Sie Ihre letzten drei Studienunterbrechungen nächer.

is1: Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.

is2: Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.
Sollten Sie mehr als dreimal unterbrochen haben, beginnen Sie bitte mit Ihrer
drittletzten Unterbrechung.

it1: (suzeitp01 / suzeitp02 / suzeitp03): Präfix: Zeitpunkt der Unterbrechung: [infield = Semester] (Drop-Down)

it2: (sudau01 / sudau02 / sudau03): Präfix: Dauer der Unterbrechung: [infield = Monate; number] (Eingabefeld)

it3: (subeur01 / subeur02 / subeur03): mit Beurlaubung

st:

ao1: (suzeitp01 / suzeitp02 / suzeitp03): : 1: : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao2: (sudau01 / sudau02 / sudau03): number 2 Stellen; 0 TO 99

ao3: (subeur01 / subeur02 / subeur03) 1: : mit Beurlaubung

mv:

ka:

vc1: SHOW q1 AND suzeitp01 & sudau01 & subeur01 IF ssujaaz=1 \

vc2: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 IF ssujaaz=2

vc3: SHOW q3/is2 AND suzeitp01 & sudau01 & subeur01 & suzeitp01 & sudau01 &
subeur01 & suzeitp02 &sudau02 & subeur02 & suzeitp03 & sudau03 & subeur03
IF ssujaaz= 3 | 4 | 5

av:

kh: (sudau01 / sudau02 / sudau03): Bitte geben Sie die Dauer Ihrer Studienunterbrechung in Monaten an (0 bis 99).

fv:

hv:

fo:

tr: GOTO A_51a IF h_split=1 
    GOTO A_51b IF h_split=2 
    
hi1: Bitte 3 Akkordeons mit den Überschriften 1. Studienunterbrechung, 2. Studienunterbrechung, 3. Studienunterbrechung      anlegen. 
hi2: Bitte die Drop-Downs und Eingabefelder pro Episode linksbündig untereinander anordnen.

\--------------------------------

D1_17 
===

tc:

vn: sint (sintaner / sintzur / sintfair / sinternst / sintkont / sintfach / sintsem)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1: (sintaner): Ich fühle mich von den Lehrenden anerkannt.

it2: (sintzur): Mit den Lehrenden meines Studiengangs komme ich gut zurecht.

it3: (sintfair): Die meisten Lehrenden behandeln mich fair.

it4: (sinternst): Die Lehrenden interessieren sich für das, was ich zu sagen habe.

it5: (sintkont): Mir ist es während meines bisherigen Studiums gut gelungen, Kontakte zu anderen Studierenden aufzubauen.

it6: (sintfach): Ich kenne viele Kommiliton\*innen, mit denen ich mich über fachspezifische Fragen austauschen kann.

it7: (sintsem): Ich habe viele Kontakte zu Studierenden aus meinem Semester.

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

D1_19 
===

tc:

vn: sask (sask1 / sask2 / sask3 / sask4 / sask5)

qt: 5er-Skala mit horizontalen ao

hl:

in:

q: Bitte beantworten Sie die folgenden Fragen ohne lange nachzudenken.

is:

it1: (sask1): Ich halte meine Begabung für das Studium für ...

it2: (sask2): Im Studium Neues zu lernen fällt mir ...

it3: (sask3): Meiner Meinung nach bin ich ...

it4: (sask4): Meine studienbezogenen Fähigkeiten sind ...

it5: (sask5): Aufgaben im Rahmen des Studiums fallen mir ...

st:

ao1 (sask1) 1 : :  ... niedrig

ao2 (sask1) 2

ao3 (sask1) 3

ao4 (sask1) 4

ao5 (sask1) 5: :  ... hoch

ao6 (sask2) 1 : :  ... schwer

ao7 (sask2) 2

ao8 (sask2) 3

ao9 (sask2) 4

ao10 (sask2) 5: :  ... leicht

ao11 (sask3) 1 : :  ... nicht intelligent

ao12 (sask3) 2

ao13 (sask3) 3

ao14 (sask3) 4

ao15 (sask3) 5: :  ... sehr intelligent

ao16 (sask4) 1 : :  ... niedrig

ao17 (sask4) 2

ao18 (sask4) 3

ao19 (sask4) 4

ao20 (sask4) 5: :  ... hoch

ao21 (sask5) 1 : :  ... schwer

ao22 (sask5) 2

ao23 (sask5) 3

ao24 (sask5) 4

ao25 (sask5) 5: :  ... leicht

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

vn: kom  (kominter / kommeth / komwiss / komtext / komkrit / komsch / kommuen / komteam / komvera / komkomm / komplan)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte schätzen Sie ein, inwieweit Sie aktuell über die folgenden Fähigkeiten und Kenntnisse verfügen.

is:

it1: (kominter): fachübergreifendes Wissen und Denken/Interdisziplinarität

it2: (kommeth): Anwendung fachbezogener Methoden

it3: (komwiss): Erarbeitung einer wissenschaftlichen Fragestellung

it4: (komtext): Verstehen von wissenschaftlichen Texten

it5: (komkrit): kritisches Denken (eigene Ideen/Ideen anderer in Frage stellen)

it6: (komsch): schriftlicher Ausdruck

it7: (kommuen): mündlicher Ausdruck

it8: (komteam): Teamfähigkeit/Zusammenarbeit in einer Gruppe

it9: (komvera): Übernahme von Verantwortung in einer Gruppe

it10: (komkomm): Kommunikation mit Professor\*innen

it11: (komplan): Planungs- und Organisationsfähigkeit

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

vn: kspr (ksprdeu / kspreng / ksprfra / ksprspa / ksprand / ksprando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie gut beherrschen Sie die folgenden Sprachen?

is:

it1: (ksprdeu): Deutsch

it2: (kspreng): Englisch

it3: (ksprfra): Französisch

it4: (ksprspa): Spanisch

it5: (ksprand / ksprando): Andere Sprache, und zwar: [50 Zeichen]

st:

ao1: 1: : Grundkenntnisse

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr gute Kenntnisse

ao6: 6: : Ich beherrsche diese Sprache nicht

ao7: 7: : Muttersprache

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_22 IF h_split=1 
GOTO D1_23 IF h_split=2 

hi: 

\--------------------------------

D1_22 
===

tc:

vn: dpzufr / dpinter / dpfrag / dsmein / dswiss / dsfreiz / sfaufw / sfober / sfklaus / ssverl / sswied / sszeit

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1: (dpzufr): Studieren gibt mir manchmal das Gefühl von tiefer persönlicher Zufriedenheit.

it2: (dpinter): Ich habe das Gefühl, dass praktisch jedes Thema hochinteressant sein kann, wenn ich mich erst einmal damit befasse.

it3: (dpfrag): In die meisten meiner Lehrveranstaltungen gehe ich mit Fragen, auf die ich nach einer Antwort suche.

it4: (dsmein): Ich bin erst zufrieden, wenn ich mich intensiv genug in ein Thema eingearbeitet habe, um mir eine eigene Meinung bilden zu können.

it5: (dswiss): Ich überprüfe mein Wissen zu wichtigen Themen, bis ich es wirklich verstanden habe.

it6: (dsfreiz): Ich nutze meine Freizeit häufig dafür, mehr über interessante Themen zu erfahren, die wir in Lehrveranstaltungen diskutiert haben.

it7: (sfaufw): Mein Ziel ist es, Lehrveranstaltungen mit so wenig Aufwand wie möglich zu bestehen.

it8: (sfober): Ich finde es nicht hilfreich, Themen zu vertiefen. Es verwirrt nur und ist verschwendete Zeit, wenn man nur oberflächliches Wissen benötigt.

it9: (sfklaus): Ich sehe keinen Grund darin Stoff zu lernen, der wahrscheinlich nicht klausurrelevant ist.

it10: (ssverl): Ich lerne nur das ernsthaft, was in meinem Studium verlangt wird.

it11: (sswied): Manche Dinge wiederhole ich so lange, bis ich sie auswendig kann, selbst wenn ich sie nicht verstehe.

it12: (sszeit): Lehrende sollten nicht erwarten, dass Studierende viel Zeit damit verbringen Stoff zu lernen, von dem jeder weiß, dass er nicht geprüft wird.

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

vn: kogorga / kogkrit1 / kogkrit2 / kogzus / kogwied / mkogplan1 / mkogplan2 / mkogwach1 / mkogwach2 / mkogreg / ressanst1 / ressanst2 / resskonz1 / resskonz2 / resszeit / lernumg1 / lernumg2 / resskomm / lit

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1: (kogorga): Ich stelle mir aus Mitschrift, Skript oder Literatur kurze Zusammenfassungen mit den wichtigsten Punkten zusammen.

it2: (kogkrit1): Beim Lernen hinterfrage ich die meisten Schlussfolgerungen kritisch.

it3: (kogkrit2): Ich denke über Alternativen zu den Behauptungen oder Schlussfolgerungen in den Lerntexten nach.

it4: (kogzus): Zu neuen Lerninhalten stelle ich mir praktische Anwendungen vor.

it5: (kogwied): Ich lerne den Lernstoff anhand von Skripten oder anderen Aufzeichnungen möglichst auswendig.

it6: (mkogplan1): Ich überlege mir vorher, in welcher Reihenfolge ich den Stoff durcharbeite.

it7: (mkogplan2): Ich versuche, mir vorher genau zu überlegen, welche Teile eines bestimmten Themengebiets ich lernen muss und welche nicht.

it8: (mkogwach1): Ich bearbeite zusätzliche Aufgaben, um festzustellen, ob ich den Stoff wirklich verstanden habe.

it9: (mkogwach2): Um Wissenslücken festzustellen, rekapituliere ich die wichtigsten Inhalte, ohne meine Unterlagen zu Hilfe zu nehmen,

it10: (mkogreg): Wenn ich Lerninhalte nicht direkt verstehe, gehe ich den Text noch einmal langsam durch.

it11: (ressanst1): Ich arbeite so lange, bis ich mir sicher bin, die Prüfung gut bestehen zu können.

it12: (ressanst2): Ich lerne auch spätabends und am Wochenende, wenn es sein muss.

it13: (resskonz1): Ich ertappe mich dabei, dass ich mit meinen Gedanken ganz woanders bin.

it14: (resskonz2): Beim Lernen fällt es mir schwer, bei der Sache zu bleiben.

it15: (resszeit): Beim Lernen stelle ich einen Zeitplan auf, an den ich mich auch halte.

it16: (lernumg1): Mein Arbeitsplatz ist so gestaltet, dass ich alles schnell finden kann.

it17: (lernumg2): Wenn ich lerne, sorge ich dafür, dass ich in Ruhe arbeiten kann.

it18: (resskomm): Ich lerne zusammen mit meinen Studienkolleg\*innen.

it19: (lit): Ich suche nach weiterführender Literatur, wenn mir bestimmte Inhalte noch nicht ganz klar sind.

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

vn: pbig (pbigintro / pbigextro / pbigtrau / pbigkrit / pbiggenau / pbigfaul / pbigruh / pbignerv / pbigkrea / pbignoku)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1: (pbigintro): Ich bin eher zurückhaltend, reserviert.

it2: (pbigextro): Ich gehe aus mir raus, bin gesellig.

it3: (pbigtrau): Ich schenke anderen leicht Vertrauen, glaube an das Gute im Menschen.

it4: (pbigkrit): Ich neige dazu, andere zu kritisieren.

it5: (pbiggenau): Ich erledige Aufgaben gründlich.

it6: (pbigfaul): Ich bin bequem, neige zur Faulheit.

it7: (pbigruh): Ich bin entspannt, lasse mich durch Stress nicht aus der Ruhe bringen.

it8: (pbignerv): Ich werde leicht nervös und unsicher.

it9: (pbigkrea): Ich habe eine aktive Vorstellungskraft, bin phantasievoll.

it10: (pbignoku): Ich habe nur wenig künstlerisches Interesse.

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

vn: pbigintro / pbigextro / pbigtrau

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1: (pbigintro): In schwierigen Situationen kann ich mich auf meine Fähigkeiten verlassen.

it2: (pbigextro): Die meisten Probleme kann ich aus eigener Kraft gut meistern.

it3: (pbigtrau): Auch anstrengende und komplizierte Aufgaben kann ich in der Regel gut lösen.

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

ao1: 1: : gar nicht risikobereit

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr risikobereit

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

vn: feel (feelstress / feellast / feeldruck)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie haben Sie sich in den letzten vier Wochen überwiegend gefühlt?

is:

it1: (feelstress): gestresst

it2: (feellast): überlastet

it3: (feeldruck): unter Druck

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

vn: dep (depschw / depglue / depdep / deptrau / depverz / depgedr / depgut / depsich / depruhe / depspass)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Wie fühlen Sie sich im Allgemeinen?

is:

it1: (depschw): Meine Stimmung ist schwermütig.

it2: (depglue): Ich bin glücklich.

it3: (depdep): Ich bin deprimiert.

it4: (deptrau): Ich bin traurig.

it5: (depverz): Ich bin verzweifelt.

it6: (depgedr): Ich bin in gedrückter Stimmung.

it7: (depgut): Ich fühle mich gut.

it8: (depsich): Ich fühle mich sicher.

it9: (depruhe): Ich bin ruhig und gelassen.

it10: (depspass): Das Leben macht mir Spaß.

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

hi1: Items bitte zufällig rotieren.
hi2: Bitte keine Verbindungslinie der Skalenpunkte da ordinale Items.
