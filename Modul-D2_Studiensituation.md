**------------------------------------------------------------**

**Qualität der Ausstattung**

D2_2
-------

tc:

vn: ssqualeq (ssqualeq1; ssqualeq2; ssqualeq3; ssqualeq4; ssqualeq5; ssqualeq6; ssqualeq7; ssqualeq8; ssqualeq9; ssqualeq10; ssqualeg11)

qt: Einfachauswahlmatrix/5er-Skala mit Zwischenüberschriften und horizontalen ao

hl:

in:

q: Wie bewerten Sie Ihre Hochschule hinsichtlich folgender Aspekte?

is:

it1: (ssqualeq1): Gesamtzustand der Veranstaltungsräume (Funktionalität, Mobiliar, Belüftung)

it2: (ssqualeq2): technische Ausstattung der Veranstaltungsräume (z. B. Beamer, Smartboards)

it3: (ssqualeq3): Verfügbarkeit und Ausstattung fachspezifischer Übungsräume (z. B. Labore, Werkstätten, Sportübungsräume)

it4: (ssqualeq4): Verfügbarkeit und Ausstattung von Räumen zum eigenständigen Lernen

it5: (ssqualeq5): Zugang zum W-LAN

it6: (ssqualeq6): IT-/digitale Ausstattung (z. B. Software)

it7: (ssqualeq7): Öffnungszeiten der Bibliothek

it8: (ssqualeq8): Verfügbarkeit von Fachliteratur

it9: (ssqualeq9): Service- und Beratungsleistungen

it10: (ssqualeq10): Betreuungsangebote für Studierende mit Kind(ern)

it11: (ssqualeq11): Unterstützungsangebote für Studierende mit Beeinträchtigung(en) (z. B. spezifisch ausgestattete Arbeitsplätze)

st:

ao1: 1: sehr schlecht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut

mv: -12: weiß ich nicht

ka1: (it1 TO it4): !!räumliche Ausstattung!!

ka2: (it5 TO it11): !!Service-Leistungen!!

vc1: SHOW it10 (ssqualeq10) IF dkinja = 2

vc2: SHOW it11 (ssqualeq11) IF h_gartcount >= 1

av:

kh:

fv:

hv:

fo1: Bitte über it1 "räumliche Ausstattung" linksbündig positionieren.

fo2: Bitte über it5 "Service-Leistungen" linksbündig positionieren.

fo3: mv/"weiß ich nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="D2_6a"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**Strukturiertheit des Studienangebots**

D2_3
-------

tc:

vn: ssstruk (ssstruk1; ssstruk2; ssstruk3; ssstruk4; ssstruk5; ssstruk6; ssstruk7; ssstruk8; ssstruk9, ssstruk10)

qt: Einfachauswahlmatrix/5er-Skala mit Zwischenüberschriften und horizontalen ao

hl:

in:

q: Inwieweit treffen folgende Aussagen auf Ihr Studium zu?

is:

it1: (ssstruk1): Es bestehen übersichtliche Modulwahlmöglichkeiten.

it2: (ssstruk2): Die Lehrveranstaltungen sind zeitlich gut koordiniert.

it3: (ssstruk3): Lehrveranstaltungstermine fallen häufiger aus.

it4: (ssstruk4): Die Semestervorgaben sind gut erfüllbar.

it5: (ssstruk5): Die einzelnen Module bauen inhaltlich aufeinander auf.

it6: (ssstruk6): Der Zusammenhang mit anderen Fächern wird aufgezeigt.

it7: (ssstruk7): Die Veranstaltungen bereiten gut auf die Prüfungen vor.

it8: (ssstruk8): Die Prüfungen liegen zeitlich oft zu nah beieinander.

it9: (ssstruk9): Das An- und Abmeldeverfahren zu Prüfungen ist unkompliziert.

it10: (ssstruk10): Die Dauer von Prüfungen bzw. Abgabefristen von Hausarbeiten sind angemessen.

st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: trifft voll und ganz zu

mv:

ka1: (it1 TO it4): !!Koordination!!

ka2: (it5 TO it6): !!Inhalte!!

ka3: (it7 TO it10): !!Prüfungsorganisation!!

vc:

av:

kh:

fv:

hv:

fo1: Bitte über it1 "Koordination" linksbündig positionieren.

fo2: Bitte über it5 "Inhalte" linksbündig positionieren.

fo3: Bitte über it7 "Prüfungsorganisation" linksbündig positionieren.

tr:

	<zofar:transitions>
            <zofar:transition target="N_9c" condition="zofar.asNumber(PRELOADhs_co)==1"/> 
            <zofar:transition target="N_9b"/>
        </zofar:transitions>


hi:

**------------------------------------------------------------**

**Größe/Struktur des Studiengangs**

D2_4
-------

tc:

vn: ssstud (ssstud1; ssstud2; ssstud3; ssstud4; ssstud5; ssstud6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Auf wie viele Lehrveranstaltungen, die Sie in diesem Semester besuchen, trifft Folgendes zu?

is:.

it1: (ssstud1): Die Lehrveranstaltung ist überfüllt.

it2: (ssstud2): Es besteht eine Anmeldepflicht.

it3: (ssstud3): Es besteht eine Anwesenheitspflicht.

it4: (ssstud4): Die Lehrveranstaltung wird als Videokonferenz/Web-Seminar angeboten.

it5: (ssstud5): Die Lehrveranstaltung ist als Videoaufzeichnung abrufbar.

it6: (ssstud6): Die Lehrveranstaltungssprache ist Englisch.

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

        <zofar:transitions>
            <zofar:transition target="D2_5"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**Anwesenheit**

D2_5
-------

tc:

vn: ssanwesend

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wenn Sie an die von Ihnen belegten Veranstaltungen denken: Wie hoch ist der Anteil der Sitzungen, an denen Sie im Schnitt auch tatsächlich teilnehmen?

is: Gemeint sind alle Formate von Veranstaltungen (Präsenz-/Onlineveranstaltungen).

it:

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

fo: mv/"trifft nicht zu" bitte etwas absetzen.

tr:

	<zofar:transitions>
            <zofar:transition target="B1_7" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6)"/>
            <zofar:transition target="A_28" condition="(zofar.asNumber(mastersplit)==7             or zofar.asNumber(mastersplit)==8             or zofar.asNumber(mastersplit)==11             or zofar.asNumber(mastersplit)==12    )"/>
        </zofar:transitions>


hi: 

**------------------------------------------------------------**

**SSCO 1**

D2_6a
-------

tc:

vn: sscowver (sscowver1; sscowver2; sscowver3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie viel Wert wird in Ihrem Studiengang auf folgende Aspekte gelegt?

is:.

it1: (sscowver1): selbständig zu denken und zu arbeiten

it2: (sscowver2): grundlegende Zusammenhänge zu verstehen

it3: (sscowver3): verschiedene Theorien und Konzepte kritisch vergleichen und beurteilen zu können

st:

ao1: 1: sehr wenig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr viel

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
            <zofar:transition target="D2_7"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**SSCO 2**

D2_7
-------

tc:

vn: sscolehr (sscolehr1; sscolehr2; sscolehr3; sscolehr4; sscolehr5; sscolehr6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte schätzen Sie ein, auf wie viele der Lehrveranstaltungen in Ihrem derzeitigen Studiengang die folgenden Aussagen zutreffen.

is:

it1: (sscolehr1): Die Lehrenden fördern die aktive Mitarbeit der Studierenden.

it2: (sscolehr2): Es wird zum Mitdenken und Durchdenken des Stoffes angeregt.

it3: (sscolehr3): Die Mischung aus Wissensvermittlung und Diskussion ist ausgewogen.

it4: (sscolehr4): Die Lehrenden führen in die Anwendung von Forschungsmethoden ein.

it5: (sscolehr5): Das Lernziel der Lernveranstaltung wird klar definiert.

it6: (sscolehr6): Die Lehrenden sind gut erreichbar.

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

        <zofar:transitions>
            <zofar:transition target="D2_8"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**SSCO 3**

D2_8
-------

tc:

vn: sscofaeh (sscofaeh1; sscofaeh2)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte geben Sie an, inwieweit folgende Aspekte in Ihrem Studiengang gefördert werden.

is:.

it1: (sscofaeh1): Fähigkeit, selbständig forschend tätig zu sein

it2: (sscofaeh2): berufspraktische Fähigkeiten

st:

ao1: 1: gar nicht gefördert

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr stark gefördert

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
            <zofar:transition target="D2_9"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**SSCO 4**

D2_9
-------

tc:

vn: sscofopra (sscofopra1; sscofopra2; sscofopra3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie stark ist Ihr Studiengang an Ihrer Hochschule charakterisiert durch ...

is:

it1: (sscofopra1): ... Forschungsbezug in der Lehre?

it2: (sscofopra2): ... eine enge Verknüpfung zwischen Theorie und Praxis?

it3: (sscofopra3): ... einen engen Praxisbezug?

st:

ao1: 1: sehr wenig

ao2: 2:

ao3: 3:

ao4: 4:

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

        <zofar:transitions>
            <zofar:transition target="D2_11"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**SSCO 6**

D2_11
-------

tc:

vn: sscokli (sscokli1; sscokli2; sscokli3; sscokli4; sscokli5; sscokli6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit stimmen die folgenden Aussagen mit dem überein, was Sie in Ihrem Studiengang typischerweise erleben?

is:

It1: (sscokli1): Die Lehrenden gehen auf Schwierigkeiten der Studierenden ein.

it2: (sscokli2): Im Allgemeinen unterstützen sich die Studierenden gegenseitig.

it3: (sscokli3): Die Lehrenden sind kooperativ und aufgeschlossen.

it4: (sscokli4): Es ist üblich, dass Studierende gemeinsam für das Studium arbeiten.

it5: (sscokli5): Die Lehrenden nehmen sich Zeit, auf die Studierenden einzugehen.

it6: (sscokli6): Die Studierenden verhalten sich untereinander solidarisch.

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

tr:

        <zofar:transitions>
            <zofar:transition target="D2_12"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**SSCO 7**

D2_12
-------

tc:

vn: sscolmo (sscolmo1; sscolmo2; sscolmo3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Inwieweit beschreiben die folgenden Aussagen die Lehre in Ihrem Studiengang?

is:.

it1: (sscolmo1): Die Lehrenden stellen den Lernstoff interessant dar.

it2: (sscolmo2): Die Lehrenden vermitteln den Studierenden Freude am Fach.

it3: (sscolmo3): Die Lehrenden schaffen es, die Studierenden für das Fach zu motivieren.

st:

ao1: 1: trifft gar nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

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
            <zofar:transition target="D2_21"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**Kontakthäufigkeit**

D2_13
-------

tc:

vn: sskonth (sskonth1; sskonth2; sskonth3; sskonth4; sskonth5; sskonth6)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie häufig haben Sie im laufenden Semester *außerhalb* der Lehrveranstaltungen zu den folgenden Personen Kontakt?

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

        <zofar:transitions>
            <zofar:transition target="D2_15"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**Kontakt zu Lehrenden**

D2_15
-------

tc:

vn: sskontl (sskontl1; sskontl2; sskontl3; sskontl4)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie oft haben Sie im aktuellen Semester *außerhalb* der Lehrveranstaltungen …

is:

it1: (sskontl1): … mit Lehrenden über Ihre Karrierepläne gesprochen?

it2: (sskontl2): … mit Lehrenden zusammengearbeitet (z. B. in Kommissionen)?

it3: (sskontl3): … mit Lehrenden über fachliche Inhalte und Ideen diskutiert?

it4: (sskontl4): … mit Lehrenden über Ihre Studienleistungen gesprochen?

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
            <zofar:transition target="D2_16"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**Leistungsdruck**

D2_16
-------

tc:

vn: ssleisd (ssleisd1; ssleisd2; ssleisd3)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie beurteilen Sie im Allgemeinen die Studienanforderungen in Ihrem Studiengang …

is:

it1: (ssleisd1): … in Bezug auf den Schwierigkeitsgrad?

it2: (ssleisd2): … in Bezug auf den Umfang?

it3: (ssleisd3): … in Bezug auf die Anzahl der Prüfungen?

st:

ao1: 1: zu niedrig

ao2: 2:

ao3: 3: genau richtig

ao4: 4:

ao5: 5: zu hoch

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
            <zofar:transition target="D2_17"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**ECTS-Punkte**

D2_17
-------

tc:

vn: ssects (ssectsakt; ssectsstud)

qt: offene Angabe

hl:

in:

q: Bitte geben Sie an, wie viele ECTS-Punkte …

is:.

it:

st:

ao1: (ssectsakt): ... Sie in Ihrem aktuellen Studium bislang ungefähr erreicht haben: [Infield = ECTS-Punkte; number, 3-stellig: 0 TO 999]

ao2: (ssectsstud): ... Sie insgesamt für Ihren Studienabschluss benötigen: [Infield = ECTS-Punkte; number, 3-stellig: 0 TO 999]

mv:

ka:

vc:

av:

kh: Bitte tragen Sie die Anzahl der ECTS-Punkte ein (0 bis 999).

fv:

hv:

fo: Bitte infield-Texte noch umsetzten.

        <zofar:transitions>
            <zofar:transition target="D2_18"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**Schriftliche Leistungen**

D2_18
-------

tc:

vn: anzprkla anzprmlp anzprsau anzprabs

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie viele der folgenden Prüfungsleistungen müssen Sie im aktuellen Semester ablegen?

is: 

it1: (anzprkla): Klausuren

it2: (anzprmlp): mündliche Prüfungen

it3: (anzprsau): schriftliche Ausarbeitung (Hausarbeit, Laborbericht)

it4: (anzprabs): Abschlussarbeiten

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

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte mittig über die ao !!Anzahl der verfassten Texte!! positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D2_19"/>
        </zofar:transitions>

hi: 

**------------------------------------------------------------**

**Leseleistungen**

D2_19
-------

tc:

vn: ssread

qt: offene Angabe

hl:

in:

q: Wenn Sie an eine typische 7-Tage-Woche des laufenden Semesters denken: Wie viele Seiten lesen Sie durchschnittlich, um sich auf Lehrveranstaltungen vorzubereiten?

is:.

it:

st:

ao: (ssread): [number, 3-stellig: 0 TO 999], Postfix: Seiten pro Woche 

mv:

ka:

vc:

av:

kh: Bitte geben Sie die Anzahl gelesener Seiten pro Woche an (0 bis 999).

fv:

hv:

fo: Postfix bitte umsetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="D2_20"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**Reflective & Integrative Learning**

D2_20
-------

tc:

vn: ssrilern (ssrilern1; ssrilern2; ssrilern3; ssrilern4)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie oft haben Sie in diesem Semester …

is:.

it1: (ssrilern1): … Erlerntes mit gesellschaftlichen Problemen verknüpft?

.

it2: (ssrilern2): … unterschiedliche Perspektiven (politische, religiöse) in eine Diskussion eingebracht?

it3: (ssrilern3): … die Stärken und Schwächen des eigenen Standpunktes reflektiert?

it4: (ssrilern4): … Erkenntnisse aus Lehrveranstaltungen mit Ihren bisherigen Erfahrungen und Kenntnissen verknüpft?

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
            <zofar:transition target="A_23"/>
        </zofar:transitions>

hi:

**------------------------------------------------------------**

**Einzelbereichszufriedenheit**

D2_21
-------

tc:

vn: sszustud (sszustud1; sszustud2; sszustud3; sszustud4; sszustud5; sszustud6; sszustud7; sszustud8; sszustud9; sszustud10; sszustud11)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie – insgesamt betrachtet – mit den folgenden Aspekten Ihres Studiums?

is:

it1: (sszustud1): fachliche Kompetenz der Lehrenden

it2: (sszustud2): digitale Kompetenz der Lehrenden

it3: (sszustud3): Aufbereitung/Vermittlung des Lehrstoffs durch die Lehrenden

it4: (sszustud4): Betreuung und Beratung durch die Lehrenden

it5: (sszustud5): Klima/Atmosphäre im Studiengang

it6: (sszustud6): inhaltliche Breite/Vielfalt des Studienangebots

it7: (sszustud7): Verknüpfung von Theorie- und Praxisanteilen

it8: (sszustud8): Aufbau und Struktur des Studiengangs

it9: (sszustud9): Ihren Studienleistungen

it10: (sszustud10): Ihrem Studienfortschritt

it11: (sszustud11): Ihrem bisher erreichten Wissen und Können

st:

ao1: 1: gar nicht zufrieden

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

        <zofar:transitions>
            <zofar:transition target="A_44"/>
        </zofar:transitions>

hi:
