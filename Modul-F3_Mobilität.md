F3_6
=====

tc:

vn: azufmob

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Trauen Sie sich zu, ein komplettes Studium im Ausland zu absolvieren?

is:

it:

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
            <zofar:transition target="F3_7" condition="(zofar.asNumber(ainfaus) ge 2)"/>
            <zofar:transition target="F3_16" condition="(zofar.asNumber(ainfaus)==1          and zofar.asNumber(auslandint)==4)"/>
            <zofar:transition target="F3_16" condition="(zofar.isMissing(ainfaus)          and zofar.asNumber(auslandint)==4)"/>
            <zofar:transition target="F3_21" condition="(zofar.asNumber(ainfaus)==1)          and (zofar.asNumber(auslandint)==1          or zofar.asNumber(auslandint)==2          or zofar.asNumber(auslandint)==3)"/>
            <zofar:transition target="F3_21" condition="(zofar.isMissing(ainfaus))          and (zofar.asNumber(auslandint)==1          or zofar.asNumber(auslandint)==2          or zofar.asNumber(auslandint)==3)"/>
            <zofar:transition target="F3_21" condition="(zofar.isMissing(ainfaus)          and zofar.isMissing(auslandint))"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_7 
=====

tc: 

vn: ainfa1; ainflo1; ainfsto1; ainfbm1; ainfbj1, ainfdau1
    ainfa2; ainflo2; ainfsto2; ainfbm2; ainfbj2, ainfdau2
    ainfa3; ainflo3; ainfsto3; ainfbm3; ainfbj3, ainfdau3
    
qt: Einfachauswahl mit Dropdown und offene Angaben

hl:

in:

q1: Bitte beschreiben Sie Ihren studienbezogenen Auslandsaufenthalt näher.

q2: Bitte beschreiben Sie Ihre beiden studienbezogenen Auslandsaufenthalte näher.

q3: Bitte beschreiben Sie Ihre drei studienbezogenen Auslandsaufenthalte näher.

is:

it:

st:

ao1: (ainfa1): [infield = Art des Aufenthalts; Auslandsstudium mit Abschluss - ... - sonstiger Aufenthalt] (Dropdown)

    (ainfa1): 1: Auslandsstudium mit Abschluss

    (ainfa1): 2: Auslandssemester
    
    (ainfa1): 3: Auslandspraktikum/-praxisphase

    (ainfa1): 4: Sprachkurs

    (ainfa1): 5: Studienreise

    (ainfa1): 6: Projektarbeit

    (ainfa1): 7: Summer School

    (ainfa1): 8: sonstiger Aufenthalt


ao2: (ainflo1): [infield = Land; 100 Zeichen] (offene Angabe)

ao3: (ainfsto1): [infield = Stadt/Hochschule; 100 Zeichen] (offene Angabe)


ao4: (ainfbm1): [infield = Monat; Januar - Februar - ... - November - Dezember] (Dropdown)

ao5: (ainfbj1): [infield = Jahr; 2021 - 2010 - ... - 2009 - vor 2009] (Dropdown)


ao6: (ainfdau1): [infield = Dauer des Aufenthalts; 1 Monat - 2 Monate - ... - 12 Monate - 13 bis 18 Monate - 19 bis  24 Monate - 25 bis 30 Monate - 31 bis 36 Monate - mehr als 36 Monate] (Dropdown)


ao7: (ainfa2): [infield = Art des Aufenthalts; Auslandsstudium mit angestrebtem Abschluss im Ausland - ... - sonstiger Aufenthalt] (Dropdown)

    (ainfa2): 1: Auslandsstudium mit Abschluss

    (ainfa2): 2: Auslandssemester
    
    (ainfa2): 3: Auslandspraktikum/-praxisphase

    (ainfa2): 4: Sprachkurs

    (ainfa2): 5: Studienreise

    (ainfa2): 6: Projektarbeit

    (ainfa2): 7: Summer School

    (ainfa2): 8: sonstiger Aufenthalt


ao8: (ainflo2): [infield = Land; 100 Zeichen] (offene Angabe)

ao9: (ainfsto2): [infield = Stadt/Hochschule; 100 Zeichen] (offene Angabe)


ao10: (ainfbm2): [infield = Monat; Januar - Februar - ... - November - Dezember] (Dropdown)

ao11: (ainfbj2): [infield = Jahr; 2021 - 2010 - ... - 2009 - vor 2009] (Dropdown)


ao12: (ainfdau2): [infield = Dauer des Aufenthalts; 1 Monat - 2 Monate - ... - 12 Monate - 13 bis 18 Monate - 19 bis  24 Monate - 25 bis 30 Monate - 31 bis 36 Monate - mehr als 36 Monate] (Dropdown)


ao13: (ainfa3): [infield = Art des Aufenthalts; Auslandsstudium mit angestrebtem Abschluss im Ausland - ... - sonstiger Aufenthalt] (Dropdown)

    (ainfa3): 1: Auslandsstudium mit Abschluss

    (ainfa3): 2: Auslandssemester
    
    (ainfa3): 3: Auslandspraktikum/-praxisphase

    (ainfa3): 4: Sprachkurs

    (ainfa3): 5: Studienreise

    (ainfa3): 6: Projektarbeit

    (ainfa3): 7: Summer School

    (ainfa3): 8: sonstiger Aufenthalt


ao14: (ainflo3): [infield = Land; 100 Zeichen] (offene Angabe)

ao15: (ainfsto3): [infield = Stadt/Hochschule; 100 Zeichen] (offene Angabe)


ao16: (ainfbm3): [infield = Monat; Januar - Februar - ... - November - Dezember] (Dropdown)

ao17: (ainfbj3): [infield = Jahr; 2021 - 2010 - ... - 2009 - vor 2009] (Dropdown)


ao18: (ainfdau3): [infield = Dauer des Aufenthalts; 1 Monat - 2 Monate - ... - 12 Monate - 13 bis 18 Monate - 19 bis  24 Monate - 25 bis 30 Monate - 31 bis 36 Monate - mehr als 36 Monate] (Dropdown)


st:

ao:

mv:

ka1 (ao1 TO ao6): !!Letzter Auslandsaufenthalt!!

ka2 (ao4 TO ao5): Start des Aufenthalts:

ka3 (ao7 TO ao12): !!Vorletzter Auslandsaufenthalt!!

ka4 (ao10 TO ao11): Start des Aufenthalts:

ka5 (ao13 TO ao18): !!Drittletzter Auslandsaufenthalt!!

ka6 (ao16 TO ao17): Start des Aufenthalts:


vc:

SHOW q1 AND ao1 TO ao6 AND ka1 TO ka2 IF ainfaus == 2 \| kA

SHOW q2 AND is1 AND ao1 TO ao12 AND ka1 TO ka4 IF ainfaus == 3

SHOW q3 AND is2 AND ao1 TO ao18 AND ka1 TO ka6 IF ainfaus == 4

av:

kh:

fv:

hv:

fo: Bitte jeweils "Art des Aufenthalts", "Land" und "Stadt/Hochschule" linkdbündig untereinander positionieren. Darunter dann linksbündig die Kategorienüberschrift "Start des Aufenthalts:" und darunter linksbündig "Monat" und daneben "Jahr". Zuletzt dann ebenfalls darunter linksbündig "Dauer des Aufenthalts". Das Ganze dann eben bis zu dreimal untereinander mit den Überschriften (fett und unterstrichen) "Letzter Auslandsaufenthalt", "Vorletzter Auslandsaufenthalt" und "Drittletzter Auslandsaufenthalt".

tr:

        <zofar:transitions>
            <zofar:transition target="F3_8"/>
        </zofar:transitions>

hi:

\--------------------------------

F3_8
====

tc: 

vn: aprono1; aproeras1; aprodaad1; aprohhs1; aprogahs1; aproanpr1
    aprono2; aproeras2; aprodaad2; aprohhs2; aprogahs2; aproanpr2
    aprono3; aproeras3; aprodaad3; aprohhs3; aprogahs3; aproanpr3

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q1: Fand Ihr studienbezogener Auslandsaufenthalt im Rahmen eines Programms statt?

q2: Fanden Ihre studienbezogenen Auslandsaufenthalte im Rahmen eines Programms statt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aprono1): nein (Exklusivkategorie)

ao2: (aproeras1): ERASMUS+, ERASMUS

ao3: (aprodaad1): DAAD-Programm

ao4: (aprohhs1): Programm meiner Heimathochschule

ao5: (aprogahs1): Programm der Gasthochschule

ao6: (aproanpr1): anderes Programm


ao7: (aprono2): nein (Exklusivkategorie)

ao8: (aproeras2): ERASMUS+, ERASMUS

ao9: (aprodaad2): DAAD-Programm

ao10: (aprohhs2): Programm meiner Heimathochschule

ao11: (aprogahs2): Programm der Gasthochschule

ao12: (aproanpr2): anderes Programm


ao13: (aprono3): nein (Exklusivkategorie)

ao14: (aproeras3): ERASMUS+, ERASMUS

ao15: (aprodaad3): DAAD-Programm

ao16 (aprohhs3): Programm meiner Heimathochschule

ao17: (aprogahs3): Programm der Gasthochschule

ao18: (aproanpr3): anderes Programm

mv:

ka1: (ao1 TO ao6): !!Letzter Auslandsaufenthalt!!

ka2: (ao2 TO ao6): Ja, und zwar:

ka3: (ao7 TO ao12): !!Vorletzter Auslandsaufenthalt!!

ka4: (ao8 TO ao12): Ja, und zwar:

ka5: (ao13 TO ao18): !!Drittletzter Auslandsaufenthalt!!

ka6: (ao14 TO ao18): Ja, und zwar:

vc:

SHOW q1 AND ao1 TO ao6 AND ka1 TO ka2 IF ainfaus == 2 OR ainfaus==MISSING

SHOW q2 AND ao1 TO ao12 AND ka1 TO ka4 IF ainfaus == 3

SHOW q2 AND is AND ao1 TO ao18 AND ka1 TO ka6 IF ainfaus == 4

av:

kh:

fv:

hv:

fo1: ao1, ao7 und ao13 jeweils etwas von den nachstehenden ao absetzen.

fo2: Bitte jeweils über ao2, ao8 und ao14 "Ja, und zwar:" linksbündig positionieren. 

fo3: Es werden bis zu drei Episoden angezeigt, die linksbündig untereinander mit den Überschriften (fett und unterstrichen) "Letzter  Auslandsaufenthalt", "Vorletzter Auslandsaufenthalt" und "Drittletzter Auslandsaufenthalt" positioniert werden.

tr:

        <zofar:transitions>
            <zofar:transition target="F3_9"/>
        </zofar:transitions>

hi:

\--------------------------------

F3_9 
=====

tc: 

vn: ainfcp

qt: Einfachauswahl

hl:

in:

q: Wurde Ihr letzter Auslandsaufenthalt auf Ihr Studium angerechnet?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, teilweise

ao3: 3: ja, vollständig

ao4: -11: Ich habe keine Leistungen erbracht.

mv: ao4

ka:

vc:

av:

kh:

fv:

hv:

fo: ao4 absetzen

tr:

        <zofar:transitions>
            <zofar:transition target="F3_10"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_10
=====

tc: 

vn: afinelt1; afinpar1; afinbaf1; afinjobv1; afinjobw1, afinstip1; afinkre1; afinand1
    afinelt2; afinpar2; afinbaf2; afinjobv2; afinjobw2; afinstip2; afinkre2; afinand2
    afinelt3; afinpar3; afinbaf3; afinjobv3; afinjobw3; afinstip3; afinkre3; afinand3

qt: Mehrfachauswahl

hl:

in:

q1: Wie haben Sie Ihren studienbezogenen Auslandsaufenthalt finanziert?

q2: Wie haben Sie Ihre studienbezogenen Auslandsaufenthalte finanziert?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (afinelt1): Eltern

ao2: (afinpar1): Partner\*in

ao3: (afinbaf1): BAföG

ao4: (afinjobv1): Verdienst aus Tätigkeit(en) vor dem Aufenthalt

ao5: (afinjobw1): Verdienst aus Tätigkeit(en) während des Aufenthalts

ao6: (afinstip1): Stipendium

ao7: (afinkre1): Bildungskredit

ao8: (afinand1): andere Finanzierungsquelle



ao9: (afinelt2): Eltern

ao10: (afinpar2): Partner\*in

ao11: (afinbaf2): BAföG

ao12: (afinjobv2): Verdienst aus Tätigkeiten vor dem Aufenthalt

ao13: (afinjobw2): Verdienst aus Tätigkeiten während des Aufenthalts

ao14: (afinstip2): Stipendium

ao15: (afinkre2): Bildungskredit

ao16: (afinand2): andere Finanzierungsquelle



ao17: (afinelt3): Eltern

ao18: (afinpar3): Partner\*in

ao19: (afinbaf3): BAföG

ao20: (afinjobv3): Verdienst aus Tätigkeiten vor dem Aufenthalt

ao21: (afinjobw3): Verdienst aus Tätigkeiten während des Aufenthalts

ao22: (afinstip3): Stipendium

ao23: (afinkre3): Bildungskredit 

ao24: (afinand3): andere Finanzierungsquelle

mv:

ka1 (ao1 TO ao8): !!Letzter Auslandsaufenthalt!!

ka2 (ao9 TO ao16): !!Vorletzter Auslandsaufenthalt!!

ka3 (ao17 TO ao24): !!Drittletzter Auslandsaufenthalt!!

vc:

SHOW q1 AND ao1 TO ao8 AND ka1 IF ainfaus==2 OR ainfaus==MISSING

SHOW q2 AND ao1 TO ao16 AND ka1 TO ka2 IF ainfaus==3

SHOW q2 AND ao1 TO ao24 AND ka1 TO ka3 IF ainfaus==4

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="F3_11"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_11 
======

tc:

vn: akont (akontgast; akontbuerg; akontdtst; akontintst)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie häufig haben Sie sich während des Aufenthalts unterhalten mit …

q2: Wie häufig haben Sie sich während des letzten Aufenthalts unterhalten mit …

is:

it1: (akontgast): … Studierenden des Gastlandes?

it2: (akontbuerg): … anderen Bürger\*innen des Gastlandes?

it3: (akontdtst): … deutschen Studierenden?

it4: (akontintst): … anderen internationalen Studierenden?

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig

mv:

ka:

vc:

SHOW q1 IF ainfaus == 2 OR ainfaus == MISSING

SHOW q2 IF ainfaus > 2

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="F3_12"/>
        </zofar:transitions>

hi:

\--------------------------------

F3_12 
======

tc: IF ainfaus > 1

vn: aprach (asprachland; asprachdeut; asprachand; asprachando)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: Wie häufig haben Sie während Ihres Auslandsaufenthalts die folgenden Sprachen gesprochen?

q2: Wie häufig haben Sie während Ihres letzten Auslandsaufenthalts die folgenden Sprachen gesprochen?

is:

it1: (asprachland): Landessprache des Gastlandes

it2: (asprachdeut): Deutsch

it3: (asprachand): Andere Sprache, und zwar: ([asprachando]; offene Angabe, 60 Zeichen)

st:

ao1: 1: nie

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr häufig

mv:

ka:

vc:

SHOW q1 IF ainfaus == 2 OR ainfaus == MISSING

SHOW q2 IF ainfaus > 2

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="F3_13"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_13 
======

tc: IF ainfaus > 1

vn: azuf (azuflernerf; azufinsg)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie in Bezug auf Ihren letzten studienbezogenen Auslandsaufenthalt mit …

is:

it1: (azuflernerf): … den gewonnenen fachlichen Kenntnissen?

it2: (azufinsg): … dem Aufenthalt insgesamt?

st:

ao1: 1: gar nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4:

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
            <zofar:transition target="F3_14"/>
        </zofar:transitions>
        

hi:


\--------------------------------

F3_14 
======

tc: IF ainfaus > 1

vn: azufleistanf; azuforgauf; azuffinauf

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: In Bezug auf Ihren letzten studienbezogenen Auslandsaufenthalt: Wie beurteilen Sie…

is:

it1: (azufleistanf): … die Leistungsanforderungen?

it2: (azuforgauf): … den organisatorischen Aufwand?

it3: (azuffinauf): … den finanziellen Aufwand?

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
            <zofar:transition target="F3_15"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_15
=====

tc: IF ainfaus > 1

vn: aeempf

qt: Einfachauswahl/5er-Skala mit vertikalen ao

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen: Würden Sie Ihren Freund\*innen/Bekannten empfehlen, im Ausland zu studieren?

is:

it:

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
            <zofar:transition target="F3_22"/>
        </zofar:transitions>

hi:

\-------------------------------- 

F3_16
=====

tc: IF (ainfaus=1 AND auslandint==4) OR (ainfaus=MISSING AND auslandint==4)

vn: aplanart

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Sie haben angegeben, dass Sie künftig einen (weiteren) studienbezogenen Auslandsaufenthalt beabsichtigen: 
Welche Art von Aufenthalt planen Sie?

is:

it:

st:

ao1: 1: Auslandsstudium mit Abschluss

ao2: 2: Auslandssemester

ao3: 3: Auslandspraktikum/-praxisphase

ao4: 4: Sprachkurs im Ausland

ao5: 5: Studienreise

ao6: 6: Projektarbeit

ao7: 7: Summer School

ao8: 8: anderer Auslandsaufenthalt

ao9: -12: weiß ich noch nicht

mv: ao9

ka:

vc:

av:

kh:

fv:

hv:

fo: "-12: weiß ich noch nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="F3_19"/>
        </zofar:transitions>

hi:

\--------------------------------

F3_17
=====

tc: IF (ainfaus=1 AND auslandint==4) OR (ainfaus=MISSING AND auslandint==4)

vn: aplan (aplanlando; aplanorto; aplanka)

qt: offene Angaben

hl:

in:

q: Wo planen Sie den Auslandsaufenthalt durchzuführen?

is: Sollten mehrere Orte infrage kommen, geben Sie bitte Ihren Favoriten an.

it:

st:

ao1: (aplanlando): Präfix: Land: [offene Angabe; 100 Zeichen]

ao2: (aplanorto): Präfix: Stadt/Hochschule: [offene Angabe, 100 Zeichen]

ao3:   (aplanka): weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: ao1 und ao2 bitte linksbündig untereinander positionieren. ao3 bitte etwas abgesetzt unter ao2 positionieren.

tr:

hi:

\--------------------------------

F3_19
=====

tc: IF (ainfaus=1 AND auslandint==4) OR (ainfaus=MISSING AND auslandint==4)

vn: aplan (aplaneras; aplandaad; aplanhhs; aplangahs; aplananpr; aplanno; aplankaa)

qt: Mehrfachauswahl mit vertikalen ao

hl:

q: Auf welche Weise möchten Sie Ihren künftigen Auslandsaufenthalt organisieren?

in: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aplaneras): ERASMUS+

ao2: (aplandaad): DAAD-Programm

ao3: (aplanhhs): Programm meiner Heimathochschule

ao4: (aplangahs): Programm der Gasthochschule

ao5: (aplananpr): anderes Programm

ao6: (aplanno): Ich werde den Aufenthalt selbst organisieren.

ao7: (aplankaa): weiß ich noch nicht [EK]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte ao7 optisch etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="F3_20"/>
        </zofar:transitions>

hi: 

\--------------------------------

F3_20
=====

tc: IF (ainfaus=1 AND auslandint==4) OR (ainfaus=MISSING AND auslandint==4)

vn: aplanfin (aplanfinelt; aplanfinpar; aplanfinbaf; aplanfinjobv; aplanfinjobw; aplanfinstip; aplanfinbkred; aplanfinand)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Wie werden Sie Ihren künftigen Auslandsaufenthalt voraussichtlich finanzieren?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (aplanfinelt): Eltern

ao2: (aplanfinpar): Partner\*in

ao3: (aplanfinbaf): BAföG

ao4: (aplanfinjobv): Verdienst aus Tätigkeit(en) vor dem Auslandsaufenthalt

ao5: (aplanfinjobw): Verdienst aus Tätigkeit(en) während des Auslandsaufenthalts

ao6: (aplanfinstip): Stipendium

ao7: (aplanfinbkred): Bildungskredit

ao8: (aplanfinand): andere Finanzierungsquelle

ao9: (aplanfinkaa): weiß ich noch nicht [EK]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: ao9 bitte etwas optisch absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="F3_22"/>
        </zofar:transitions>

hi:

\--------------------------------

F3_22
=====

tc:

vn: akont (akontdeust; akontneust)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig unterhalten Sie sich mit …

is:

it1: (akontdeust): … deutschen Studierenden?

it2: (akontneust): … internationalen Studierenden?

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
            <zofar:transition target="F3_23"/>
        </zofar:transitions>

hi:


\--------------------------------

F3_25
=====

tc:

vn: intpsy (intpsydeu; intpsyzeita; intpsydaua)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wenn Sie an Ihre Zukunft denken, wo möchten Sie leben?

is:

it1: (intpsydeu): in Deutschland

it2: (intpsyzeita): zeitweise im Ausland

it3: (intpsydaua): dauerhaft im Ausland

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
            <zofar:transition target="A_56"/>
        </zofar:transitions>

hi:
