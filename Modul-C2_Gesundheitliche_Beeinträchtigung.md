\--------------------------------

C2_1
====

tc: IF gartmob-gartka (Grundprogramm) mindestens einmal =1

vn: gbegrmob; gbegrseh; gbegrohr; gbegrspr; gbegrpsy; gbegrchron; gbegrtls;
gbegrson; gbegrka

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwiefern wirkt sich Ihre Beeinträchtigung bzw. Ihre Beeinträchtigungen auf Ihr aktuelles Studium aus?

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

fo: mv abgesetzt

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

ao11 (bedand): Anderes, und zwar: [bedando] [offenes Eingabefeld]

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

qt: Einfachauswahl mit offenenm Zahlenfeld

hl:

in:

q: Seit wann besteht Ihre Beeinträchtigung?

is: Sofern Ihre Beeinträchtigungen zu unterschiedlichen Zeitpunkten aufgetreten sind, beziehen Sie Ihre Antwort bitte auf die zuerst aufgetretene studienerschwerende Beeinträchtigung.

it:

st:

ao1 (bezeit): 1: : seit meiner Geburt

ao2 (bezeit): 2: : seit meinem [bezeitj] [number] Lebensjahr

mv:

ka:

vc1: SHOW is IF h_gartcount > 1

av: number: 2 stellig: 1 TO 99

kh: Bitte tragen Sie eine Zahl zwischen 1 und 99 ein.

fv:

hv:

fo:

tr: GOTO C2_4

hi:

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

ao2: 2: : Ja, nach einiger Zeit.

ao3: 3: : Ja, bei der ersten Begegnung.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_5 if h_split==1
GOTO C2_6 if h_split==2

hi:

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

ao3: 3: : Nein, weil der Grad der Behinderung niedriger als 50 eingestuft wurde.

ao4: 4: : Ja, mit einem Grad der Behinderung (GdB) von [(beauswo1), number, 3
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

ao3: 3: : Nein, weil der Grad der Behinderung niedriger als 50 eingestuft wurde.

ao4: 4: : Ja, mit einem Grad der Behinderung (GdB) von [(beauswo2), 3 Zeichen,
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

q1: Mit Blick auf Ihr Studium: In welchen Bereichen hatten oder haben Sie im Zusammenhang mit Ihrer Beeinträchtigung bzw. Ihren Beeinträchtigungen Schwierigkeiten?

is: Bitte denken Sie dabei auch an Schwierigkeiten, die – z. B. durch einen Nachteilsausgleich oder individuelle Absprachen – bereits ausgeglichen wurden.
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

mv:

ka:

vc1: SHOW q1 IF h_gartcount = 1

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_8

hi:

\--------------------------------

C2_8
====

tc: IF gartmob-gartka auf [SDK-gub\#01] (Grundprogramm) mindestens einmal =1

vn: ntabau; ntaorg; ntapru; ntaand; ntaando

qt: Einfachauswahlmatrix mit vertikalen ao

hl:

in:

q: In welchen Bereichen haben Sie um individuelle Anpassungen/Absprachen gebeten oder   Nachteilsausgleiche beantragt? Und wurden diese bewilligt?

is: Bitte berücksichtigen Sie sowohl Antragstellungen bei Prüfungsausschüssen/der Hochschulverwaltung als auch informelle Absprachen mit Dozent*innen.

it1: (ntabau): bauliche Barrierefreiheit, räumliche Bedingungen (z. B. Sicht-/Hörverhältnisse)

it2: (ntaorg): Studienorganisation, Lehre und Lernen (z. B. Gestaltung von Lehrveranstaltungen)

it3: (ntapru): Prüfungen, Hausarbeiten und andere Leistungsnachweise (z. B. Art
der Prüfungen)

it4: (ntaand): Anderer Studienbereich, und zwar: [ntaando] [offenes Eingabefeld; 250 Zeichen]

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

tr: GOTO C2_9 IF ntabau=2 OR ntaorg=2 OR ntapru=2 OR ntaand=2

GOTO C2_10 IF ntabau=1 AND ntaorg=1 AND ntapru=1 AND ntaand=1

GOTO C2_11 IF ntabau=3 OR ntaorg=3 OR ntapru=3 OR ntaand=3

ODER

        <zofar:transitions>
            <zofar:transition target="C2_9" condition="zofar.asNumber(ntabau)==2 or zofar.asNumber(ntaorg)==2 or zofar.asNumber(ntapru)==2 or zofar.asNumber(ntaand)==2"/>
            <zofar:transition target="C2_11" condition="zofar.asNumber(ntabau)==3 or zofar.asNumber(ntaorg)==3 or zofar.asNumber(ntapru)==3 or zofar.asNumber(ntaand)==3"/>
	        <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.isMissing(ntaorg) and zofar.isMissing(ntapru) and zofar.isMissing(ntaand)"/>
			<zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.asNumber(ntaorg)==1 and zofar.isMissing(ntapru) and zofar.isMissing(ntaand)"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.asNumber(ntaorg)==1 and zofar.isMissing(ntapru) and zofar.isMissing(ntaand)"/>
            <zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.isMissing(ntaorg) and zofar.asNumber(ntapru)==1 and zofar.isMissing(ntaand)"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.isMissing(ntaorg) and zofar.asNumber(ntapru)==1 and zofar.isMissing(ntaand)"/>
			<zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.asNumber(ntaorg)==1 and zofar.asNumber(ntapru)==1 and zofar.isMissing(ntaand)"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.asNumber(ntaorg)==1 and zofar.asNumber(ntapru)==1 and zofar.isMissing(ntaand)"/>
            <zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.isMissing(ntaorg) and zofar.isMissing(ntapru) and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.isMissing(ntaorg) and zofar.isMissing(ntapru) and zofar.asNumber(ntaand)==1"/>
			<zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.asNumber(ntaorg)==1 and zofar.isMissing(ntapru) and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.asNumber(ntaorg)==1 and zofar.isMissing(ntapru) and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.isMissing(ntaorg) and zofar.asNumber(ntapru)==1 and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.isMissing(ntaorg) and zofar.asNumber(ntapru)==1 and zofar.asNumber(ntaand)==1"/>
			<zofar:transition target="C2_10" condition="zofar.isMissing(ntabau) and zofar.asNumber(ntaorg)==1 and zofar.asNumber(ntapru)==1 and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_10" condition="zofar.asNumber(ntabau)==1 and zofar.asNumber(ntaorg)==1 and zofar.asNumber(ntapru)==1 and zofar.asNumber(ntaand)==1"/>
            <zofar:transition target="C2_12" condition="zofar.isMissing(ntabau) and zofar.isMissing(ntaorg) and zofar.isMissing(ntapru) and zofar.isMissing(ntaand)"/>
		</zofar:transitions>


hi:

\--------------------------------

C2_9
====

tc: IF ntabau=2 OR ntaorg=2 OR ntapru=2 OR ntaand=2

vn: ntahbau; ntahorg; ntahpru; ntahand; ntahando

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie hilfreich waren die zuletzt verabredeten individuellen
Anpassungen/Nachteilsausgleiche?

is:

it1: (ntahbau): bauliche Barrierefreiheit, räumliche Bedingungen (z. B. Sicht-/Hörverhältnisse)

it2: (ntahorg): Studienorganisation, Lehre und Lernen (z. B. Gestaltung von Lehrveranstaltungen)

it3: (ntahpru): Prüfungen, Hausarbeiten und andere Leistungsnachweise (z. B. Art der Prüfungen)

it4: (ntahand): Anderer Studienbereich, und zwar: [ntahando] [Offenes Eingabefeld; 250 Zeichen]

st:

ao1: 1: 1: sehr hilfreich

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: gar nicht hilfreich

ao6: 6: Nicht um individuelle Anpassung gebeten

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

tr: 

GOTO C2_11 IF ntabau=3 OR ntaorg=3 OR ntapru=3 OR ntaand=3

ELSE GOTO C2_12

hi:

\--------------------------------

C2_10
=====

tc: IF ntabau=1 OR ntaorg=1 OR ntapru=1 OR ntaand=1

vn: nbkenn; nbsond; nbhemm; nbsecr; nbsich; nbsupp; nbaufw; nbexp; nbmiss;
nbkons; nband; nbando

qt: Mehrfachauswahl

hl:

in:

q1: Weshalb haben Sie nicht um individuelle Anpassungen/Absprachen gebeten bzw. keine Nachteilsausgleiche beantragt?

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

av:

kh:

fv:

hv:

fo:

tr: GOTO C2_12

hi:

\--------------------------------

C2_11
=====

tc: IF ntabau=3 OR ntaorg=3 OR ntapru=3 OR ntaand=3

vn: kbgrund; kbordn; kbwert; kbbev; kblehr; kbtech; kborga; kbatt; kbzeit;
kband; kbando; kbunbe; kbmem

qt: Mehrfachauswahl; offene Angabe

hl:

in:

q: Weshalb wurden Ihre beantragten Nachteilsausgleiche bzw. individuellen Anpassungen/Absprachen nicht bewilligt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1 (kbgrund): Meine Beeinträchtigung(en) wurde(n) nicht als Grund akzeptiert.

ao2 (kbordn): Individuelle Anpassungen/Absprachen bzw. Nachteilsausgleiche
wurden als nicht vereinbar mit der Studien-/Prüfungsordnung angesehen.

ao3 (kbwert): Ersatzleistung wurde nicht als gleichwertig angesehen.

ao4 (kbbev): Individuelle Anpassung/Absprache bzw. Nachteilsausgleich wird als
Bevorzugung angesehen.

ao5 (kblehr): Lehrende*r war nicht dazu bereit, Lehrroutinen zu ändern.

ao6 (kbtech): Aufgrund technischer Probleme (z. B. fehlende Ausstattung).

ao7 (kborga): Aufgrund organisatorischer Probleme (z. B. keine Raum- oder Prüfungsverlegung
möglich).

ao8 (kbatt): Aufgrund fehlender Nachweise (z. B. fachärztliches Attest,
Schwerbehindertenausweis).

ao9 (kbzeit): Nachteilsausgleiche und/oder individuellen Anpassungen/Absprachen wurden zu spät beantragt.

ao10 (kband): Anderer Grund, und zwar: [(kbando), 250 Zeichen]

ao12 (kbunbe): mir nicht bekannt

ao13 (kbmem): weiß ich nicht

mv:

ka:

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

q: Welche Angebote für eine persönliche Beratung zum Thema Studium und Beeinträchtigung kennen Sie bzw. haben Sie genutzt?

is:

it1: beauftr: Beratungsstellen für Studierende mit
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

ELSE GOTO A_16

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
