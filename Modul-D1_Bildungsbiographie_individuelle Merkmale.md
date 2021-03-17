D1_1
==

tc:

vn: vtrae; vtraeo

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: An welcher Schule haben Sie die Hochschulzugangsberechtigung erworben?

is:

it:

st:

ao1: 1: staatliche Schule

ao2: 2: private Schule

ao3: 3: kirchliche Schule

ao4: 4: Andere Schule, und zwar: [(vtraeo); 50 Zeichen]

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
            <zofar:transition target="D1_2"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_2 
==

tc:

vn: prffach (prffach1 / prffach2 / prffach3 / prffach4 / prffach5)
    notefach (notefach1 / notefach2 / notefach3 / notefach4 / notefach5)

qt: Tableau / offene Angabe / Drop-Down

hl:

in:

q: Bitte nennen Sie uns Ihre schulischen Prüfungsfächer inklusive der jeweiligen Abschlussnote.

is: Punktzahl bitte in Note umrechnen.

it:

st:

ao1: (prffach1): [infield = 1. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao2: (prffach2): [infield = 2. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao3: (prffach3): [infield = 3. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao4: (prffach4): [infield = 4. Prüfungsfach; 60 Zeichen] (offene Angabe)

ao5: (prffach5): [infield = 5. Prüfungsfach; 60 Zeichen] (offene Angabe)


ao6: (notefach1): [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao7: (notefach2): [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao8: (notefach3): [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao9: (notefach4): [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

ao10: (notefach5): [infield = Note; sehr gut - gut - befriedigend - ausreichend - mangelhaft - ungenügend] (Dropdown)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo1: Wenn möglich, bitte die offene Angabe zum Prüfungsfach und das dazugehörige Drop-down mit der jeweiligen Note nebeneinander platzieren. Das ganze dann fünfmal bündig untereinander (2x5-Matrix). Hier bitte keine zeilenweise graue Schraffierung verwenden.

fo2: Sollte hi2 nicht möglich sein, bitte die Eingabefelder/Drop-Downs jeweils abwechselnd linksbündig untereinander platzieren (erst offen, dann drop-down, dann wieder offen, dann drop-down ...). Diesen Vorschlag mit grauer Schraffierung umsetzen, wobei jeweils Prüfungsfach/offene Angabe und dazugehörige Note/Drop-Down dann ggf. schraffiert werden (erste offene Angabe + Drop-down nicht schraffieren, zweite offene Abfrage + Drop-Down schraffieren , dritte offene Angabe + Drop-Down nicht schraffieren ...)

tr:

        <zofar:transitions>
            <zofar:transition target="D1_3"/>
        </zofar:transitions>

hi: 


\--------------------------------

D1_3 
==

tc:

vn: inkl (inklnein / inklja / inklschu)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Unabhängig davon, ob bei Ihnen selbst ein Förderbedarf bestand oder nicht: Wurden Sie jemals in einer Inklusionsklasse oder einer Förderschule unterrichtet?

is: Mit „Inklusionsklasse“ ist der gemeinsame Unterricht von Schüler\*innen mit und ohne sonderpädagogischen Förderbedarf gemeint.
#{layout.BREAK}
Bitte alles Zutreffende auswählen.

it: 

st:

ao1: (inklnein): nein, weder noch [EK]

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

tr:

        <zofar:transitions>
            <zofar:transition target="A_40"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_4 
==

tc: IF (vsbstyp= 10 | 11) | (vausbja=3)

vn: vausberufo; vausbzpjo; vausbzpmo; vausaufo; vausaufojo; vausaufomo

qt: offene Angabe / Drop-Down / Einfachauswahl / Exklusivkategorie

hl:

in:

q1: Welchen Beruf haben Sie (zuletzt) erlernt?

q2: Tragen Sie hier bitte Ihre Berufsausbildung ein.

q3: Wann haben Sie die Berufsausbildung abgeschlossen?

q4: Tragen Sie hier bitte Ihre Aufstiegsfortbildung ein.

q5: Wann haben Sie die Aufstiegsfortbildung abgeschlossen?

is1: Beispielsweise Mechatroniker/*in, Bankkauffrau oder-mann

is2: Beispielsweise Elektrotechnikmeister/*in, Bankfachwirt/*in, Betriebswirt/*in

it:

st:

ao1: (vausberufo): [infield = erlernter Beruf; 80 Zeichen] (offene Angabe)

ao2a: (vausbzpjo): [infield = Jahr; 2021 - 2020 - 2019 - ... - 1950] (Dropdown)

ao2b: (vausbzpmo): [infield = Monat; Januar - Februar - März - ... - Dezember] (Dropdown)

ao3: (vausaufo): [infield = Aufstiegsfortbildung; 80 Zeichen] (offene Angabe)

ao4a: (vausaufojo): [infield = Jahr; 2021 - 2020 - 2019 - ... - 1950] (Dropdown)

ao4b: (vausaufomo): [infield = Monat; Januar - Februar - März - ... - Dezember] (Dropdown)

mv:

ka:

vc: Show q4 AND q5 AND is2 AND ao3 AND ao4a AND ao4b if (vsbstyp10 = 1 OR vsbstyp11 = 1)

av:

kh: 

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D1_5"/>
        </zofar:transitions>

hi: Auf dieser Seite werden untereinander drei Fragen mit den zugehörigen Antwortoptionen usw. dargestellt (zuerst q1 mit ao1, dann q2 mit ao2a und ao2b sowie abschließend q3 mit is3, ao3a, kh3a und ao3b). ao2a und ao2b bitte nebeneinander darstellen, ao3a und ao3b können gerne linksbündig untereinander darsgestellt werden. Wichtig: ao3a bitte als NUMBER mit einer Dezimalstelle programmieren und nicht als Textfeld/string!

\--------------------------------

D1_7 
==

tc: IF (ssemhs <= 4 | isMissing(ssemhs)) 

vn: stfw (stfwein / stfwart / stfwalt / stfwzeit / stfwfam / stfwber / stfwbega / stfwint / stfwwiss / stfwverf / stfwverb / stfwand / stfwando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen Studienfaches? 

is:

it1: (stfwein): Einkommens- und Karrierechancen

it2: (stfwart): gute Aussichten auf sicheren Arbeitsplatz 

it3: (stfwalt): keine Zulassung im gewünschten Studienfach

it4: (stfwzeit): kurze Studienzeiten

it5: (stfwfam): Eltern/Familie haben mir dazu geraten

it6: (stfwber): fester Berufswunsch

it7: (stfwbega): eigene Begabung

it8: (stfwint): spezielles Fachinteresse

it9: (stfwwiss): eine gute wissenschaftliche Ausbildung

it10: (stfwverf): Vereinbarkeit von Familie mit späteren Beschäftigungsmöglichkeiten

it11: (stfwverb): Vereinbarkeit meiner Beeinträchtigung(en) mit späteren Beschäftigungsmöglichkeiten

it12: (stfwand): Anderes, und zwar: [(stfwando); 100 Zeichen]

st:

ao1: 1: gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv:

ka:

vc: SHOW it11 (stfwverb) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh: 

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D1_8"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_8 
==

tc: IF (ssemhs <= 4 | isMissing(ssemhs)) | (sabsan = 2)

vn: hsw (hswkont / hswbed / hswatt / hswfach / hswrank / hswtrad / hswzul / hswint / hswtz / hswsupp / hswbarr / hswand / hswando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen Hochschule?

is:

it1: (hswkont): Freund\*innen/Familie vor Ort

it2: (hswbed): günstige Lebensbedingungen am Hochschulort

it3: (hswatt): Attraktivität von Stadt und Umgebung

it4: (hswfach): gewünschte Fachrichtung

it5: (hswrank): gute Platzierung meines Fachs in Rankings

it6: (hswtrad): Tradition und Ruf der Hochschule

it7: (hswzul): keine Zulassung an Wunschhochschule

it8: (hswint): internationale Ausrichtung der Hochschule

it9: (hswtz): Möglichkeit, in Teilzeit studieren zu können

it10: (hswsupp): hochschulspezifische Beratungs- und Unterstützungsangebote

it11: (hswbarr): Barrierefreiheit der Hochschule

it12: (hswand): Anderes, und zwar: [(hswando); 100 Zeichen]

st:

ao1: 1: gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv:

ka:

vc: SHOW it11 (hswbarr) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh: 

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D2_6" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==14)"/>
            <zofar:transition target="A_44" condition="(zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==9             or zofar.asNumber(mastersplit)==10)"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_10 
===

tc: IF sabserbl1 = 0 

vn: sabserbl

qt: Drop-Down

hl:

in:

q: In welchem Bundesland liegt die Hochschule, an der Sie Ihren letzten Hochschulabschluss erworben haben?

is:

it1: (sabserbl): [infield = Bundesland] (Drop-Down)

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
            <zofar:transition target="D1_11" condition="(zofar.asNumber(sabserbl)==2            or zofar.asNumber(sabserbl)==3             or zofar.asNumber(sabserbl)==4             or zofar.asNumber(sabserbl)==5             or zofar.asNumber(sabserbl)==6             or zofar.asNumber(sabserbl)==7             or zofar.asNumber(sabserbl)==8             or zofar.asNumber(sabserbl)==9             or zofar.asNumber(sabserbl)==10             or zofar.asNumber(sabserbl)==11             or zofar.asNumber(sabserbl)==12             or zofar.asNumber(sabserbl)==13             or zofar.asNumber(sabserbl)==14             or zofar.asNumber(sabserbl)==15             or zofar.asNumber(sabserbl)==16             or zofar.asNumber(sabserbl)==17)"/>
            <zofar:transition target="D1_11a" condition="zofar.asNumber(sabserbl)==18"/>
            <zofar:transition target="D1_12" condition="zofar.isMissing(sabserbl) or zofar.asNumber(sabserbl)==0"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_11 
====

tc: IF sabserbl = 1 – 16 

vn: sabserhs1 / sabserhs2

qt: Drop-Down / offene Angabe

hl:

in:

q1: An welcher Hochschule haben Sie Ihren Abschluss erworben?

q2: Sollte Ihre Hochschule nicht aufgeführt sein, tragen Sie diese bitte hier ein (z. B. HU Berlin, FH Bielefeld):

is:

it:

st:

ao1: (sabserhs1): [infield = Hochschule] (Drop-Down)

ao2: (sabserhs2): [infield = Hochschule; 100 Zeichen] (offene Nennung)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: q1 und ao1 bitte zusammen oberhalb von q2 und ao2 platzieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D1_12"/>
        </zofar:transitions>

hi: Das Drop-Down zu sabserhs1 wird mit einer von uns noch zu lieferenden Hochschulliste (vorgefiltert nach Bundesland) gefüllt.

\--------------------------------


D1_11a 
====

tc: IF sabserbl = 17

vn: sabserhs3 / sabserhs4

qt: offene Angabe

hl:

in:

q: An welcher ausländischen Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao1: (sabserhs3): [infield = Land; 100 Zeichen] 

ao2: (sabserhs4): [infield = Hochschule; 100 Zeichen] 

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
            <zofar:transition target="D1_12"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_12 
===

tc: IF sabsja=2 

vn: sabserfacho1; sabserfacho2

qt: offene Angabe

hl:

in:

q: In welchem Fach haben Sie diesen Abschluss erworben?

is:

it:

st:

ao1: (sabserfacho1): [infield =  1. Studienfach; 80 Zeichen]

ao2: (sabserfacho2): [infield =  2. Studienfach; 80 Zeichen]

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
            <zofar:transition target="A_49a" condition="zofar.asNumber(sabser)==1"/>
            <zofar:transition target="A_49b" condition="zofar.asNumber(sabser)!=1 or zofar.isMissing(sabser)"/>
        </zofar:transitions>
    
hi:

\--------------------------------

D1_13 
===

tc:

vn: absterm

qt: Drop-Down

hl:

in:

q: Wann werden Sie Ihr derzeitiges Studium voraussichtlich abschließen?

is: 

it: 

st:

ao: (absterm): [infield = Semester; Sommersemester 2021 - Wintersemester 2021/22 - Sommersemester 2022 ... - Sommersemester 2030] (Drop-Down) 

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

\--------------------------------

D1_13 (Fortsetzung D1_13)
===
tc: IF NRW / zusatzsplit ==1

vn: nrwregel

qt: Einfachauswahl mit horizontaler ao

hl:

in:

q: Wie wichtig ist Ihnen ein Abschluss in Regelstudienzeit?

is: Die Regelstudienzeit entspricht der Anzahl an Fachsemestern, die der Studienverlaufsplan vorsieht.

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
            <zofar:transition target="A_27"/>
        </zofar:transitions>

hi: 

\--------------------------------

D1_15 
===

tc: IF ssweijaaz>=1 und/oder saweijaaz>=1 und/oder shwijaaz>=1 

vn: beginn01 – beginn05 / ende01 – ende05 / hs01 – hs05 / fach01 – fach05 / abs01 – abs05 / stand01 – stand05 

qt: Akkordeon / Tableau / Drop-Down / offene Angaben / Einfachauswahl

hl:

in:

q: Bitte tragen Sie die wesentlichen Stationen Ihres Studienverlaufs in das nachfolgende Tableau ein.

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit Studienbeginn.

it1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): [infield = Beginn] (Drop-Down)

it2: (ende01 / ende02 / ende03 / ende04 / ende05): [infield = Ende] (Drop-Down)

it3: (hs01 / hs02 / hs03 / hs04 / hs05): [infield = Hochschule; 100 Zeichen] (offene Angabe)

it4: (fach01 / fach02 / fach03 / fach04 / fach05): [infield = Studienfach; 80 Zeichen] (offene Angabe)

it5: (abs01 / abs02 / abs03 / abs04 / abs05): [infield = angestrebter Abschluss] (Drop-Down)

it6: (stand01 / stand02 / stand03 / stand04 / stand05): letzter Stand [Einfachauswahl]

st:

ao1: (beginn01 / beginn02 / beginn03 / beginn04 / beginn05): 1: Sommersemester 2021 \ 2: Wintersemester 2020/2019 \ 3: Sommersemester 2019 \ 4: Wintersemester 2018/2019 \ ... 23: Sommersemester 2010 \ 24: vor Sommersemester 2010

ao2: (ende01 / ende02 / ende03 / ende04 / ende05): 1: Sommersemester 2021 \ 2: Wintersemester 2020/2019 \ 3: Sommersemester 2019 \ 4: Wintersemester 2018/2019 \ ... 23: Sommersemester 2010 \ 24: vor Sommersemester 2010

ao3: (hs01 / hs02 / hs03 / hs04 / hs05): [infield = Hochschule; 100 Zeichen] 

ao4: (fach01 / fach02 / fach03 / fach04 / fach05): [infield = Studienfach; 80 Zeichen] 

ao5: (abs01 / abs02 / abs03 / abs04 / abs05): 1: Bachelor \ 2: Bachelor (Lehramt) \ 3: Master \ 4: Master (Lehramt) \ 5: Staatsexamen \ 6: Staatsexamen (Lehramt) \ 7: Diplom \ 8: Magister \ 9: Promotion (Dr., PhD) \ 10: anderer Abschluss (bspw. Ausländischer Abschluss) \ 11: kein Studienabschluss

ao6: (stand01 / stand02 / stand03 / stand04 / stand05): 1: läuft noch \ 2: abgeschlossen \ 3: abgebrochen \ 4: unterbrochen

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
            <zofar:transition target="D1_15b" condition="zofar.asNumber(techepi)==2"/>
            <zofar:transition target="D1_16" condition="zofar.asNumber(ssuja)==1"/>
            <zofar:transition target="A_51a" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_51b" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>
    
hi1: Bitte 5 Akkordeons mit den Überschriften (!!in fett!!) !!1. Studienepisode!!, !!2. Studienepisode!!, !!3. Studienepisode!!, !!4. Studienepisode!!, !!5. Studienepisode!! linksbündig untereinander anlegen. 

hi2: Bitte die Drop-Downs und Eingabefelder pro Episode linksbündig nebeneinander anordnen. Sollte das nicht möglich sein, bitte pro Episode linksbündig untereinander anordnen.

hi3: Bitte bei it6/ao6 (!!in fett!!) !!letzter Stand!! darüber positionieren.

\--------------------------------

D1_16 
===

tc: IF ssuja=1 

vn: suzeitp01 / suzeitp02 / suzeitp03 / suzeitp04 / suzeitp05 / sudau01 / sudau02 / sudau03 / sudau04 / sudau05 / subeur01 / subeur02 / subeur03 / subeur04 / subeur05

qt: Tableau / Drop-Down / Einfachauswahl

hl:

in:

q1: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q2: Bitte beschreiben Sie Ihre Studienunterbrechungen näher.

q3: Bitte beschreiben Sie Ihre letzten fünf Studienunterbrechungen näher.

is: 

it1: (suzeitp01 / suzeitp02 / suzeitp03 / suzeitp04 / suzeitp05): Präfix: Zeitpunkt [infield = Semester] (Drop-Down)

it2: (sudau01 / sudau02 / sudau03 / sudau04 / sudau05): Präfix: Dauer [infield = Monate] (Drop-Down)

it3: (subeur01 / subeur02 / subeur03 / subeur04 / subeur05): Präfix: Beurlaubung [Einfachauswahl]

st:

ao1: (suzeitp01 / suzeitp02 / suzeitp03 / suzeitp04 / suzeitp05): 1: Sommersemester 2021 \ 2: Wintersemester 2020/2019 \ 3: Sommersemester 2019 \ 4: Wintersemester 2018/2019 \ ... 23: Sommersemester 2010 \ 24: vor Sommersemester 2010

ao2: (sudau01 / sudau02 / sudau03 / sudau04 / sudau05): 1: 1 Monat \ 2: 2 Monate \ 3: 3 Monate \ 4: 4 Monate \ ... \ 24: 24 Monate und mehr

ao3: (subeur01 / subeur02 / subeur03 / subeur04 / subeur05) 1: ja; 2: nein

mv:

ka:

vc1: SHOW q1 AND suzeitp01 & sudau01 & subeur01 IF ssuja=1

vc2: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 IF ssuja=2

vc3: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 & suzeitp03 & sudau03 & subeur03 IF ssuja=

vc4: SHOW q2/is1 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 & sudau02 &
subeur02 & suzeitp03 & sudau03 & subeur03 & suzeitp04 & sudau04 & subeur04 IF ssuja=4

vc5: SHOW q3/is2 AND suzeitp01 & sudau01 & subeur01 & suzeitp02 &sudau02 & subeur02 & 
suzeitp03 & sudau03 & subeur03 & suzeitp04 & sudau04 & subeur04 & suzeitp05 & sudau05 & subeur05 IF ssuja= 5

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_51a" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="A_51b" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>
    
hi1: Bitte 5 Zeilen programmieren, in denen jeweils ganz vorne/in der ersten Spalte (!!in fett!!) !!1. Unterbrechung!!, !!2. Unterbrechung!!, !!3. Unterbrechung!!, !!4. Unterbrechung!! und !!5. Unterbrechung!! linksbündig untereinander stehen. Die beiden Drop-Downs und die Einfachauswahl dann bitte pro Unterbrechung/Zeile linksbündig nebeneinander anordnen/folgen lassen. Diese drei Spalten bitte (!!in fett!!) mit !!Zeitpunkt!!, !!Dauer!! und !!Beurlaubung!! überschreiben.

hi2: Sollte hi1 nicht möglich sein, bitte die einzelnen Unterbrechungsepisoden linksbündig untereinander umsetzen.

\--------------------------------

D1_19 
===

tc:

vn: sask (sask1 / sask2 / sask3 / sask4)

qt: Einfachauswahl/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte beantworten Sie die folgenden Fragen ohne lange nachzudenken.

is:

it1: (sask1): Ich halte meine Begabung für das Studium für ...

it2: (sask2): Im Studium Neues zu lernen fällt mir ...

it3: (sask3): Meine studienbezogenen Fähigkeiten sind ...

it4: (sask4): Aufgaben im Rahmen des Studiums fallen mir ...

st:

ao1 (sask1) 1:  ... niedrig

ao2 (sask1) 2

ao3 (sask1) 3

ao4 (sask1) 4

ao5 (sask1) 5:  ... hoch

ao6 (sask2) 1:  ... schwer

ao7 (sask2) 2

ao8 (sask2) 3

ao9 (sask2) 4

ao10 (sask2) 5:  ... leicht

ao11 (sask3) 1:  ... niedrig

ao12 (sask3) 2

ao13 (sask3) 3

ao14 (sask3) 4

ao15 (sask3) 5:  ... hoch

ao16 (sask4) 1:  ... schwer

ao17 (sask4) 2

ao18 (sask4) 3

ao19 (sask4) 4

ao20 (sask4) 5:  ... leicht

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
            <zofar:transition target="D2_13" condition="(zofar.asNumber(mastersplit)==1                 or zofar.asNumber(mastersplit)==2                 or zofar.asNumber(mastersplit)==7                 or zofar.asNumber(mastersplit)==8                 or zofar.asNumber(mastersplit)==14) "/>
            <zofar:transition target="A_23" condition="(zofar.asNumber(mastersplit)==3                 or zofar.asNumber(mastersplit)==4                 or zofar.asNumber(mastersplit)==9                 or zofar.asNumber(mastersplit)==10) "/>
        </zofar:transitions>

hi:

\--------------------------------

D1_20 
===

tc:

vn: kom  (komsch / kommuen / kombela / komdurch / komteam / komvera / komplan / komkomm / komtext / komwiss / kommeth / 
komwisl / komkrit / kominter / komdig)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit würden Sie sich die folgenden Fähigkeiten und Kenntnisse zuschreiben?

is:

it1: (komsch): schriftlicher Ausdruck

it2: (kommuen): mündlicher Ausdruck

it3: (kombela): Belastbarkeit

it4: (komdurch): Durchsetzungsfähigkeit

it5: (komteam): Teamfähigkeit

it6: (komvera): Übernahme von Verantwortung in Gruppen

it7: (komplan): Planungs- und Organisationsfähigkeit

it8: (komkomm): Kommunikation mit Professor\*innen

it9: (komtext): Verstehen wissenschaftlicher Texte

it10: (komwiss): Erarbeitung einer wissenschaftlichen Fragestellung

it11: (kommeth): Anwendung wissenschaftlicher Methoden

it12: (komwisl): eigene Wissenslücken erkennen und schließen

it13: (komkrit): kritisches Denken/Ideen hinterfragen

it14: (kominter): fachübergreifendes Wissen und Denken

it15: (komdig): digitale Kompetenzen

st:

ao1: 1: gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: in hohem Maße

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
            <zofar:transition target="D1_21"/>
        </zofar:transitions>

hi:

\--------------------------------

D1_21 
===

tc:

vn: kspr (ksprdeu / kspreng / ksprfra / ksprspa / ksprand1 / ksprando1 / ksprand2 / ksprando2 / ksprand3 / ksprando3)

qt: Einfachauswahlmatrix/offene Angaben mit horizontalen ao

hl:

in:

q: Wie gut beherrschen Sie die folgenden Sprachen?

is:

it1: (ksprdeu): Deutsch

it2: (kspreng): Englisch

it3: (ksprfra): Französisch

it4: (ksprspa): Spanisch

it5: (ksprand1): [(ksprando1); 60 Zeichen] (offene Angabe)

it6: (ksprand2): [(ksprando2); 60 Zeichen] (offene Angabe)

it7: (ksprand3): [(ksprando3); 60 Zeichen] (offene Angabe)

st:

ao1: 1: keine Kenntnisse

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr gute Kenntnisse

ao6: 6: Muttersprache

mv:

ka: (it5 TO it7): Andere Sprache(n), und zwar:

vc:

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="D1_22" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="D1_23" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi1: Bitte über die drei offenen Angaben eine Zeile linksbündig einfügen mit "Andere Sprache(n), und zwar:"

hi2: "Muttersprache" bitte etwas nach rechts absetzen und ohne Verbindungslinie.

\--------------------------------

D1_22 
===

tc:

vn: dpfrag / dsfreiz / sfklaus / ssverl

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1: (dpfrag): In die meisten meiner Lehrveranstaltungen gehe ich mit Fragen, auf die ich nach Antworten suche.

it2: (dsfreiz): Ich nutze meine Freizeit häufig dafür, mehr über interessante Themen zu erfahren, die wir in Lehrveranstaltungen diskutiert haben.

it3: (sfklaus): Ich sehe keinen Grund darin Stoff zu lernen, der wahrscheinlich nicht klausurrelevant ist.

it4: (ssverl): Ich lerne nur das ernsthaft, was in meinem Studium verlangt wird.

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

tr:

        <zofar:transitions>
            <zofar:transition target="D1_24"/>
        </zofar:transitions>
        
hi: Rotierung der Items bitte entfernen.

\--------------------------------

D1_23 
===

tc:

vn: kogorga / kogkrit / kogwied / mkogwach / ressanst / resskonz / lernumg / lit / digmat

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Im Folgenden möchten wir gerne mehr darüber erfahren, wie Sie lernen. Bitte geben Sie für jede der folgenden Lerntätigkeiten an, wie oft Sie diese ausführen. 

is:

it1: (lernumg): Ich gestalte meinen Arbeitsplatz so, dass ich alles schnell finden kann.

it2: (kogorga): Ich stelle mir aus Mitschrift, Skript oder Literatur kurze Zusammenfassungen zusammen.

it3: (digmat): Ich nutze digitale Lehr- und Lernmaterialien.

it4: (mkogwach): Um Wissenslücken festzustellen, rekapituliere ich die wichtigsten Inhalte ohne 
meine Unterlagen zu Hilfe zu nehmen.

it5: (kogwied): Ich lerne den Lernstoff möglichst auswendig.

it6: (ressanst): Ich lerne auch spätabends und am Wochenende, wenn es sein muss.

it7: (resskonz): Beim Lernen fällt es mir schwer, bei der Sache zu bleiben.

it8: (kogkrit): Ich denke über Alternativen zu Schlussfolgerungen in den Lehrtexten nach.

it9: (lit): Ich suche nach weiterführender Literatur, wenn mir bestimmte Inhalte noch nicht ganz klar sind.

st:

ao1: 1: sehr selten

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr oft

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
            <zofar:transition target="D1_24"/>
        </zofar:transitions>
        
hi: Rotierung der Items bitte entfernen.

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

it9: (pbigkrea): Ich habe eine aktive Vorstellungskraft, bin fantasievoll.

it10: (pbignoku): Ich habe nur wenig künstlerisches Interesse.

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

tr:

        <zofar:transitions>
            <zofar:transition target="D1_25"/>
        </zofar:transitions>

hi: Rotierung der Items bitte entfernen.

\--------------------------------

D1_25 
===

tc:

vn: psw (pswskill / pswkraft / pswaufg)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1: (pswskill): In schwierigen Situationen kann ich mich auf meine Fähigkeiten verlassen.

it2: (pswkraft): Die meisten Probleme kann ich aus eigener Kraft gut meistern.

it3: (pswaufg): Auch anstrengende und komplizierte Aufgaben kann ich in der Regel gut lösen.

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

tr:

        <zofar:transitions>
            <zofar:transition target="D1_26"/>
        </zofar:transitions>

hi: Items bitte zufällig rotieren

\--------------------------------

D1_29 
===

tc:

vn: intsoc1b / intsoc3b / intsoc4b / intinv1b / intinv2b / intinv4b / intart1b / intart2b / intart4b / intent1b / intent2b / intent3b / Intconv2b / intconv3b / intconv4b / intreal1b / intreal2b / intreal3b

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte geben Sie an, wie sehr Sie sich für folgende Tätigkeiten interessieren. 

is:

it1: (intsoc1b): anderen Menschen helfen

it2: (intsoc3b): sich mit den Lebenslagen von Menschen/Gruppen auseinandersetzen

it3: (intsoc4b): mit Menschen (zusammen)arbeiten

it4: (intinv1b): etwas genau beobachten und analysieren

it5: (intinv2b): Unbekanntes erforschen, experimentieren

it6: (intinv4b): Lösungen für komplexe Probleme finden

it7: (intart1b): kreativ/gestaltend tätig sein

it8: (intart2b): sich mit Kunst und Kultur befassen

it9: (intart4b): etwas sprachlich ansprechend formulieren

it10: (intent1b): Unternehmen gründen oder leiten

it11: (intent2b): andere von einer Sache überzeugen

it12: (intent3b): andere Menschen anleiten oder führen

it13: (Intconv2b): sich mit rechtlichen Fragen beschäftigen

it14: (intconv3b): Arbeitsprozesse planen

it15: (intconv4b): mit Zahlen oder Statistiken arbeiten

it16: (intreal1b): untersuchen, wie Dinge funktionieren

it17: (intreal2b): innovative technische Lösungen entwickeln

it18: (intreal3b): an Soft- oder Hardware arbeiten

st:

ao1: 1: überhaupt nicht

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

hi: Items bitte blockweise rotieren in folgen drei Blöcken: (intreal1b, intinv1b, intart1b, intsoc1b, intent1b, Intconv2b) (intreal2b, intinv2b, intart2b, intsoc3b, intent2b, Intconv3b) (intreal3b, intinv4b, intart4b, intsoc4b, intent3b, intconv4b).

\--------------------------------

D1_30 
===

tc:

vn: semtag

qt: Einfachauswahl mit vertikalen ao´s

hl:

in:

q: Wenn Sie an dieses Semester denken: An wie vielen Tagen in der Woche sind Sie an Ihrer Hochschule?
An...

is:

it:

st:

ao1: 1: ... keinem Tag

ao2: 2: ... 1 Tag

ao3: 3: ... 2 Tagen

ao4: 4: ... 3 Tagen

ao5: 5: ... 4 Tagen

ao6: 6: ... 5 Tagen

ao7: 7: ... 6 Tagen

ao8: 8: ... 7 Tagen

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
