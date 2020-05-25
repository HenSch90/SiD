

\--------------------------------

A_17
=========

tc:

vn: ssemfs

qt: offene Angabe

hl:

in:

q: Im wievielten Fachsemester befinden Sie sich zurzeit?

is: Fachsemester sind die Semester, die Sie in Ihrem derzeitigen Studiengang eingeschrieben sind.

it:

st:

ao: (ssemfs) Präfix: Fachsemester: [offene Angabe; Number, 2-stellig: 1 TO 99]

mv:

ka:

vc: 

av: 

kh: Bitte geben Sie die Anzahl Ihrer Fachsemester an (1 bis 99).

fv:

hv:

fo: 


tr: (siehe unten)

hi: 

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemhs

qt: offene Angabe

hl:

in:

q: Im wievielten Hochschulsemester befinden Sie sich zurzeit?

is: Hochschulsemester sind alle Semester seit Beginn des Studiums, einschließlich Urlaubs-, Auslands- und Praxissemester.

it:

st:

ao: (ssemhs) Präfix: Hochschulsemester: [offene Angabe; Number, 2-stellig: 1 TO 99]

mv:

ka:

vc:

av: 

kh: Bitte geben Sie die Anzahl Ihrer Hochschulsemester an (1 bis 99).

fv:

hv:

fo: 

tr: (siehe unten)

hi: 

\------------------------------------------------------------

A_17
=========

tc:

vn: ssemul

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Befinden Sie sich aktuell in einem Urlaubssemester?

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

GOTO CO_1

hi:

\------------------------------------------------------------

CO_1
=========

tc: 

vn: VCO_1

qt: Einfachauswahl mit vertikaler ao

hl:

in:

q: Halten Sie eine Verlängerung Ihres Studiums aufgrund der Corona-Pandemie für wahrscheinlich?
is:

it:

st:

ao1: 1: nein, sehr unwahrscheinlich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: ja, sehr wahrscheinlich


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

hi:

\------------------------------------------------------------


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

GOTO N_4

hi:

\--------------------------------

N_4
=========

tc: 

vn: nrwregel

qt: Einfachauswahl mit horizontalen ao

hl:

in:

q: Wie wichtig ist Ihnen ein Abschluss in Regelstudienzeit?
is:

it:

st:

ao1: 1: unwichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_2

hi:

\------------------------------------------------------------

CO_2
=========

tc:

vn: VCO_2a

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Hat sich die Corona-Pandemie auf Ihre ++bisherige++ Prüfungssituation ausgewirkt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: 1: … wie geplant durchgeführt.

ao2: 2: … abgesagt.

ao3: 3: … verschoben.
	
ao4: 4: … kurzfristig online durchgeführt.

ao5: 5: … durch andere Formen ersetzt.

mv:

ka1: Klausuren wurden …

vc:

av:

kh:

fv:

hv:

fo: 

tr: (siehe unten)

hi:

\------------------------------------------------------------

CO_2
=========

tc:

vn: VCO_2b

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: 

is:

it:

st:

ao1: 1: … wie geplant durchgeführt.

ao2: 2: … abgesagt.

ao3: 3: … verschoben.
	
ao4: 4: … kurzfristig online durchgeführt.

ao5: 5: … durch andere Formen ersetzt.

mv:

ka: Mündliche Prüfungen wurden …
vc:

av:

kh:

fv:

hv:

fo: 

tr: (siehe unten)

hi:

\------------------------------------------------------------

CO_2
=========

tc:

vn: VCO_2c

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: 

is:

it:

st:

ao1: 1: … wie geplant durchgeführt.

ao2: 2: … abgesagt.

ao3: 3: … verschoben.
	
ao4: 4: … kurzfristig online durchgeführt.

ao5: 5: … durch andere Formen ersetzt.

mv:

ka: Schriftliche Leistungen (z. B. Hausarbeiten, 
Abschlussarbeiten) wurden …


vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO N9_b

hi:

\------------------------------------------------------------


N_9b
=========

tc:

vn: digfor (digfor1; digfor2; digfor3; digfor4; digfor5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Im Zuge der Corona-Pandemie haben sich die Studienbedingungen in vielen Studiengängen verändert: Wie viele Ihrer Lehrveranstaltungen werden im Online- oder Präsenzformat angeboten?

is:

it1: (digfor1): … in diesem Semester

it2: (digfor2): … im letzten Semester

it3: (digfor3): … in diesem Semester

it4: (digfor4): … im letzten Semester

it5: (digfor5): … in diesem Semester

it6: (digfor6): … im letzten Semester

it7: (digfor7): … in diesem Semester

it8: (digfor8): … im letzten Semester


st:

ao1: 1: keine

ao2: 2:

ao3: 3: etwa die Hälfte

ao4: 4:

ao5: 5: alle 

mv:

ka1: (it1 TO it2): !! als reine Online-Veranstaltung (z. B. Online-Vorlesung, Online-Seminar)!!

ka2: (it3 TO it4): !! als Online-Selbststudium mit einzelnen Präsenzterminen!!

ka3: (it5 TO it6): !! als Präsenzveranstaltung mit einzelnen Online-Terminen!!

ka4: (it7 TO it8): !! als reine Präsenzveranstaltung!!

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_3

hi:


\------------------------------------------------------------

CO_3
-------

tc:

vn: ssstud (ssstud1; ssstud2; ssstud3; ssstud4; ssstud5; ssstud6; ssstud7; ssstud8)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie viele Ihrer Lehrveranstaltungen sind in diesem Semester wie folgt organisiert?

is: Damit sind Vorlesungen, Seminare und (praktische) Übungen gemeint.


it1: (ssstud1): … findet als Videokonferenz/Webinar statt.

it2: (ssstud2): … ist in virtuelle Lehr- und Lernräume eingebunden.

it3: (ssstud3): … ist als Video abrufbar.

it4: (ssstud4): … ist als Audioaufzeichnung abrufbar.

it5: (ssstud5): … findet über die Bereitstellung der Lehrmaterialien statt.

it6: (ssstud6): … basiert auf der regelmäßigen Vergabe zu bearbeitender Aufgaben.

it7: (ssstud7): … ist ersatzlos ausgefallen.

it8: (ssstud8): … soll zu einem späteren Zeitpunkt nachgeholt werden?

st:

ao1: 1: keine

ao2: 2:

ao3: 3: etwa die Hälfte

ao4: 4:

ao5: 5: alle

mv:

ka: Lehrveranstaltung …

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_4

hi: 

\------------------------------------------------------------

CO_4
=========

tc: 

vn: VCO_4

qt: Einfachauswahl mit horizontalen ao

hl:

in:

q: In wie vielen Online-Lehrveranstaltungen werden aktive Interaktionsmöglichkeiten angeboten?
is:	

it:

st:

ao1: 1: keine

ao2: 2:

ao3: 3: etwa die Hälfte

ao4: 4:

ao5: 5: alle

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D2_21

hi:

\------------------------------------------------------------




D2_21
-------

tc:

vn: sszustud (sszustud1; sszustud2; sszustud3; sszustud4; sszustud5; sszustud6; sszustud7; sszustud8; sszustud9; sszustud10; sszustud11)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie im ++aktuellen++ Semester mit den folgenden Aspekten Ihres Studiums?

is:

it1: (sszustud1): fachliche Kompetenz der Lehrenden

it2: (sszustud2): digitale Kompetenz der Lehrenden

it3: (sszustud3): Vermittlung des Lehrstoffs durch die Lehrenden

it4: (sszustud4): Betreuung und Beratung durch die Lehrenden

it5: (sszustud5): Klima/Atmosphäre im Studiengang

it6: (sszustud6): Verfügbarkeit von Fachliteratur

it7: (sszustud7): Service- und Beratungsleistungen

it8: (sszustud8): Ihren Studienleistungen

it9: (sszustud9): Ihrem Studienfortschritt

it10: (sszustud10): Ihrem bisher erreichten Wissen und Können

st:

ao1: 1: überhaupt nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr zufrieden

mv: -12: kann ich nicht beurteilen

ka1: (it1 TO it4): !!Lehre!!

ka2: (it5 TO it8): !!Studiengang!!

ka3: (it9 TO it11): !!Leistungen!!

vc:

av:

kh:

fv:

hv:

fo1: Bitte über it1 "Lehre" linksbündig positionieren.

fo2: Bitte über it5 "Studiengang" linksbündig positionieren.

fo3: Bitte über it9 "Leistungen" linksbündig positionieren.

fo4: mv/"kann ich nicht beurteilen" bitte etwas absetzen.

tr:
       GOTO CO_5

hi:

\--------------------------------

CO_5
-------

tc:

vn: VCO_5_ (VCO_5_a; VCO_5_b; VCO_5_c; VCO_5_d; VCO_5_e; VCO_5_f;  VCO_5_g; VCO_5_h)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und wie zufrieden sind Sie im aktuellen Semester mit …

is: 
	

it1: (VCO_5_a): … dem Angebot an digitalen Lehrveranstaltungen?

it2: (VCO_5_b): … der Umsetzung Ihrer digitalen Lehrveranstaltungen?

it3: (VCO_5_c): … der Erreichbarkeit der Lehrenden (z. B. Feedback zu Aufgaben)?

it4: (VCO_5_d): … der Ansprechbarkeit der Verwaltung?

it5: (VCO_5_e): … der Informationspolitik zum Lehrbetrieb?

it6: (VCO_5_f): … der Kommunikation der Prüfungsmodalitäten?

it7: (VCO_5_g): … Vorbereitung auf die Prüfungen?

it8: (VCO_5_h): … mit der Umsetzung digitaler Prüfungen?
st:

ao1: 1: gar nicht zufrieden

ao2: 2:

ao3: 3: 

ao4: 4:

ao5: 5: voll und ganz zufrieden

mv:

ka: 

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_6

hi: 

**------------------------------------------------------------**

CO_6
-------

tc:

vn: VCO_6_ (VCO_6_a; VCO_6_b)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie beurteilen Sie die Reaktion Ihrer Hochschule auf die Corona-Pandemie? Die getroffenen Maßnahmen sind …
is: 


it1: (VCO_6_a): … angemessen.

it2: (VCO_6_b): … schnell umgesetzt worden.

st:

ao1: 1: stimme gar nicht zu

ao2: 2:

ao3: 3: 

ao4: 4:

ao5: 5: stimme voll und ganz zu
mv:

ka: 

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_23

hi: 

**------------------------------------------------------------**


A_23
=========

tc:

vn: sfach12; sfach22

qt: offene Angaben

hl:

in:

q: Bitte geben Sie Ihr Studienfach an.

is: Bitte geben Sie nicht Ihren angestrebten Abschluss an (z. B. Masterstudent\*in, Promotionsstudent\*in).

it:

st:

ao1 (sfach12): Präfix: erstes Studienfach: [offene Angabe; 60 Zeichen]

ao2 (sfach22): Präfix: ggf. zweites Studienfach: [offene Angabe; 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_24

hi:

\------------------------------------------------------------

A_24
=========

tc:

vn: sabslaja

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Sind Sie in einem Lehramtsstudiengang eingeschrieben?

is:

it:

st:

ao1: 1: nein

ao2: 2: Lehramt an Grundschulen (Primarstufe)

ao3: 3: Lehramt an Haupt-, Real- und Sekundar-/Mittelschulen (Sekundarstufe I)

ao4: 4: Lehramt an Gymnasien und Gesamtschulen (Sekundarstufe II)

ao5: 5: Lehramt an beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: Lehramt an Förderschulen/Sonderpädagogik

mv:

ka: (ao2 TO ao6): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: 

tr: GOTO A_25

hi:

\------------------------------------------------------------

A_25
=========

tc:

vn: sabsan; sabsanoaa; sabsanoka

qt: Einfachauswahl mit vertikalen ao und offenen Angaben

hl:

in:

q: Und welchen Abschluss streben Sie als nächstes an?

is: Sollten Sie mehrere Abschlüsse anstreben, beziehen Sie sich bitte auf den zeitlich nächsten.

it:

st:

ao1: (sabsan): 1: Bachelor

ao2: (sabsan): 2: Master

ao3: (sabsan): 3: Staatsexamen

ao4: (sabsan): 4: Diplom

ao5: (sabsan): 5: Promotion

ao6: (sabsan): 6: kirchliche Abschlussprüfung

ao7: (sabsan): 7: künstlerische Abschlussprüfung

ao8: (sabsan): 8: Anderen Abschluss (bspw. ausländischer Abschluss, Magister), und zwar: [(sabsanoaa), offene Angabe, 80 Zeichen]

ao9: (sabsan): 9: Keinen Studienabschluss, sondern: [(sabsanoka), offene Angabe, 80 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A_27
	
hi:


\------------------------------------------------------------

A_27
=========

tc:
	
vn: sform (sformpraes; sformfern; sformdua; sformberu; sformgast; sformsons; sformsonso)


qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Abgesehen von der besonderen Studiensituation durch die Corona-Pandemie: Um welche Form handelt es sich bei Ihrem Studium?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (sformpraes): Präsenzstudium (im Gegensatz zu Fernstudium)
ao2: (sformfern): Fernstudium
ao3: (sformdua): duales Studium
ao4: (sformberu): berufsbegleitendes Studium
ao5: (sformgast): Gasthörerschaft
ao6: (sformsons): Anderes, und zwar: [(sformsonso), offene Angabe, 60 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_28

hi:

\--------------------------------

A_28
=========

tc:

vn: spernot; spernoto

qt: offene Angabe, Einfachauswahl

hl:

in:

q: Mit welcher Note wurden Ihre bisherigen Studienleistungen im ++letzten Semester++ bewertet?

is: Punktzahl bitte in Note umrechnen.

it:

st:

ao1: (spernot): Präfix: Durchschnittsnote im letzten Semester (z.B. 2,5): [(spernoto): Number, 3-stellig: 1,0 TO 5,0]

ao2: (spernot): -11: Ich habe bisher keine Noten erhalten.

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihre aktuelle Durchschnittsnote an (1,0 bis 5,0)

fv:

hv:

fo: 

tr: (siehe unten)

hi: 

\------------------------------------------------------------

A_28
=========

tc:

vn: spernot2; spernoto2

qt: offene Angabe, Einfachauswahl

hl:

in:

q: Und wie wurden Ihre bisherigen Studienleistungen bislang ++insgesamt++ bewertet?

is: 

it:

st:

ao1: (spernot2): Präfix: Durchschnittsnote insgesamt (z.B. 2,5): [(spernoto2): Number, 3-stellig: 1,0 TO 5,0]

ao2: (spernot2): -11: Ich habe bisher keine Noten erhalten.

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihre aktuelle Durchschnittsnote an (1,0 bis 5,0)

fv:

hv:

fo1: Bitte offene Angabe und Einfachauswahl untereinander, linksbündig positionieren

fo2: Bitte diese Frage zusammen mit der vorherigen Frage auf einer Seite (A_28) darstellen. 

tr:  GOTO D2_5

hi: 

\------------------------------------------------------------


D2_5
-------

tc:

vn: lsanwesend; dsanwesend

qt: Comparison

hl:

in:

q: Wenn Sie an die von Ihnen belegten Veranstaltungen denken: Wie hoch ist der Anteil der Sitzungen, an denen Sie im Schnitt auch tatsächlich teilnehmen?
is:

it1: (lsanwesend) im letzten Semester

it2: (dsanwesend) in diesem Semester

st:

ao1: 1: 0 bis 10 %

ao2: 2: 11 bis 20 %

ao3: 3: 21 bis 30 %

ao4: 4: 31 bis 40 %

ao5: 5: 41 bis 50 %

ao6: 6: 51 bis 60 %

ao7: 7: 61 bis 70 %

ao8: 8: 71 bis 80 %

ao9: 9: 81 bis 90 %

ao10: 10: 91 bis 100 %

mv: -11: trifft nicht zu

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr: GOTO D2_18

hi: 

\------------------------------------------------------------


D2_18
-------

tc:

vn: sswrite (sswrite1; sswrite2; sswrite3; sswrite4; sswrite5; sswrite6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie viele Zusammenfassungen, Exzerpte, Hausarbeiten und andere schriftliche Leistungen müssen Sie in diesem Semester erbringen?	

is: Bitte geben Sie die ++Anzahl++ der schriftlichen Leistungen (inklusive der noch nicht abgeschlossenen) entsprechend ihrer Länge an.

it1: (sswrite1): bis zu 5 Seiten

it2: (sswrite2): 6 bis 10 Seiten

it3: (sswrite3): 11 bis 15 Seiten

it4: (sswrite4): 16 bis 20 Seiten

it5: (sswrite5): 21 bis 25 Seiten

it6: (sswrite6): 26 Seiten oder mehr

st:

ao1: 0: 0

ao2: 1: 1

ao3: 2: 2

ao4: 3: 3

ao5: 4: 4

ao6: 5: 5

ao7: 6: 6

ao8: 7: 7

ao9: 8: 8

ao10: 9: 9

ao11: 10: ≥10

mv:

ka: Anzahl der verfassten Texte

vc:

av:

kh:

fv:

hv:

fo: 

tr: GOTO D2_19

hi: 

\------------------------------------------------------------
D2_19
-------

tc:

vn: ssread; ssread2

qt: offene Angabe

hl:

in:

q: Wie viele Seiten lesen Sie pro Woche, um sich auf die von Ihnen besuchten Lehrveranstaltungen vorzubereiten?

is:.

it:

st:

ao1: (ssread): Präfix: in diesem Semester [number, 3-stellig: 0 TO 999], Postfix: Seiten pro Woche 

ao2: (ssread2): Präfix: im letzten Semester [number, 3-stellig: 0 TO 999], Postfix: Seiten pro Woche 

mv:

ka:

vc:

av:

kh: Bitte geben Sie die Anzahl gelesener Seiten pro Woche an (0 bis 999).

fv:

hv:

fo:

tr:

        GOTO CO_18

hi:

\------------------------------------------------------------

CO_18
-------

tc:

vn: VCO_18_ (VCO_18_a; VCO_18_b; VCO_18_c; VCO_18_d; VCO_18_e; VCO_18_f; VCO_18_g; VCO_18_h; VCO_18_i; VCO_18_j)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwiefern haben sich die folgenden Aspekte durch die Corona-Pandemie für Sie verändert?

is: 
	

it1: (VCO_18_a): Veranstaltungsinhalten folgen

it2: (VCO_18_b): die Menge an Lernstoff bewältigen

it3: (VCO_18_c): … Lernstrategien entwickeln

it4: (VCO_18_d): Literaturbeschaffung

it5: (VCO_18_e): Prüfungsanforderungen bewältigen
	
it6: (VCO_18_f): Kontakte zu Mitstudierenden knüpfen
	
it7: (VCO_18_g): Kommunikation mit Lehrenden

it8: (VCO_18_h): Austausch in Lerngruppen

it9: (VCO_18_i): Beziehungen im familiären Umfeld

it10: (VCO_18_j): Tagesstrukturierung

st:

ao1: 1: schwieriger geworden

ao2: 2:

ao3: 3: gleich geblieben

ao4: 4:

ao5: 5: einfacher geworden

mv:

ka: 

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_51b

hi: 

**------------------------------------------------------------**



A_51b
=========

tc:

vn: ssa (ssahswe; ssafawe; ssaunt; ssaaja)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwieweit denken Sie zurzeit daran …

is:

it1: (ssahswe): … die Hochschule zu wechseln?

it2: (ssafawe): … Ihr Studienfach zu wechseln?

it3: (ssaunt): … Ihr aktuelles Studium zu unterbrechen?

it4: (ssaaja): … das Studium ganz aufzugeben?

st:

ao1: 1: gar nicht

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

GOTO D2_11

hi:

\------------------------------------------------------------

D2_11
-------

tc:

vn: sscokli (sscokli1; sscokli2; sscokli3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit stimmen die folgenden Aussagen mit dem überein, was Sie in Ihrem Studiengang typischerweise erleben?

is:

It1: (sscokli1): Die Lehrenden gehen auf Schwierigkeiten der Studierenden ein.

it2: (sscokli2): Im Allgemeinen unterstützen sich die Studierenden gegenseitig.

it3: (sscokli3): Die Lehrenden vermitteln den Studierenden Freude am Fach.

st:

ao1: 1: stimmt gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: stimmt genau

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:  GOTO D2_13

hi: 

\------------------------------------------------------------

D2_13
-------

tc:

vn: sskonth (sskonth1; sskonth2; sskonth3; sskonth4; sskonth5; sskonth6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig haben Sie im aktuellen Semester außerhalb der Lehrveranstaltungen zu den folgenden Personen Kontakt?

is: Gemeint sind Kontakte jeglicher Art (persönlich, telefonisch, schriftlich, digital).

it1: (sskonth1): Kommiliton\*innen

it2: (sskonth2): Studierenden anderer Fächer

it3: (sskonth3): Freund\*innen und Bekannten außerhalb der Hochschule

it4: (sskonth4): Lehrenden

it5: (sskonth5): Mitarbeiter\*innen der Hochschulverwaltung

it6: (sskonth6): Familie (Eltern, Geschwistern u. a.)

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

        GOTO CO_7

hi: 

**------------------------------------------------------------**

CO_7
-------

tc:

vn: VCO_7_ (VCO_7_a; VCO_7_b; VCO_7_c; VCO_7_d; VCO_7_e; VCO_7_f)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Haben Sie im Vergleich zum vorangegangenen Semester mehr oder weniger Kontakt zu folgenden Personen?

is: Gemeint sind Kontakte jeglicher Art (persönlich, telefonisch, schriftlich, digital).

it1: (VCO_7_a): Kommiliton\*innen

it2: (VCO_7_b): Studierenden anderer Fächer

it3: (VCO_7_c): Freund\*innen und Bekannten außerhalb der Hochschule

it4: (VCO_7_d): Lehrenden

it5: (VCO_7_e): Mitarbeiter\*innen der Hochschulverwaltung

it6: (VCO_7_f): Familie (Eltern, Geschwistern u. a.)

st:

ao1: 1: viel weniger

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: viel mehr

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

        GOTO N_9

hi: 

**------------------------------------------------------------**


N_9
=========

tc:

vn: digorg (digorg1; digorg2; digorg3; digorg4; digorg5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wenn Sie an die Zeit vor der Corona-Pandemie denken: In wie vielen Ihrer Lehrveranstaltungen wurden die folgenden Bestandteile über digitale Plattformen (z. B. StudIP, Moodle, Ilias, Olat) organisiert?

is:

it1: (digorg1): An-/Abmeldung zu Lehrveranstaltungen

it2: (digorg2): An-/Abmeldung zu Prüfungen, Ergebniseinsicht

it3: (digorg3): Kommunikation innerhalb der Lehrveranstaltungen

it4: (digorg4): Bereitstellung von Literatur und Lehrmaterialien

it5: (digorg5): Erbringung von Leistungsnachweisen/elektronische Prüfungen

st:

ao1: 1: keine

ao2: 2:

ao3: 3: etwa die Hälfte

ao4: 4:

ao5: 5: alle 

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

        GOTO N_10a

hi: 

\------------------------------------------------------------

N_10a
=========

tc:

vn: diggeso (diggeso1; diggeso2; diggeso3; diggeso4; diggeso5)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Und wie häufig wurden in den vorangegangenen Semestern die folgenden Geräte bzw. Software in die Lehre eingebunden?

is:

it1: (diggeso1): Laptop und Beamer der Hochschule

it2: (diggeso2): Smart-Board

it3: (diggeso3): eigener Laptop, Tablet, Smartphone

it4: (diggeso4): Präsentationssoftware (PowerPoint, Prezi)

it5: (diggeso5): fachspezifische Software

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

GOTO N_10b

hi:

\------------------------------------------------------------

N_10b
=========

tc:

vn: digflehr (digflehr1; digflehr2; digflehr3; digflehr4; digflehr5; digflehr6)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Abgesehen von den Lehrveranstaltungen Ihrer Hochschule, wie häufig nutzen Sie die folgenden Formen des digitalen Lernens?

is:

it1: (digflehr1): … in diesem Semester

it2: (digflehr2): … im letzten Semester

it3: (digflehr3): … in diesem Semester

it4: (digflehr4): … im letzten Semester

it5: (digflehr5): … in diesem Semester

it6: (digflehr6): … im letzten Semester


st:

ao1: 1: nie

ao2: 2:

ao3: 3: 

ao4: 4:

ao5: 5: sehr häufig

mv:

ka1: (it1 TO it2): !! im Internet zugängliche Lehr- und Lernmaterialien!!

ka2: (it3 TO it4): !! Lehr- und Lernvideos!!

ka3: (it5 TO it6): !! digitale Selbstlernprogramme (z. B. Simulation, Lernapps, Lernspiele)!!

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_22

hi:

\------------------------------------------------------------


A_22
=========

tc:

vn: sperleiszufr

qt: Einfachauswahl mit Horizontalen ao

hl:

in:

q: Alles in allem: Wie zufrieden sind Sie insgesamt mit den Bedingungen an Ihrer Hochschule?

is:

it:

st:

ao1: 1: sehr unzufrieden

ao2: 2

ao3: 3

ao4: 4

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

GOTO A_41
    
hi:

\------------------------------------------------------------

A_41
===========

tc:

vn: vausbja

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor dem Studium eine Berufsausbildung begonnen bzw. abgeschlossen?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, begonnen und nicht abgeschlossen

ao3: 3: ja, begonnen und abgeschlossen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: 


tr:

GOTO A_1

hi:

\------------------------------------------------------------

A_1
=========

tc:

vn: vsbdeba

qt: Einfachauswahl mit vertikalen ao

hl:

in: 

q: Wo haben Sie erstmals Ihre Hochschulreife erworben?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

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

\------------------------------------------------------------

A_1
=========

tc:

vn: dnatdeu; dnatausl

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Und: Welche Staatsangehörigkeit haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (dnatdeu): deutsche Staatsangehörigkeit

ao2: (dnatausl): andere Staatsangehörigkeit(en)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

    GOTO A_38

hi:


\------------------------------------------------------------

A_38
==========

tc:

vn: vsbart

qt: Einfachauswahl

hl:

in:

q: In Deutschland führen verschiedene Wege ins Studium: Welchen höchsten Schulabschluss hatten Sie vor Beginn des Studiums erworben?
is:

it:

st:

ao1: 1: allgemeine Hochschulreife

ao2: 2: fachgebundene Hochschulreife

ao3: 3: Fachhochschulreife

ao4: 4: Mittlere Reife

ao5: 5: Hauptschulabschluss

ao6: 6: anderer Abschluss

a07: 7: keinen Abschluss

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_5

hi:

\------------------------------------------------------------


A_5
====

tc:

vn: dgebort

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wo wurden Sie geboren?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_34

hi:

\------------------------------------------------------------


A_34
=========

tc:

vn: deltgebv; deltgebm

qt: Einfachauswahl mit vertikalen ao im Spaltenformat/Comparison

hl:

in:

q: Wo wurden Ihre Eltern geboren?

is:

it1 (deltgebv): Vater

it2 (deltgebm): Mutter

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_32
    
hi:

\------------------------------------------------------------


A_32
=========

tc:

vn: deltberuv; deltberum

qt: Einfachauswahl mit vertikalen ao im Spaltenformat/Comparison

hl:

in:

q: Welches ist der höchste berufliche Abschluss Ihres Vaters/Ihrer Mutter?

is:

it1: (deltberuv): Vater

it2: (deltberum): Mutter

st:

ao1: 7: Promotion (Doktortitel)

ao2: 6: Universitätsabschluss

ao3: 5: Fachhochschulabschluss

ao4: 4: Abschluss an einer Meister-, Techniker-, Fachschule

ao5: 3: Lehre bzw. Facharbeiterabschluss, Abschluss an einer Berufsfach-, Handels-, Berufsaufbauschule

ao6: 2: anderer beruflicher Abschluss

ao7: 1: hat keinen beruflichen Abschluss

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_9b

hi:

\------------------------------------------------------------


A_9b
=========

tc:

vn: demosex; demosexo

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Welches Geschlecht haben Sie?

is:

it:

st:

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: divers

ao4: 4: Keine der genannten Kategorien, sondern: [(demosexo); 50 Zeichen] (offene Angabe)

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_10

hi:

\------------------------------------------------------------


A_10
=========

tc:

vn: demoage

qt: offene Angabe

hl:

in:

q: Wie alt sind Sie?

is:

it:

st:

ao: (demoage) [offene Angabe; Number, 2-stellig: 15 TO 99], Postfix: Jahre 

mv:

ka:

vc:

av: 

kh: Bitte geben Sie Ihr Lebensalter an (15 bis 99).

fv:

hv:

fo:

tr:

GOTO A_12a

hi: 

\------------------------------------------------------------

A_12a
=========

tc:

vn: dsib; dsibo

qt: Einfachauswahl mit vertikalen ao und offener Angabe

hl:

in:

q: Haben Sie Geschwister?

is: Bitte geben Sie auch Ihre Halb- und Stiefgeschwister an.

it:

st:

ao1: (dsib): 1: nein

ao2: (dsib): 2: Ja, und zwar: ([dsibo], NUMBER, 2-Steller)

mv:

ka:

vc:

av:

kh: ao2: Bitte geben Sie die Anzahl der Personen an.

fv:

hv:

fo:

tr:

GOTO A_11
    
hi:


\------------------------------------------------------------

A_11
=========

tc:

vn: demofam (demofamsin; demofampar; demofamehe; demofamaus; demofamtod; demofamka)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Welchen Familienstand haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (demofamsin): ohne feste*n Partner*in

ao2: (demofampar): mit einer/einem festen Partner*in

ao3: (demofamehe): verheiratet/eingetragene Lebenspartnerschaft

ao4: (demofamaus): geschieden
	
ao5: (demofamtod): verwitwet

ao6: (demofamka): keine Angabe [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_12

hi:

\------------------------------------------------------------

A_12
=========

tc:

vn: dkinja

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Haben Sie Kinder?

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

GOTO C1_1 IF dkinja == 2
GOTO CO_21

hi:

\------------------------------------------------------------


C1_1
====

tc: 


vn: dkinanz

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wie viele Kinder haben Sie?

is:

it:

st:

ao1: (dkinanz) 1: eins

ao2: (dkinanz) 2: zwei

ao3: (dkinanz) 3: drei

ao4: (dkinanz) 4: vier oder mehr

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO C1_2
        
hi:

\--------------------------------


C1_2
====

tc: 


vn: dkinage (dkinagej / dkinage1 / dkinage2 / dkinage3 / dkinage4 / dkinage5)

qt: offene Angaben mit vertikaler Eingabespalte/-feldern

hl:

in:

q1: Wie alt sind Ihre Kinder?

is: Mit “1. Kind” meinen wir Ihr ältestes Kind.

it1: (dkinagej) [infield = Alter jüngstes Kind]

it2: (dkinage1): [infield = Alter Ihres Kindes]

it3: (dkinage2): [infield = Alter 1. Kind]

it4: (dkinage3): [infield = Alter 2. Kind]

it5: (dkinage4): [infield = Alter 3. Kind]

it6: (dkinage5): [infield = Alter 4. Kind]

st:

ao1: (dkinagej): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao2: (dkinage1): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao3: (dkinage2): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao4: (dkinage3): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao5: (dkinage4): 4-stellig: 0 TO 99, number, Suffix: Jahre

ao6: (dkinage5): 4-stellig: 0 TO 99, number, Suffix: Jahre

mv:

ka:

vc1: SHOW dkinagej IF dkinanz = k. A.

vc2: SHOW dkinage1 IF dkinanz = 1

vc3: SHOW dkinage2 IF dkinanz >= 2

vc4: SHOW dkinage3 IF dkinanz >= 2

vc5: SHOW dkinage4 IF dkinanz >= 3

vc6: SHOW dkinage5 IF dkinanz >= 4

vc7: SHOW is IF dkinanz >= 2

vc8: SHOW q1 IF dkinanz = k. A.

vc9: SHOW q2 IF dkinanz = 1

vc10: SHOW q3 IF dkinanz >= 2

av: 

kh: Bitte geben Sie das Lebensalter Ihres Kindes an (0 bis 99).

fv:

hv:

fo:

tr:

GOTO C1_6

hi: 

\--------------------------------

C1_6
====

tc: 


vn: dkinbe (dkinbesel / dkinbepar / dkinbeelt / dkinbegelt / dkinbefr / dkinbesit / dkinbealo)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q1: In Anbetracht der besonderen Situation durch die Schließung von Kitas, Kindergärten und Schulen: Wie häufig betreuen die folgenden Personen Ihre Kinder im aktuellen Semester?

is:

it1: (dkinbesel): ich selbst

it2: (dkinbepar): Partner*in

it3: (dkinbeelt): anderer Elternteil (falls nicht Partner*in)

it4: (dkinbegelt): Großeltern oder andere Verwandte

it5: (dkinbefr): formale Kinderbetreuung (Sitter*in, Kita, Schule usw.)

it6: (dkinbesit): andere Personen

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

GOTO CO_21

hi:

\--------------------------------

CO_21
====

tc: 

vn: VCO_21

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: hören Sie zur COVID-19-Risikogruppe?

is:

it:

st:

ao1: (VCO_21) 1: nein

ao2: (VCO_21) 2: ja

ao3: (VCO_21) 3: weiß ich nicht

ao4: (VCO_21) 4:  Ich möchte keine Angabe machen.

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_15
        
hi:

\--------------------------------

A_15
=========

tc:

vn: gbeges; gartmob; gartseh; gartohr; gartspr; gartpsy; gartsom; garttls; gartson; gartsono; gartka; h_gartcount

qt: Mehrfachauswahl mit vertikalen ao

hl:

in: Im Folgenden stellen wir Ihnen einige kurze Fragen zu möglichen Beeinträchtigungen. Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu.

q: Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (gbeges): keine [Exklkusivkategorie]

ao2: (gartmob): Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

ao3: (gartseh): Blindheit/Sehbeeinträchtigung

ao4: (gartohr): Gehörlosigkeit/Hörbeeinträchtigung

ao5: (gartspr): Sprechbeeinträchtigung (z. B. Stottern)

ao6: (gartpsy): psychische Erkrankung (z. B. Depression, Essstörung)

ao7: (gartsom): körperlich länger dauernde/chronische Krankheit (z. B. Rheuma, MS, Darmerkrankung)

ao8: (garttls): Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

ao9: (gartson): andere Beeinträchtigung/Erkrankung (z. B. Tumorerkrankung, Autismus-Spektrum-Störung): [(gartsono), 50 Zeichen]

ao10: (gartka): Ich möchte die Form meiner Beeinträchtigung nicht nennen. 

mv: 

ka: (ao2 TO ao10): Ja, und zwar:

vc:

av:

kh:

fv:

hv: Es wird die Hilfsvariable h_gartcount berechnet: als Anzahl aller hier gewählten Antworoptionen ao1-ao9, exklusive ao10.

fo: 

tr:

GOTO C2_0 IF h_gartcount >= 1

GOTO D3_23

hi: 

\------------------------------------------------------------

C2_0
====

tc: 


vn: beschwer

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wirkt sich Ihre Beeinträchtigung erschwerend auf Ihr Studium aus?

is:

it:

st:

ao1: (beschwer) 1: nein

ao2: (beschwer) 2: ja

ao3: (beschwer) 3: Ich möchte keine Angabe machen.

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr: 

GOTO D3_23

hi:


\--------------------------------


D3_23
====

tc:

vn: allges

qt: Einfachauswahl/5er-Skala mit horizontalen ao

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

tr:

GOTO D1_27

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

tc: 


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

tr:

       GOTO B1_2

hi1: Items bitte zufällig rotieren.

\--------------------------------

B1_2
=

tc:

vn: genidsach; genidloes; genidrat; genidlieb; genideinf; genidemo; genidrisk

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wenn Sie sich selbst beschreiben müssten: Welche Eigenschaften treffen am ehesten auf Sie zu?

is:

it1: (genidrat): rational

it2: (genidemo): emotional

it3: (genidrisk): risikobereit

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

GOTO D1_24

hi:

\--------------------------------


D1_24 
===

tc:

vn: pbig (pbigintro / pbigextro / pbigtrau / pbigkrit / pbiggenau / pbigfaul / pbigruh / pbignerv / pbigkrea / pbignoku)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Und inwieweit treffen die folgenden Aussagen auf Sie zu?

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

GOTO D1_25

hi: 

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

GOTO CO_19

hi: 

**------------------------------------------------------------**

CO_19

==========

tc:

vn: VCO_19

qt: Einfachauswahl

hl:

in:

q: Hatten Sie in diesem Semester ein studienbezogenes Praktikum geplant?

is: 

it:

st:

ao1: 1: Nein

ao2: 2: … wie geplant durchgeführt.

ao3: 3: … aber verschoben.

ao4: 4: … aber abgesagt.

mv:

ka: (ao2 to ao4): Ja, wurde…

vc: 

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_42

hi:

\------------------------------------------------------------


A_42 
==========

tc:

vn: eaktsens

qt: Einfachauswahl

hl:

in:

q: Waren Sie unmittelbar vor der Corona-Pandemie erwerbstätig?

is: 

it:

st:

ao1: 1: nein

ao2: 2: ja, mit einer Tätigkeit

ao3: 3: ja, mit zwei verschiedenen Tätigkeiten

ao4: 4: ja, mit drei oder mehreren Tätigkeiten

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr:

GOTO D3_19

hi:

\------------------------------------------------------------


D3_19
=====

tc:

vn: etat1; fachn1 

qt: Tableau/Einfachauswahl

hl:

in: 

q:  Bitte geben Sie die Art der Erwerbstätigkeit und deren inhaltliche Nähe zu den Studieninhalten an.

is: Beziehen Sie sich dabei bitte auf Ihre Haupttätigkeit.


it1: (etat1): !!Haupttätigkeit!!

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

st:

mv: 

vc: 

av: 

kh: 

fv: 

hv: 

fo: 

tr:

GOTO CO_8

hi: 



\--------------------------------

CO_8
=========

tc:

vn: VCO_8; VCO_8o

qt: Einfachauswahl mit vertikalen ao und offenen Angaben

hl:

in:

q: Sie haben angegeben, unmittelbar vor der Corona-Pandemie erwerbstätig gewesen zu sein: In welcher Berufsbranche lag diese Beschäftigung?

is: Bitte beziehen Sie sich auf Ihre Haupttätigkeit.


it:

st:

ao1: (VCO_8): 1: Land- und Forstwirtschaft/Fischerei

ao2: (VCO_8): 2: Energie- und Wasserversorgung, Bergbau

ao3: (VCO_8): 3: Verarbeitendes Gewerbe (Industrie u. Handwerk o. Bau) 

ao4: (VCO_8): 4: Bauwirtschaft

ao5: (VCO_8): 5: Handel (Groß- und Einzelhandel) 

ao6: (VCO_8): 6: Verkehr und Nachrichtenübermittlung 

ao7: (VCO_8): 7: Banken, Sparkassen 

ao8: (VCO_8): 8: Versicherungen (außer gesetzliche Sozialversicherung)

ao9: (VCO_8): 9: Gaststätten und Hotelgewerbe 

ao10: (VCO_8): 10: Reinigung 

ao11: (VCO_8): 11: Bildungseinrichtungen, Verlage 

ao12: (VCO_8): 12: Gesundheitswesen

ao13: (VCO_8): 13: andere Dienstleistungen 

ao14: (VCO_8): 14: Organisationen ohne Erwerbszweck (Verbände, Gewerkschaften, Kirchen), private Haushalte 

ao15: (VCO_8): 15: Gebietskörperschaften (allgemeine öffentliche Verwaltung: Bund, Länder, Gemeinden) und gesetzliche Sozialversicherung 

ao16: (VCO_8): 16: Anderer Status, und zwar: [(VCO_8o), offene Angabe, 80 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

       GOTO CO_9
	
hi:


\------------------------------------------------------------

CO_9
=========

tc:
	
vn: VCO_9_ (VCO_9_a; VCO_9_b; VCO_9_c; VCO_9_d; VCO_9_e; VCO_9_f; VCO_9_g)


qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Hat sich die Corona-Pandemie auf Ihre Erwerbstätigkeit ausgewirkt?

is: Bitte beziehen Sie sich auf Ihre Haupttätigkeit und wählen Sie alles Zutreffende aus.

it:

st:

ao1: (VCO_9_a): Ja, ich wurde entlassen.

ao2: (VCO_9_b): Ja, ich wurde unbezahlt freigestellt.

ao3: (VCO_9_c): Ja, ich wurde bezahlt freigestellt.

ao4: (VCO_9_d): Ja, meine Arbeitszeit wurde reduziert.

ao5: (VCO_9_e): Ja, meine Arbeitszeit wurde erhöht. 

ao6: (VCO_9_f): Ja, ich musste von Zuhause aus arbeiten.

ao7: (VCO_9_g): Ja, ich habe gekündigt.

ao8: (VCO_9_h): Ja, ich habe eine neue Erwerbstätigkeit aufgenommen.

ao9: (VCO_9_i): Nein, nichts davon

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO CO_9a

hi:

\--------------------------------

CO_9a
=====

tc:

vn: VCO_9a

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist Ihre neue Erwerbstätigkeit systemrelevant?

is: Gemeint sind Erwerbstätigkeiten, die zur Bekämpfung der Corona-Pandemie und deren Folgen beitragen.

it:

st:

ao1: 1: ja

ao2: 2: nein

ao3: 3: weiß ich nicht

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO CO_24

hi:


\--------------------------------

CO_24
=====

tc:

vn: VCO_24

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Hat sich die Corona-Pandemie auf die Einkommenssituation Ihrer Eltern ausgewirkt?

is:

it:

st:

ao1: 1: … deutlich verschlechtert.

ao2: 2: … nicht verändert.

ao3: 3: … deutlich verbessert.

mv:

ka: Die Einkommenssituation hat sich…

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D3_13

hi:


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

tr:

GOTO D3_6

hi:


\--------------------------------


D3_6
====

tc:

vn: fein (feininsg1 / feininsg2 / feinelto1 / feinelto2 / feinjobo1 / feinjobo2 / feinbafo1 / feinbafo2 / feinkredo1 / feinkredo2 / feinandq1 / feinandq2 )

qt: offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich ++pro Monat++ zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst verfügen. ++Nicht++ gemeint sind Beträge, die z. B. von Ihren Eltern für Sie direkt an Dritte überwiesen werden (z. B. Überweisung der Miete durch Ihre Eltern).

ita: im letzten Semester

itb: in diesem Semester

st:

ao1a: (feininsg1): Gesamteinnahmen [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao1b: (feininsg2): Gesamteinnahmen [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao2a: (feinelto1): Eltern und Verwandte [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao2b: (feinelto2): Eltern und Verwandte [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3a: (feinjobo1): Erwerbstätigkeit [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao3b: (feinjobo2): Erwerbstätigkeit [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4a: (feinbafo1): BAföG [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao4b: (feinbafo2): BAföG [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5a: (feinkredo1): Kredit(e) [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao5b: (feinkredo2): Kredit(e) [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6a: (feinandq1): Weitere Finanzierungsquelle(n) [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

ao6b: (feinandq1): Weitere Finanzierungsquelle(n) [infield = € pro Monat; number, 4-stellig: 0 TO 9999]

mv:

ka: (ao2 TO ao6): **++davon entfallen auf…++**

vc: 

av: 

kh1: ao1: Bitte geben Sie Ihre monatlichen Gesamteinnahmen an (0 bis 99999).

kh2: ao2 TO ao6: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (0 bis 9999).

fv:

hv:

fo: 

tr:

GOTO CO_20

hi: 

\--------------------------------

























CO_20
=========

tc:

vn: VCO_20_ (VCO_20_a; VCO_20_b; VCO_20_c; VCO_20_d; VCO_20_e; VCO_20_f; VCO_20_g VCO_20_h; VCO_20_i; VCO_20_j, VCO_20_k, VCO_20_ko)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Auf welche Finanzierungsquellen greifen Sie zurück, um mögliche finanzielle Engpässe aufgrund der Corona-Pandemie auszugleichen?

is:

it1: (VCO_20_a): Familie/Verwandte/Partner*in
	
it2: (VCO_20_b): Erwerbstätigkeit

it3: (VCO_20_c): eigene Ersparnisse

it4: (VCO_20_d): BAföG-Aktualisierung

it5: (VCO_20_e): KfW-Studienkredit

it6: (VCO_20_f): privater Kredit

it7: (VCO_20_g): Überbrückungshilfe in pandemiebedingten Notlagen

it8: (VCO_20_h): Nothilfefond Ihrer Hochschule

it9: (VCO_20_i): Nothilfefond des Studierendenwerks

it10: (VCO_20_j): Darlehenskasse des Studierendenwerks

it10: (VCO_20_k): Andere Finanzierungsquelle(n), und zwar [(VCO_20_ko), offene Angabe]

st:

ao1: 1:  Nein

ao2: 2: geplant

ao3: 3: beantragt/ erbeten

ao4: 4: wird bereits genutzt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_22 IF VCO_20_e= 3 OR VCO_20_e= 4

GOTO CO_23 IF VCO_20g == 3 or VCO_20g == 4 or VCO_20h == 3 or VCO_20h == 4 or VCO_20_i == 3 or VCO_20_i == 4

GOTO D3_8

hi:

\--------------------------------


CO_22
====

tc:

vn: VCO_22

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wann haben Sie den KfW-Studienkredit beantragt?

is:

it:

st:

ao1: 1: vor dem 8. Mai 2020

ao2: 2:  nach dem 8. Mai 2020

mv:

ka:

vc: 

av: 

kh:

fv:

hv:

fo:

tr:

GOTO CO_23 IF VCO_20g == 3 or VCO_20g == 4 or VCO_20h == 3 or VCO_20h == 4 or VCO_20_i == 3 or VCO_20_i == 4

GOTO D3_8

hi: 

\--------------------------------

CO_23
====

tc:

vn: VCO_23

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wann haben Sie die Überbrückungshilfe bzw. den Nothilfefond beantragt?

is:

it:

st:

ao1: 1: vor dem 1. Juni 2020

ao2: 2:  nach dem 1. Juni 2020

mv:

ka:

vc: 

av: 

kh:

fv:

hv:

fo:

tr:

GOTO D3_8

hi: 

\--------------------------------


D3_8
====

tc:

vn: VD3_8

qt: offene Angabe

hl:

in:

q: Bitte geben Sie Ihre durchschnittlichen ++monatlichen++ Gesamtausgaben an.


is: 

it: 

st:

ao1: (VD3_8): [infield = € pro Monat; number, 5-stellig: 0 TO 99999]

mv:

ka:

vc: 

av: 

kh:  Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 99999).

fv:

hv:

fo: 

tr: GOTO D3_9

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

ao1: (fmineinko): [number, 5-stellig: 1 TO 99999], Postfix: € 

mv:

ka:

vc:

av: 

kh: (fmineinko): Bitte geben Sie Ihre benötigten monatlichen Mindesteinnahmen an (1 bis 99999).

fv:

hv:

fo:

tr:

GOTO D3_11

hi:

\--------------------------------

D3_11
=====

tc:

vn: fsitzum (fsitzum1, fsitzum2, fsitzum3, fsitzum4, fsitzum5)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie und Ihre finanzielle Situation zu?

is:

it1: (fsitzum1): Die Finanzierung meines Lebensunterhalts während des Studiums ist sichergestellt.

it2: (fsitzum2): Ich habe zurzeit finanzielle Schwierigkeiten.

it3: (fsitzum3): Im Großen und Ganzen gelingt es mir, mit meinem Geld auszukommen.

it4: (fsitzum4): Aufgrund der Corona-Pandemie kann ich mein Studium ohne zusätzliche finanzielle Unterstützung nicht fortführen.

it4: (fsitzum5): Meine Eltern sind nur eingeschränkt in der Lage mich finanziell zu unterstützen.

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

GOTO B2_7

hi: 

\--------------------------------


B2_7
=====

tc:

vn: skeuro / skwiss / skjobs / skantr / skkarr

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie wahrscheinlich ist es, dass jemand aus Ihrem persönlichen Umfeld …

is:

it1: (skeuro) … Ihnen spontan 1000 € leihen würde?

it2: (skwiss) … Ihre wissenschaftlichen Arbeiten gegenliest?

it3: (skjobs) … Ihnen einen Job oder ein Praktikum vermittelt?

it4: (skantr) … Ihnen beim Ausfüllen von amtlichen Anträgen (z. B. BAföG, Steuererklärung) helfen würde?

it5: (skkarr) … Ihnen hilfreiche Ratschläge für den weiteren Berufs- und Karriereweg gibt?

st:

ao1: 1: sehr unwahrscheinlich

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO A_56
    
hi:

\--------------------------


A_56
=========

tc:

vn: zlv (zlvwo, zlvwo2); zses (zseswo, zseswo2); zer (zerwo, zerwo2); zcar (zcarwo, zcarwo2) zchi (zchiwo, zchiwo2)

qt: Comparison, offene Angaben-Matrix

hl:

in:

q: Wie viele Stunden wenden Sie in einer für Sie typischen Woche für folgende Aktivitäten auf?

is: Bitte runden Sie Ihre Zeitangaben jeweils auf volle Zeitstunden.

ita: in diesem Semester

itb: in letzten Semester

st:

ao1a: (zlvwo): Lehrveranstaltungen [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao1b: (zlvwo2): Lehrveranstaltungen [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao2a: (zseswo): Selbststudium [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao2b: (zseswo2): Selbststudium [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao3a: (zerwo): Erwerbstätigkeit [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao3b: (zerwo2): Erwerbstätigkeit [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao4a: (zcarwo): Pflege- und Betreuungsarbeiten [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao4b: (zcarwo2): Pflege- und Betreuungsarbeiten [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao5a: (zchiwo): Kinderbetreuung [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

ao5b: (zchiwo2): Kinderbetreuung [offene Angabe, NUMBER, 2-stellig (0 bis 99)]

mv:

ka:

vc: 

av: NUMBER, 2-stellig (0 bis 99)

kh: Bitte geben Sie volle Zeitstunden an (0 bis 99).

fv:

hv:

fo: 

tr:

GOTO A_53

hi: 


\------------------------------------------------------------


A_53
=========

tc:

vn: wohn (wohnal1; wohnwg1; wohnel1; wohnpar1; wohnkin1; wohnfam1; wohnsons1; wohnal2; wohnwg2; wohnel2; wohnpar2; wohnkin2; wohnfam2; wohnsons2)

qt: Mehrfachauswahlmatrix mit Exklusivkategorie

hl:

in:

q1: Wie wohnen Sie während der Vorlesungszeit überwiegend?

is: Bitte alles Zutreffende auswählen.

it:

st:

it1: (wohnal1; wohnal2): ... alleine. [Exklusivkategorie]

it2: (wohnwg1; wohnwg2): … in einer Wohngemeinschaft.

it3: (VA_51_1; VA_51_2): … in einem Studierendenwohnheim

it4: (wohnel1; wohnel2): … bei/mit meinen Eltern (bzw. Elternteil).

it5: (wohnpar1; wohnpar2): ... mit meinem/meiner (Ehe-) Partner*in.

it6: (wohnkin1; wohnkin2): ... mit meinem Kind/meinen Kindern.

it7: (wohnfam1; wohnfam2): ... mit anderen Familienangehörigen.

it8: (wohnsons1; wohnsons2): ... mit anderen Personen.

st:

ao1: in diesem Semester

ao2: im letzten Semester

mv:

ka: Ich wohne …

vc:

av:

kh:

fv:

hv:

fo: 

tr:

GOTO D3_2
  
hi:

\------------------------------------------------------------

D3_2
====

tc:

vn: wohnamio

qt: offene Angaben

hl:

in:

q1: Mit wie vielen Personen wohnen Sie insgesamt – also Sie selbst mit eingeschlossen – zusammen?

is:

it:

st:

ao1: (wohnamio): [number, 2-stellig: 1 To 15], Postfix: Person(en)

mv:

ka:

vc: gesamte Frage wird nur angezeigt, wenn wohnal1 == FALSE

av: 

kh1: (wohnamio): Bitte geben Sie die Anzahl an Personen an, mit denen Sie zusammenwohnen (1 bis 15).


fv:

hv:

fo: 

tr: (siehe unten)

hi: 

\--------------------------------


D3_2
====

tc:

vn: wohncov

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Gehören eine oder mehrere Haushaltsangehörige zur COVID-19-Risikogruppe?

is:

it:

st:

ao1: 1: nein

ao2: 2:  ja

ao3: 3:  weiß ich nicht

mv:

ka:

vc: gesamte Frage wird nur angezeigt, wenn wohnal1 == FALSE

av: 

kh: 

fv:

hv:

fo: 

tr: (siehe unten)

hi: 

\--------------------------------

D3_2
====

tc:

vn: wohnqmw; wohnqmz

qt: offene Angaben

hl:

in:

q3: Wie groß ist Ihre Wohnung/Ihr Haus?


is:

it:

st:

ao3: (wohnqmw): [number, 3-stellig: 1 TO 999], Postfix: m²

mv:

ka:

vc: 

av: 

kh2: (wohnqmw): Bitte geben Sie die Größe Ihrer Wohnung/Ihres Hauses an (1 bis 999).

fv:

hv:

fo: 

tr:

GOTO CO_10

hi: 

\--------------------------------

D3_2
====

tc:

vn: wohnqmw; wohnqmz

qt: offene Angaben

hl:

in:

q4: Wie groß ist das von Ihnen genutzte Zimmer?

is:

it:

st:

ao4: (wohnqmz): [number, 2-stellig: 1 TO 99], Postfix: m²

mv:

ka:

vc: gesamte Frage wird nur angezeigt, wenn wohnal1 == FALSE

av: 

kh3: (wohnqmz): Bitte geben Sie die Größe Ihres Zimmers an (1 bis 99).

fv:

hv:

fo: 

tr:

GOTO CO_10

hi: 

\--------------------------------


CO_10
=========

tc:

vn: VCO_10_ (VCO_10_a; VCO_10_b; VCO_10_c; VCO_10_d; VCO_10_e; VCO_10_f; VCO_10_g VCO_10_h; VCO_10_i; VCO_10_j)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wenn Sie an Ihre bisherigen Erfahrungen mit digitaler Lehre denken: Inwiefern stimmen Sie den folgenden Aussagen zu?

is:

it1: (VCO_10_a): Meine Wohnsituation ist für viele Formen digitaler Lehre nicht geeignet.
	
it2: (VCO_10_b): Meine Internetverbindung ist für viele Formen digitaler Lehre nicht geeignet.

it3: (VCO_10_c): Mein Rechner ist für viele Formen digitaler Lehre nicht geeignet.

it4: (VCO_10_d): Viele Formen digitaler Lehre sind für mich nicht nutzbar/zugänglich.

it5: (VCO_10_e): Durch den Einsatz digitaler Lehrformate bin ich zeitlich flexibler.

it6: (VCO_10_f): Digitale Lehre führt zu einem effizienteren Studium.

it7: (VCO_10_g): Mir fehlt der persönliche Austausch mit anderen Studierenden.

it8: (VCO_10_h): Mir fehlt der persönliche Austausch mit Lehrenden.

it9: (VCO_10_i): Die digitalen Plattformen/Tools meiner Hochschule funktionieren auch unter der aktuellen Belastung reibungslos.

it10: (VCO_10_j): Im Rahmen digitaler Lehrformate lassen sich Fragen mindestens genauso gut klären wie im persönlichen Kontakt.

st:

ao1: 1:  trifft gar nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5:   trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO N_16

hi:

\--------------------------------

N_16
=========

tc:

vn: lftaus (lftaus1; lftaus2; lftaus3; lftaus4)
 
       

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie wichtig sind Ihnen folgende Freizeitaktivitäten in Ihrem Leben?

is: 

it1: (lftaus1): künstlerisch und kulturell aktiv sein 

it2: (lftaus2): Bücher lesen

it3: (lftaus3): Freund*innen treffen

it4: (lftaus4): sportlich aktiv sein

st:

ao1: 1: unwichtig

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: sehr wichtig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO B2_5

hi:

\------------------------------------------------------------


B2_5
=========

tc:

vn: VB2_5_ (VB2_5_a; VB2_5_b; VB2_5_c; VB2_5_d)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig gehen Sie in der aktuellen Situation folgenden Freizeitaktivitäten nach?

is:

it1: (VB2_5_a): künstlerisch und kulturell aktiv sein 

it2: (VB2_5_b): Bücher lesen

it3: (VB2_5_c): Freund*innen treffen

it4: (VB2_5_d): sportlich aktiv sein

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

GOTO D3_22

hi:

\------------------------------------------------------------


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

it3: (zufrfinsit): … Ihrer Freizeit?

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

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_16

hi:

\--------------------------------


A_16
=========

tc:

vn: imausl

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Befinden Sie sich zurzeit studienbezogen außerhalb Deutschlands?

is:

it:

st:

ao1: 1: nein

ao2: 2: nein, musste den Auslandsaufenthalt abbrechen

ao3: 3: nein, konnte den Auslandsaufenthalt nicht antreten

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

GOTO A_54

hi:

\------------------------------------------------------------


A_54
=========

tc:

vn: ainfaus

qt: Einfachauswahl

hl:

in:

q: Waren Sie im Rahmen Ihres Studiums bereits im Ausland?

is: 

it:

st:

ao1: 1: nein

ao2: 2: ja, ein Aufenthalt

ao3: 3: ja, zwei Aufenthalte

ao4: 4: ja, drei oder mehr Aufenthalte

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A_55

hi:

\------------------------------------------------------------

A_55
=========

tc:

vn: auslandint

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor, künftig einen weiteren studienbezogenen Auslandsaufenthalt durchzuführen?

is:

it:

st:

ao1: 1: nein, kein Interesse

ao2: 2: nein, sehe keine Realisierungschance

ao3: 3: weiß ich noch nicht

ao4: 4: ja, geplant

ao5: 5: ja, bereits in Vorbereitung


mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_15

hi:

\------------------------------------------------------------


F1_15
=====

tc:

vn: azufrsichba

qt: Einfachauswahl mit horizontalen ao 

hl:

in:

q1: (azufrsichba): Wie sicher fühlen Sie sich in Deutschland insgesamt?

is:

it:

st:


ao1: (azufrsichba): 1: gar nicht sicher

ao2: (azufrsichba): 2:

ao3: (azufrsichba): 3:

ao4: (azufrsichba): 4:

ao5: (azufrsichba): 5: sehr sicher

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO F1_18

hi:

\--------------------------------


F1_18
=====

tc:

vn: aeempfba1; aeempfba2

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Ausgehend von Ihren bisherigen Erfahrungen: Würden Sie Ihren Freund*innen/Bekannten empfehlen, …

is:

it1: (aeempfba1):  … im Ausland zu studieren?

it2: (aeempfba2): … in Deutschland zu studieren?

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

GOTO CO_11

hi:


\--------------------------------

CO_11
=========

tc:

vn: VCO_11_ (VCO_11_a; VCO_11_b; VCO_11_c; VCO_11_d; VCO_11_e; VCO_11_f; VCO_11_g)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Vor dem Hintergrund der Corona-Pandemie: Wie sehr treffen die folgenden Aussagen Ihrer Meinung nach zu?

is:

it1: (VCO_11_a): Ich habe Angst mich mit dem Coronavirus zu infizieren.

it2: (VCO_11_b): Es fällt mir leicht, mich an die einschränkenden Maßnahmen im Zuge der Corona-Pandemie zu halten.

it3: (VCO_11_c): Ich denke, die Veränderungen durch die Corona-Pandemie werden langfristig auch positive Folgen haben.

it4: (VCO_11_d): Risikogruppen sollten in Quarantäne bleiben, damit das „normale Leben“ wieder aufgenommen werden kann.

it5: (VCO_11_e): Ich befolge die Verbote und beachte die Gebote strikt.

it6: (VCO_11_f): Regelungen, die mir weniger einleuchten, nehme ich nicht so ernst.

it7: (VCO_11_g): Alle Gebote und Verbote kann ich gar nicht beachten.

st:

ao1: 1:  trifft gar nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5:   trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_12

hi:

\--------------------------------


CO_12
=========

tc:

vn: VCO_12_ (VCO_12_a; VCO_12_b; VCO_12_c; VCO_12_d; VCO_12_e; VCO_12_f)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie viele Menschen halten Ihrer Meinung nach die folgenden Regeln zur Eindämmung des Coronavirus und der Krise ein?

is:

it1: (VCO_12_a): Abstandsgebot im öffentlichen Raum

it2: (VCO_12_b): Abstandsgebot in den geöffneten Geschäften

it3: (VCO_12_c): Beschränkung der persönlichen Kontakte

it4: (VCO_12_d): Sport im Freien nur allein/zu zweit

it5: (VCO_12_e): Häufiges sorgfältiges Händewaschen

it6: (VCO_12_f): Einhaltung der Nies- und Hustenetikette

It7: (VCO_12_g): Tragen eines Mund-Nasen-Schutzes

st:

ao1: 1:  fast niemand

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5:  fast alle

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_13

hi:

\--------------------------------


CO_13
=========

tc:

vn: VCO_13; VCO_13o

qt: Einfachauswahl mit vertikalen ao und offenen Angaben

hl:

in:

q: Gibt es in Ihrem persönlichen Umfeld jemanden, der positiv auf COVID-19 getestet wurde?

is:

it:

st:

ao1: (VCO_13): 1: nein

ao2: (VCO_13): 2: ja, und zwar: [(VCO_13o), offene Angabe] (bitte Anzahl der Personen angeben)

mv:

ka:

vc:

av:

kh: 

fv:

hv:

fo:

tr:

       GOTO CO_14
	
hi:

\--------------------------------

CO_14
=========

tc:

vn: VCO_14

qt: Einfachauswahl

hl:

in:

q1: Was trifft im Hinblick auf eine potenzielle Ansteckung mit dem COVID-19-Virus auf Sie persönlich zu?

is:

it:

st:

ao1: 1: Ich hatte keine Symptome 

ao2: 2: Ich hatte leichte Symptome

ao3: 3: Ich hatte schwere Symptome


mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr:

GOTO CO_15

hi:

\------------------------------------------------------------

CO_15
=========

tc:

vn: VCO_15

qt: Einfachauswahl

hl:

in:

q1: Wurden Sie bereits auf COVID-19 getestet?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, positiv

ao3: 3: ja, negative

ao4: 4: ja, Ergebnis steht noch auf

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo: 

tr:

GOTO CO_16

hi:

\------------------------------------------------------------



CO_16
=========

tc:

vn: VCO_16_ (VCO_6_a; VCO_6_b; VCO_6_c; VCO_6_d; VCO_6_e)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie groß ist Ihr Vertrauen in Organisationen und Akteure der folgenden Bereiche, gut und richtig mit der Corona-Pandemie umzugehen?

is:

it1: (VCO_16_a): Gesundheitswesen

it2: (VCO_16_b): Wirtschaft

it3: (VCO_16_c): Wissenschaft

it4: (VCO_16_d): Medien

it5: (VCO_16_e): Politik

st:

ao1: 1:  sehr niedrig

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

GOTO CO_17

hi:

\--------------------------------



CO_17
=========

tc:

vn: VCO_17_ (VCO_17_a; VCO_17_b; VCO_17_c; VCO_17_d; VCO_17_e; VCO_17_f)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Rechnen Sie damit, dass sich die Corona-Pandemie auf Ihren Arbeitsmarkteintritt auswirken wird?

is:

it1: (VCO_17_a): Ich werde wohl länger nach einer passenden Stelle suchen müssen.

it2: (VCO_17_b): Ich rechne mit Einbußen beim Gehalt.

it3: (VCO_17_c): Anders als geplant gehe ich von einer Beschäftigung in Teilzeit aus.

it4: (VCO_17_d): Ich werde nicht meine gewünschte Tätigkeit ausüben können.

it5: (VCO_17_e): Wahrscheinlich wird mein Arbeitsvertrag nun befristet sein.

it6: (VCO_17_f): Für den Berufseinstieg werde ich umziehen müssen.

st:

ao1: 1:  nein, sehr unwahrscheinlich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5:    ja, sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO D1_20

hi:

\--------------------------------


D1_20 
===

tc:

vn: kom  (kombela / komteam / komplan /komwisl / komkrit); VD1_20

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit würden Sie sich die folgenden Fähigkeiten und Kenntnisse zuschreiben.

is:


it1: (kombela): Belastbarkeit

it2: (komteam): Teamfähigkeit

it3: (komplan): Planungs- und Organisationsfähigkeit

it4: (komwisl): eigene Wissenslücken erkennen und schließen

it5: (komkrit): kritisches Denken/Ideen hinterfragen

it6: (VD1_20): digitale Kompetenzen


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

GOTO A_57

hi:

\--------------------------------


A_57
=========

tc:

vn: sdkzei (sdkzei1; sdkzei3; sdkzei5; sdkzei8; sdkzei12; sdkzei14; sdkzei16)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie wichtig sind Ihnen die folgenden Aspekte Ihres weiteren Berufs- und Lebensweges?

is:

it1: (sdkzei1): hohes Einkommen

it2: (sdkzei3): sicherer Arbeitsplatz

it3: (sdkzei5): flexible Arbeitszeiten

it4: (sdkzei8): eigene Ideen verwirklichen

it5: (sdkzei12): anderen Menschen helfen zu können

it6: (sdkzei14): Vereinbarkeit von Privatleben und Beruf

it7: (sdkzei16): eine Familie gründen

st:

ao1: 1: unbedeutend

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr bedeutend

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO end

hi:



