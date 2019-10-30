\--------------------------------

C2_1
====

tc: IF gartmob-gartka (Grundprogramm) mindestens einmal =1

vn: gbegrmob; gbegrseh; gbegrohr; gbegrspr; gbegrpsy; gbegrchron; gbegrtls;
gbegrson; gbegrka

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q1: Wie stark wirkt sich Ihre Beeinträchtigung im aktuellen Studium aus?

q2: Wie stark wirken sich Ihre Beeinträchtigungen im aktuellen Studium aus?

is:

it1: (gbegrmob): Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

it2: (gbegrseh): Sehbeeinträchtigung/Blindheit

it3: (gbegrohr): Hörbeeinträchtigung/Gehörlosigkeit

it4: (gbegrspr): Sprechbeeinträchtigung (z. B. Stottern)

it5: (gbegrpsy): psychische Erkrankung (z. B. Depression, Essstörung)

it6: (gbegrchron): länger dauernde Krankheit/chronische Krankheit (z. B. Rheuma,
MS, Darmerkrankung)

it7: (gbegrtls): Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

it8: (gbegrson): andere Beeinträchtigung/schwere Erkrankung (z. B.
Tumorerkrankung, Autismus-Spektrum-Störung)

it9: (gbegrka): Beeinträchtigung ohne Zuordnung

st:

ao1: 1: 1: sehr schwach

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr stark

mv: -13: : gar nicht

ka:

vc1: SHOW q1 IF h_gartcount = 1

vc2: SHOW q2 IF h_gartcount > 1

vc3: SHOW it1 IF gartmob=1

vc4: SHOW it2 IF gartseh=1

vc5: SHOW it3 IF gartohr=1

vc6: SHOW it4 IF gartspr=1

vc7: SHOW it5 IF gartpsy=1

vc8: SHOW it6 IF gartsom=1

vc9: SHOW it7 IF garttls=1

vc10: SHOW it8 IF gartson=1

vc11: SHOW it9 IF gartka=1

av:

kh:

fv:

hv:

fo: ao6 abgesetzt

tr: GOTO C2_2

hi:

\--------------------------------

C2_2
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: bedno; bedbau; bedori; bedauss; bedsich; bedaku; bedruh; bedmed ; bedpers;
bedtech; bedand; bedando

qt: Mehrfachnennung; offene Abgabe

hl:

in:

q: Haben Sie aufgrund Ihrer Beeinträchtigung spezielle Bedürfnisse?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (bedno): nein [EK]

ao2 (bedbau): bauliche Barrierefreiheit der Gebäude (z. B. Rampen, Aufzüge,
selbstöffnende Türen, barrierefreie WCs)

ao3 (bedori): taktile, optische oder akustische Leitsysteme, Wegbeschreibungen
oder Orientierungshilfen

ao4 (bedauss): spezielle technische Ausstattungen an der Hochschule (z. B.
unterfahrbare Tische, Großbildschirme, Induktionsschleifen, barrierefreie
PC-Arbeitsplätze)

ao5 (bedsich): störungsfreie/-arme Sichtverhältnisse

ao6 (bedaku): störungsfreie/-arme Hörverhältnisse/Akustik

ao7 (bedruh): Ruhe-/Rückzugsräume

ao8 (bedmed): barrierefrei aufbereitete Medien (z. B. Dokumente, Formulare,
Literatur, Webseiten)

ao9 (bedpers): personelle Assistenzen (z. B. Pflegeassistenz, Mitschreibkraft,
Gebärdensprachdolmetscher\*in)

ao10 (bedtech): technische Hilfsmittel zum individuellen Gebrauch (z. B. Screen
Reader, Braille-Zeile, FM-Anlage)

ao11 (bedand): Anderes, und zwar: [[bedando] 250 Zeichen]

mv:

ka (ao2 TO ao11): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_3

hi:

\--------------------------------

C2_3
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: bezeit; bezeitj

qt: Einfachauswahl mit Dropdown-Menü

hl:

in:

q: Seit wann besteht Ihre Beeinträchtigung?

is: Sofern Ihre Beeinträchtigungen zu unterschiedlichen Zeitpunkten aufgetreten
sind, beziehen Sie Ihre Antwort bitte auf die zuerst aufgetretene
studienerschwerende Beeinträchtigung.

it:

st:

ao1 (bezeit): 1: : seit meiner Geburt

ao2 (bezeit): 2: : 0,5 cm, seit meinem [number]. Lebensjahr

mv:

ka:

vc: SHOW is IF Zahl der Nennungen von gartmob bis gartka \> 1

av: number: 2 stellig: 1 TO 99

kh: Bitte tragen Sie eine Zahl zwischen 1 und 99 ein.

fv:

hv:

fo:

tr: GOTO C2_4

hi: \@ ZOFAR: Wie sollen diese Drop-Down-Listen hier codiert werden? / soll eine
Ziffernliste von 1. bis 99. Enthalten

\--------------------------------

C2_4
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: bewahr

qt: Einfachauswahl

hl:

in:

q: Ist für andere wahrnehmbar, dass Sie eine Beeinträchtigung haben?

is:

it:

st:

ao1: 1: : nein

ao2: 2: : Ja, möglicherweise nach einiger Zeit.

ao3: 3: : Ja, bei der ersten Begegnung.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_5 / C2_6 (50%-50%-Split)

hi: \@ ZOFAR: Wahrscheinlich legt ihr für den Split eine Systemvariable an? Wie
soll das in dieser Vorlage codiert werden?

\--------------------------------

C2_5
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: beausw1; beauswo1

qt: Einfachauswahl; offene Angabe

hl:

in:

q: Haben Sie einen Schwerbehindertenausweis?

is:

it:

st:

ao1: 1: : Nein, habe ich nicht beantragt.

ao2: 2: : Nein, weil keine Behinderung festgestellt wurde.

ao4: 3: : Ja, mit einem Grad der Behinderung (GdB) von [(beauswo1), number, 3
Zeichen]

mv:

ka:

vc:

av: number : \<=dreistellig : 0 TO 100

kh: Bitte tragen Sie eine Zahl zwischen 0 und 100 ein.

fv:

hv:

fo:

tr: GOTO C2_7

hi:

\--------------------------------

C2_6
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: beausw2; beauswo2

qt: Einfachauswahl; offene Angabe

hl:

in:

q: Wurde Ihre Beeinträchtigung amtlich festgestellt?

is:

it:

st:

ao1: 1 : Nein, habe ich nicht beantragt.

ao2: 2: : Nein, weil keine Behinderung festgestellt wurde.

ao3: 3: : Ja, mit einem Grad der Behinderung (GdB) von [(beauswo2), 3 Zeichen,
number]

mv:

ka:

vc:

av: number : \<=dreistellig : 0 TO 100

kh: Bitte tragen Sie eine Zahl zwischen 0 und 100 ein.

fv:

hv:

fo:

tr: GOTO C2_7

hi:

\--------------------------------

C2_7
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: schwbau; schworg; schwpru; schwand; schwando, schwno

qt: Mehrfachauswahl; offene Angabe

hl:

in:

q1: Mit Blick auf Ihr Studium: In welchen Bereichen hatten oder haben Sie im Zusammenhang mit Ihrer
Beeinträchtigung Schwierigkeiten?

q2: Mit Blick auf Ihr Studium: In welchen Bereichen hatten oder haben Sie im Zusammenhang mit Ihren
Beeinträchtigungen Schwierigkeiten?

is: Bitte denken Sie dabei auch an Schwierigkeiten, die – z. B. durch einen
Nachteilsausgleich oder individuelle Absprachen – bereits ausgeglichen wurden.
Bitte alles Zutreffende auswählen.

it:

st:

ao1 (schwbau): bauliche Barrierefreiheit, räumliche Bedingungen (z. B.
Zugänglichkeit und Orientierung, Sicht-/Hörverhältnisse, Rückzugsräume)

ao2 (schworg): Studienorganisation, Lehre und Lernen (z. B. unflexibler
Stundenplan, Gestaltung von Lehrveranstaltungen, Gruppenarbeit, Auslandsstudium,
Praktika)

ao3 (schwpru): Prüfungen, Hausarbeiten und andere Leistungsnachweise (z. B. Art
der Prüfungen, zeitliche Vorgaben)

ao4 (schwand): Anderer Studienbereich, und zwar: [(schwando): 250 Zeichen]

ao5 (schwno): keine beeinträchtigungsbedingten Schwierigkeiten [EK]

mv:

ka:

vc1: SHOW q1 IF h_gartcount = 1

vc2: SHOW q2 IF h_gartcount > 1

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_8 IF schwno <> 1

ELSE GOTO C2_12 

hi:

\--------------------------------

C2_8
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: ntabau; ntaorg; ntapru; ntaand; ntaando

qt: Einfachauswahlmatrix mit vertikalen ao

hl:

in:

q: In welchen Bereichen haben Sie um individuelle Anpassungen/Absprachen gebeten
oder Nachteilsausgleiche beantragt? Und wurden diese bewilligt?

is: Bitte berücksichtigen Sie sowohl Antragstellungen bei
Prüfungsausschüssen/der Hochschulverwaltung als auch informelle Absprachen mit
Dozent\*innen.

Bei mehreren Anträgen/Bitten um Anpassungen im selben Bereich, denken Sie bitte
an die letzte Situation

it1: (ntabau): bauliche Barrierefreiheit, räumliche Bedingungen (z. B.
Zugänglichkeit und Orientierung, Sicht-/Hörverhältnisse, Rückzugsräume)

it2: (ntaorg): Studienorganisation, Lehre und Lernen (z. B. unflexibler
Stundenplan, Gestaltung von Lehrveranstaltungen, Gruppenarbeit, Auslandsstudium,
Praktika)

it3: (ntapru): Prüfungen, Hausarbeiten und andere Leistungsnachweise (z. B. Art
der Prüfungen, zeitliche Vorgaben)

it4: (ntaand): Anderer Studienbereich, und zwar: [(ntaando): 250 Zeichen]

st:

ao1: 1: : nicht beantragt

ao2: 2: : beantragt, wurde bewilligt

ao3: 3: : beantragt, wurde nicht bewilligt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_9 IF ntabau=2 OR ntaorg=2 OR ntaorg=2 OR ntaand=2

GOTO C2_10 IF ntabau=1 OR ntaorg=1 OR ntaorg=1 OR ntaand=1

GOTO C2_11 IF ntabau=3 OR ntaorg=3 OR ntaorg=3 OR ntaand=3

hi:

\--------------------------------

C2_9
====

tc: IF ntabau=2 OR ntaorg=2 OR ntaorg=2 OR ntaand=2

vn: ntahbau; ntahorg; ntahpru; ntahand; ntahando

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie hilfreich waren die zuletzt verabredeten individuellen
Anpassungen/Nachteilsausgleiche?

is:

it1: (ntahbau): bauliche Barrierefreiheit, räumliche Bedingungen (z. B.
Zugänglichkeit und Orientierung, Sicht-/Hörverhältnisse, Rückzugsräume)

it2: (ntahorg): Studienorganisation, Lehre und Lernen (z. B. unflexibler
Stundenplan, Gestaltung von Lehrveranstaltungen, Gruppenarbeit, Auslandsstudium,
Praktika)

it3: (ntahpru): Prüfungen, Hausarbeiten und andere Leistungsnachweise (z. B. Art
der Prüfungen, zeitliche Vorgaben)

it4: (ntahand): Anderer Studienbereich, und zwar: [(ntahando), 250 Zeichen]

st:

ao1: 1: 1: sehr hilfreich

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: gar nicht hilfreich

ka:

vc1: SHOW it1 IF ntabau = 2

vc2: SHOW it2 IF ntaorg = 2

vc3: SHOW it3 IF ntapru = 2

vc4: SHOW it4 IF ntaand = 2

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_10 IF ntabau=1 OR ntaorg=1 OR ntaorg=1 OR ntaand=1

GOTO C2_11 IF ntabau=3 OR ntaorg=3 OR ntaorg=3 OR ntaand=3

ELSE GOTO C2_12

hi:

\--------------------------------

C2_10
=====

tc: IF ntabau=1 OR ntaorg=1 OR ntaorg=1 OR ntaand=1

vn: nbkenn; nbsond; nbhemm; nbsecr; nbsich; nbsupp; nbaufw; nbexp; nbmiss;
nbkons; nband; nbando

qt: Mehrfachauswahl

hl:

in:

q1: Sie haben angegeben, mit räumlichen Bedingungen Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q2: Sie haben angegeben, mit der Studienorganisation/Lehre Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q3: Sie haben angegeben, mit Prüfungen Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q4: Sie haben angegeben, in einem (weiteren) anderen Bereich Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q5: Sie haben angegeben, mit räumlichen Bedingungen und der Studienorganisation/Lehre Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q6: Sie haben angegeben, mit räumlichen Bedingungen und Prüfungen Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q7: Sie haben angegeben, mit räumlichen Bedingungen und einem anderen Bereich Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q8: Sie haben angegeben, mit der Studienorganisation/Lehre und Prüfungen Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q9: Sie haben angegeben, mit der Studienorganisation/Lehre und einem anderen Bereich Schwierigkeiten zu haben: Weshalb haben Sie
nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q10: Sie haben angegeben, mit Prüfungen und einem anderen Bereich Schwierigkeiten zu haben: Weshalb haben Sie nicht
um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q11: Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q12: Sie haben angegeben, mit räumlichen Bedingungen, Prüfungen und einem anderen Bereich Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q13: Sie haben angegeben, mit der Studienorganisation/Lehre, Prüfungen und einem anderen Bereich Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q14: Sie haben angegeben, mit räumlichen Bedingungen, der Studienorganisation/Lehre und Prüfungen Schwierigkeiten zu haben:
Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

q15: Sie haben angegeben, mit räumlichen Bedingungen, der Studienorganisation/Lehre und einem anderen Bereich Schwierigkeiten
zu haben: Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (nbkenn): Die Möglichkeit war mir nicht bekannt.

ao2 (nbsond): Ich will keine „Sonderbehandlung“.

ao3 (nbhemm): Ich hatte Hemmungen, mich aufgrund meiner
beeinträchtigungsbedingten Probleme an jemanden zu wenden.

ao4 (nbsecr): Ich will/wollte meine Beeinträchtigung nicht preisgeben.

ao5 (nbsich): Ich bin nicht sicher, ob ich anspruchsberechtigt bin oder mein
Antrag Chancen hat.

ao6 (nbsupp): Ich wusste nicht, wen ich um Unterstützung/Beratung hätte bitten
können.

ao7 (nbaufw): Es wäre zu viel Aufwand gewesen.

ao8 (nbexp): Weil ich mich früher schon erfolglos um individuelle
Anpassungen/Absprachen bzw. Nachteilsausgleiche bemüht habe.

ao9 (nbmiss): Ich glaube nicht, dass sich meine Situation ändern lässt.

ao10 (nbkons): Weil ich dadurch Nachteile im weiteren Studium befürchte.

ao11 (nband): Aus anderen Gründen, und zwar: [(nbando), 350 Zeichen]

mv:

ka:

vc1: SHOW q1 IF ntabau=1 AND ntaorg<>1 AND ntapru<>1 AND ntaand<>1

vc2: SHOW q2 IF ntaorg=1 AND ntabau<>1 AND ntapru<>1 AND ntaand<>1

vc3: SHOW q3 IF ntapru=1 AND ntabau<>1 AND ntaorg<>1 AND ntaand<>1

vc4: SHOW q4 IF ntaand=1 AND ntabau<>1 AND ntaorg<>1 AND ntapru<>1

vc5: SHOW q5 IF ntabau=1 AND ntaorg=1 AND ntapru<>1 AND ntaand<>1

vc6: SHOW q6 IF ntabau=1 AND ntapru=1 AND ntaorg<>1 AND ntaand<>1

vc7: SHOW q7 IF ntabau=1 AND ntaand=1 AND ntaorg<>1 AND ntapru<>1

vc8: SHOW q8 IF ntaorg=1 AND ntapru=1 AND ntabau<>1 AND ntaand<>1

vc9: SHOW q9 IF ntaorg=1 AND ntaand=1 AND ntabau<>1 AND ntapru<>1

vc10: SHOW q10 IF ntapru=1 AND ntaand=1 AND ntabau<>1 AND ntaorg<>1

vc11: SHOW q11 IF ntabau=1 AND ntaorg=1 AND ntapru=1 AND ntaand=1

vc12: SHOW q12 IF ntabau=1 AND ntapru=1 AND ntaand=1 AND ntaorg<>1

vc13: SHOW q13 IF ntaorg=1 AND ntapru=1 AND ntaand=1 AND ntabau<>1

vc14: SHOW q14 IF ntabau=1 AND ntaorg=1 AND ntapru=1 AND ntaand<>1

vc15: SHOW q15 IF ntabau=1 AND ntaorg=1 AND ntaand=1 AND ntapru<>1

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_11 IF ntabau=3 OR ntaorg=3 OR ntaorg=3 OR ntaand=3

ELSE GOTO C2_12

hi:

\--------------------------------

C2_11
=====

tc: IF ntabau=3 OR ntaorg=3 OR ntaorg=3 OR ntaand=3

vn: kbgrund; kbordn; kbwert; kbbev; kblehr; kbtech; kborga; kbatt; kbzeit;
kband; kbando; kbunbe; kbmem

qt: Mehrfachauswahl; offene Angabe

hl:

in:

q1: Weshalb wurde der zuletzt beantragte Nachteilsausgleich und/oder individuelle Anpassung/Absprache
in Bezug auf die räumlichen Bedingungen nicht bewilligt?

q2: Weshalb wurde der zuletzt beantragte Nachteilsausgleich und/oder individuelle Anpassung/Absprache
in Bezug auf die Studienorganisation/Lehre nicht bewilligt?

q3: Weshalb wurde der zuletzt beantragte Nachteilsausgleich und/oder individuelle Anpassung/Absprache
in Bezug auf Prüfungen nicht bewilligt?

q4: Weshalb wurde der zuletzt beantragte Nachteilsausgleich und/oder individuelle Anpassung/Absprache
in Bezug auf einen anderen Bereich nicht bewilligt?

q5: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen und die Studienorganisation/Lehre nicht bewilligt?

q6: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen und Prüfungen nicht bewilligt?

q7: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen und einen anderen Bereich nicht bewilligt?

q8: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die Studienorganisation/Lehre und Prüfungen nicht bewilligt?

q9: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die Studienorganisation/Lehre und einen anderen Bereich nicht bewilligt?

q10: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf Prüfungen und einen anderen Bereich nicht bewilligt?

q11: Weshalb wurde mindestens einer der zuletzt beantragten Nachteilsausgleiche
und/oder individuellen Anpassungen/Absprachen nicht bewilligt?

q12: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen, Prüfungen und einen anderen Bereich nicht bewilligt?

q13: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die Studienorganisation/Lehre, Prüfungen und einen anderen Bereich nicht bewilligt?

q14: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen, die Studienorganisation/Lehre und Prüfungen nicht bewilligt?

q15: Weshalb wurden die zuletzt beantragten Nachteilsausgleiche und/oder individuelle Anpassungen/Absprachen
in Bezug auf die räumlichen Bedingungen, die Studienorganisation/Lehre und einen anderen Bereich nicht bewilligt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (kbgrund): Meine Beeinträchtigung(en) wurde(n) nicht als Grund akzeptiert.

ao2 (kbordn): Individuelle Anpassungen/Absprachen bzw. Nachteilsausgleiche
wurden als nicht vereinbar mit der Studien-/Prüfungsordnung angesehen.

ao3 (kbwert): Ersatzleistung wurde nicht als gleichwertig angesehen.

ao4 (kbbev): Individuelle Anpassung/Absprache bzw. Nachteilsausgleich wird als
Bevorzugung angesehen.

ao5 (kblehr): Lehrende\*r war nicht dazu bereit, Lehrroutinen zu ändern.

ao6 (kbtech): Aufgrund technischer Probleme (z. B. fehlende Ausstattung).

ao7 (kborga): Aufgrund organisatorischer Probleme (z. B. keine Raum- oder Prüfungsverlegung
möglich).

ao8 (kbatt): Aufgrund fehlender Nachweise (z. B. fachärztliches Attest,
Schwerbehindertenausweis).

ao9 (kbzeit): Nachteilsausgleiche und/oder individuellen Anpassungen/Absprachen wurden zu spät beantragt.

ao10 (kband): Anderer Grund, und zwar: [(kbando), 250 Zeichen]

ao12 (kbunbe): Ist mir nicht bekannt.

ao13 (kbmem): Weiß ich nicht mehr.

mv:

ka:

vc1: SHOW q1 IF ntabau=3 AND ntaorg<>3 AND ntapru<>3 AND ntaand<>3

vc2: SHOW q2 IF ntaorg=3 AND ntabau<>3 AND ntapru<>3 AND ntaand<>3

vc3: SHOW q3 IF ntapru=3 AND ntabau<>3 AND ntaorg<>3 AND ntaand<>3

vc4: SHOW q4 IF ntaand=3 AND ntabau<>3 AND ntaorg<>3 AND ntapru<>3

vc5: SHOW q5 IF ntabau=3 AND ntaorg=3 AND ntapru<>3 AND ntaand<>3

vc6: SHOW q6 IF ntabau=3 AND ntapru=3 AND ntaorg<>3 AND ntaand<>3

vc7: SHOW q7 IF ntabau=3 AND ntaand=3 AND ntaorg<>3 AND ntapru<>3

vc8: SHOW q8 IF ntaorg=3 AND ntapru=3 AND ntabau<>3 AND ntaand<>3

vc9: SHOW q9 IF ntaorg=3 AND ntaand=3 AND ntabau<>3 AND ntapru<>3

vc10: SHOW q10 IF ntapru=3 AND ntaand=3 AND ntabau<>3 AND ntaorg<>3

vc11: SHOW q11 IF ntabau=3 AND ntaorg=3 AND ntapru=3 AND ntaand=3

vc12: SHOW q12 IF ntabau=3 AND ntapru=3 AND ntaand=3 AND ntaorg<>3

vc13: SHOW q13 IF ntaorg=3 AND ntapru=3 AND ntaand=3 AND ntabau<>3

vc14: SHOW q14 IF ntabau=3 AND ntaorg=3 AND ntapru=3 AND ntaand<>3

vc15: SHOW q15 IF ntabau=3 AND ntaorg=3 AND ntaand=3 AND ntapru<>3

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_12

hi:

\--------------------------------

C2_12
=====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: beauftr; besoz; bepsy; bestud; beselb; beand; beandhs; beandhso; beandauß;
beandaußo

qt: Einfachauswahlmatrix mit horizontalen ao und offener Nachfrage

hl:

in:

q: Welche Angebote für eine persönliche Beratung zum Thema Studium und
Beeinträchtigung kennen Sie bzw. haben Sie genutzt?

is:

it1: beauftr: eratungsstellen für Studierende mit
Beeinträchtigungen der Hochschule

it2: besoz: Beratungsstelle für Studierende mit
Beeinträchtigungen des Studentenwerks

it3: bepsy: psychologische Beratungsstelle des Studentenwerks/der Hochschule

it4: bestud: Beratung für Studierende mit Beeinträchtigungen des
AStA, StuRa, UStA etc.

it5: beselb: studentische Behindertenselbsthilfe (u. a. BHSA, DVBS, BAG Behinderung
und Studium)

it6: beand: studienbezogene Beratung anderer Selbsthilfevereinigungen

it7: beandhs: (Anderes) beeinträchtigungsspezifisches Beratungsangebot ++an der
Hochschule++, und zwar: [(beandhso), 150 Zeichen]

it8: beandauß: (Anderes) beeinträchtigungsspezifisches Beratungsangebot
++außerhalb der Hochschule++, und zwar: [(beandaußo), 150 Zeichen]

st:

ao1: 1: : kenne ich nicht/sind nicht vorhanden

ao2: 2: : kenne ich, aber nicht genutzt

ao3: 3: : habe ich genutzt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_13 IF beauftr = 3 OR besoz = 3 OR bepsy = 3 OR bestud = 3 OR beselb =
3 OR beand = 3

ELSE GOTO nächstes Modul

hi:

\--------------------------------

C2_13
=====

tc: IF beauftr = 3 OR besoz =3 OR bepsy = 3 OR bestud = 3 OR beselb = 3 OR beand
= 3

vn: behauftr; behsoz; behpsy; behstud; behselb; behand)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie hilfreich waren diese Angebote für Sie?

is:

it1: (behauftr): Beauftragte/Beratungsstellen für Studierende mit
Behinderungen/Beeinträchtigungen der Hochschule

it2: (behsoz): Sozialberatung/Beratungsstelle für Studierende mit
Behinderungen/Beeinträchtigungen des Studentenwerks

it3: (behpsy): psychologische Beratungsstelle des Studentenwerks/der Hochschule

it4: (behstud): Beratung für Studierende mit Behinderungen/Beeinträchtigungen
des AStA, StuRa, UStA etc.

it5: (behselb): studentische Behindertenselbsthilfe (u. a. BHSA, DVBS, BAG Behinderung
und Studium)

it6: (behand): studienbezogene Beratung anderer Selbsthilfevereinigungen

st:

ao1: 1: 1: gar nicht hilfreich

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr hilfreich

mv:

ka:

vc: SHOW it1 IF beauftr =3

SHOW it2 IF besoz =3

SHOW it3 IF bepsy =3

SHOW it4 IF bestud =3

SHOW it5 IF beselb =3

SHOW it6 IF beand =3

av:

kh:

fv:

hv:

fo:

tr: GOTO A_16

hi:
