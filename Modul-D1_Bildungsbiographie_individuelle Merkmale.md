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

vn: vausberufo; vausbzpjo; vausbzpmo; vausbnoteo; vausbnote

qt: offene Angaben, Einfachauswahl mit Dropdown und Exklusivkategorie

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

ao1 (vausberufo), [infield = erlernter Beruf; 80 Zeichen] (offene Angabe)

ao2a: (vausbzpjo), [infield = Jahr; 2020 - 2019 - 2018 - ... - 1950] (Dropdown)

ao2b: (vausbzpmo), [infield = Monat; Januar - Februar - März - ... - Dezember] (Dropdown)

ao3a: (vausbnoteo),[infield = Abschlussnote (z. B. 2,5); 3 Zeichen] (offene Angabe, NUMBER mit Dezimalstelle)

ao3b: (vausbnote): Ich habe keine Note erhalten. [Exklusivkategorie]

mv:

ka:

vc:

av3a: (vausbnoteo): 1,0 TO 4,0

kh3a: (vausbnoteo): Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo:

tr:

GOTO D1_7

hi: Auf dieser Seite werden untereinander drei Fragen mit den zugehörigen Antwortoptionen usw. dargestellt (q1 mit ao1, q2 mit ao2a und ao2b sowie q3 mit is3, ao3a, kh3a und ao3b). ao2a und ao2b bitte nebeneinander darstellen, ao3a und ao3b können gerne linksbündig untereinander darsgestellt werden. Wichtig: ao3a bitte als NUMBER mit einer Dezimalstelle programmieren!


\--------------------------------

D1_7 
==

tc: IF (ssemhs <= 4 | isMissing(ssemhs)) 

vn: stfw (stfwein / stfwart / stfwzul / stfwalt / stfwzeit / stfwfam / stfwber / stfwent / stfwbega / stfwint / stfwwiss / stfwverf / stfwverb / stfwand / stfwando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen Studienfaches?  

is:

it1: (stfwein): Einkommens- und Karrierechancen

it2: (stfwart): gute Aussichten auf sicheren Arbeitsplatz

it3: (stfwzul): keine Zulassungsbeschränkungen

it4: (stfwalt): Ausweichlösung, da keine Zulassung im gewünschten Studienfach

it5: (stfwzeit): kurze Studienzeiten

it6: (stfwfam): Eltern/Familie haben mir dazu geraten

it7: (stfwber): fester Berufswunsch

it8: (stfwent): persönliche Entfaltung

it9: (stfwbega): eigene Begabung

it10: (stfwint): spezielles Fachinteresse

it11: (stfwwiss): eine gute wissenschaftliche Ausbildung

it12: (stfwverf): Vereinbarkeit von Familie mit späteren Beschäftigungsmöglichkeiten

it13: (stfwverb): Vereinbarkeit meiner Beeinträchtigung mit späteren Beschäftigungsmöglichkeiten

it14: (stfwand): Anderes, und zwar: [(stfwando)]

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc: SHOW it13 (stfwverb) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh: 

fv:

hv:

fo:

tr:

GOTO D1_8

hi:

\--------------------------------

D1_8 
==

tc: IF (ssemhs <= 4 | isMissing(ssemhs)) 

vn: hsw (hswkont / hswbed / hswatt / hswfach / hswrank / hswruf / hswtrad / hswzul / hswint / hsweng / hswtz / hswsupp / hswdig / hswuntb / hswbarr / hswand / hswando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen Hochschule?

is:

it1: (hswkont): Freund\*innen/Familie vor Ort

it2: (hswbed): günstige Lebensbedingungen am Hochschulort

it3: (hswatt): Attraktivität von Stadt und Umgebung

it4: (hswfach): gewünschte Fachrichtung

it5: (hswrank): gute Platzierung meines Fachs in Rankings

it6: (hswruf): guter Ruf der Lehrenden in meinem Fachgebiet

it7: (hswtrad): Tradition und Ruf der Hochschule

it8: (hswzul): keine Zulassung an Wunschhochschule

it9: (hswint): internationale Ausrichtung der Hochschule

it10: (hsweng): Wunschstudiengang wird auf Englisch angeboten

it11: (hswtz): Möglichkeit, in Teilzeit studieren zu können

it12: (hswsupp): hochschulspezifische Beratungs- und Unterstützungsangebote

it13: (hswdig): Online-Angebot (Studium und Lehre)

it14: (hswuntb): beeinträchtigungsspezifische Unterstützungsangebote der Hochschule

it15: (hswbarr): Barrierefreiheit der Hochschule

it16: (hswand): Anderes, und zwar: [(hswando)]

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc1: SHOW it14 (hswuntb) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

vc2: SHOW it15 (hswbarr) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh: 

fv:

hv:

fo:

tr:

GOTO D2_6 IF mastersplit=1, 2, 7, 8, 14
GOTO A_44 IF mastersplit=3, 4, 9, 10


hi:


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

q2: Sollte Ihre Hochschule nicht aufgeführt sein, tragen Sie diese bitte hier ein (z. B. HU Berlin, FH Bielefeld):

is:

it:

st:

ao1: (sabserhs1), [infield = Hochschule] (Drop-Down)

ao2: (sabserhs2), [infield = Hochschule; 100 Zeichen] (offene Nennung)

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

ao1: (sabserhs3), [infield = Land; 100 Zeichen] 

ao2: (sabserhs4), [infield = Hochschule; 100 Zeichen] 

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

vn: sabserfacho1; sabserfacho2

qt: offene Nennung

hl:

in:

q: In welchem Fach haben Sie diesen Abschluss erworben?

is:

it:

st:

ao1: (sabserfacho1), [infield =  1. Studienfach; 80 Zeichen]

ao2: (sabserfacho2), [infield =  2. Studienfach; 80 Zeichen]

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

it: 

st:

ao: (absterm): [infield = Semester; Sommersemester 2020 - Wintersemester 2020/21 - Sommersemester 2021 - ... - Sommersemester 2030] (Drop-Down) 

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

D1_15 
===

tc: IF ssweijaaz>=1 und/oder saweijaaz>=1 und/oder shwijaaz>=1 


vn: beginn01 – beginn05 / ende01 – ende05 / hs01 – hs05 / fach01 – fach05 / abs01 – abs05 / stand01 – stand05 

qt: Akkordeon/ Tableau / Dropdown-Menü / offene Angaben / Einfachauswahl

hl:

in:

q: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit Studienbeginn.

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit Studienbeginn.

it1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): [infield = Beginn] (Drop-Down)

it2: (ende01 / ende02 / ende03 / ende04 / ende05): [infield = Ende] (Drop-Down)

it3: (hs01 / hs02 / hs03 / hs04 / hs05): [infield = Hochschule; 100 Zeichen] (offene Angabe)

it4: (fach01 / fach02 / fach03 / fach04 / fach05): [infield = Studienfach; 80 Zeichen] (offene Angabe)

it5: (abs01 / abs02 / abs03 / abs04 / abs05): [infield = angestrebter Abschluss] (Drop-Down)

it6: (stand01 / stand02 / stand03 / stand04 / stand05): letzter Stand [Einfachauswahl]

st:

ao1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): 1: : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao2: (ende01 / ende02 / ende03 / ende04 / ende05): 1 : : Sommersemester 2020 \ 2 : : Wintersemester 2019/2020 \ 3 : : Sommersemester 2019 \ 4 : : Wintersemester 2018/2019 \ ... 21 : : Sommersemester 2010

ao3: (hs01 / hs02 / hs03 / hs04 / hs05): Präfix: [infield = Hochschule; 100 Zeichen] 

ao4: (fach01 / fach02 / fach03 / fach04 / fach05): Präfix: [infield = Studienfach; 60 Zeichen] 

ao5: (abs01 / abs02 / abs03 / abs04 / abs05): 1: : Bachelor \ 2: :Bachelor (Lehramt) \ 3: : Master \ 4: :Master (Lehramt) \ 5: : Staatsexamen \ 6: : Staatsexamen (Lehramt) \ 7: : Diplom, Promotion \ 8: : künstlerische Abschlussprüfung \ 9: : anderer Abschluss (bspw. Ausländischer Abschluss, Magister) \ 10: : kein Studienabschluss

ao6: 1: begonnen \ 2: abgeschlossen \ 3: abgebrochen \ 4: unterbrochen

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
    
hi1: Bitte 5 Akkordeons mit den Überschriften 1. Studienepisode, 2. Studienepisode, 3. Studienepisode, 4. Studienepisode, 5. Studienepisode linksbündig untereinander anlegen. 
hi2: Bitte die Drop-Downs und Eingabefelder pro Episode linksbündig nebeneinander anordnen.


\--------------------------------

D1_16 
===

tc: IF ssujaaz>=1 

vn: suzeitp01 / suzeitp02 / suzeit03 / suzeitp04 / suzeit05 / sudau01 / sudau02 / sudau03 / sudau04 / sudau05 / subeur01 / subeur02 / subeur03 / subeur04 / subeur05

qt: Akkordeon / Tableau / Drop-Down-Menü / Einfachauswahl

hl:

in:

q1: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q2: Bitte beschreiben Sie Ihre Studienunterbrechungen näher.

q3: Bitte beschreiben Sie Ihre letzten fünf Studienunterbrechungen näher.

is1: Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.

is2: Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.
Sollten Sie mehr als fünfmal unterbrochen haben, beginnen Sie bitte mit Ihrer fünftletzten Unterbrechung.

it1: (suzeitp01 / suzeitp02 / suzeitp03 / suzeitp04 / suzeitp05): Präfix: Zeitpunkt: [infield = Semester] (Drop-Down)

it2: (sudau01 / sudau02 / sudau03 / sudau04 / sudau05): Präfix: Dauer: [infield = Monate] (Drop-Down)

it3: (subeur01 / subeur02 / subeur03 / subeur03 / subeur04): Beurlaubung [Einfachauswahl]

st:

ao1: (suzeitp01 / suzeitp02 / suzeitp03 / suzeitp04 / suzeitp05): 1: Sommersemester 2020 \ 2 : Wintersemester 2019/2020 \ 3 : Sommersemester 2019 \ 4 : Wintersemester 2018/2019 \ ... 21 : Sommersemester 2010

ao2: (sudau01 / sudau02 / sudau03 / sudau04 / sudau05): 1: 1 Monat \ 2: 2 Monate \ 3: 3 Monate \ 4: 4 Monate \ 24: 24 Monate

ao3: (subeur01 / subeur02 / subeur03 / subeur04 / subeur05) 1: ja; 2: nein

mv:

ka:

vc1: SHOW q1 AND suzeitp01 & sudau01 & subeur01 IF ssujaaz=1 \

vc2: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 IF ssujaaz=2

vc3: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 & suzeitp03 & sudau03 & subeur03 IF ssujaaz=3

vc4: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 & suzeitp03 & sudau03 & subeur03 & suzeitp04 & sudau04 & subeur04 IF ssujaaz=4

vc5: SHOW q3/is2 AND suzeitp01 & sudau01 & subeur01 & suzeitp01 & sudau01 &
subeur01 & suzeitp02 &sudau02 & subeur02 & suzeitp03 & sudau03 & subeur03 & suzeitp04 & sudau04 & subeur04 & suzeitp05 & sudau05 & subeur05
IF ssujaaz= 5

av:

kh:

fv:

hv:

fo:

tr: GOTO A_51a IF h_split=1 
    GOTO A_51b IF h_split=2 
    
hi1: Bitte 5 Akkordeons mit den Überschriften 1. Unterbrechung, 2. Unterbrechung, 3. Unterbrechung, 4. Unterbrechung, 5. Unterbrechung linksbündig untereinander anlegen. Die Überschriften bitte in die erste Spalte der jeweiligen Akkordeons einfügen. 
hi2: Bitte die Drop-Downs und Eingabefelder pro Unterbrechung linksbündig nebeneinander anordnen.


\--------------------------------

D1_19 
===

tc:

vn: sask (sask1 / sask2 / sask3 / sask4)

qt: 5er-Skala mit horizontalen ao

hl:

in:

q: Bitte beantworten Sie die folgenden Fragen ohne lange nachzudenken.

is:

it1: (sask1): Ich halte meine Begabung für das Studium für ...

it2: (sask2): Im Studium Neues zu lernen fällt mir ...

it3: (sask3): Meine studienbezogenen Fähigkeiten sind ...

it4: (sask4): Aufgaben im Rahmen des Studiums fallen mir ...

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

ao11 (sask3) 1 : :  ... niedrig

ao12 (sask3) 2

ao13 (sask3) 3

ao14 (sask3) 4

ao15 (sask3) 5: :  ... hoch

ao16 (sask4) 1 : :  ... schwer

ao17 (sask4) 2

ao18 (sask4) 3

ao19 (sask4) 4

ao20 (sask4) 5: :  ... leicht

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

vn: kom  (komsch / kommuen / kommbela / kommdurch / komteam / komvera / komplan / komkomm / komtext / komwiss / kommeth / kommwisl / komkrit / kominter)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte schätzen Sie ein, inwieweit Sie aktuell über die folgenden Fähigkeiten und Kenntnisse verfügen.

is:

it1: (komsch): schriftlicher Ausdruck

it2: (kommuen): mündlicher Ausdruck

it3: (kommbela): Belastbarkeit

it4: (kommdurch): Durchsetzungsfähigkeit

it5: (komteam): Teamfähigkeit

it6: (komvera): Übernahme von Verantwortung in Gruppen

it7: (komplan): Planungs- und Organisationsfähigkeit

it8: (komkomm): Kommunikation mit Professor\*innen

it9: (komtext): Verstehen wissenschaftlicher Texte

it10: (komwiss): Erarbeitung einer wissenschaftlichen Fragestellung

it11: (kommeth): Anwendung wissenschaftlicher Methoden

it12: (kommwisl): eigene Wissenslücken erkennen und schließen

it13: (komkrit): kritisches Denken/Ideen hinterfragen

it14: (kominter): fachübergreifendes Wissen und Denken

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

hi:

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


