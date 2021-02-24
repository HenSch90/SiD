\--------------------------------

C2_0
====

tc: IF h_gartcount >= 1

vn: beschwer

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wirkt sich Ihre Beeinträchtigung erschwerend auf Ihr Studium aus?

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

hi:


\--------------------------------

C2_1
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: gbegrmob; gbegrseh; gbegrohr; gbegrspr; gbegrpsy; gbegrchron; gbegrtls; gbegrson; gbegrsono; gbegrka

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q1: Wie stark wirkt sich Ihre Beeinträchtigung auf Ihr aktuelles Studium aus?

q2: Wie stark wirken sich Ihre Beeinträchtigungen auf Ihr aktuelles Studium aus?

is:

it1: (gbegrmob): Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

it2: (gbegrseh): Blindheit/Sehbeeinträchtigung

it3: (gbegrohr): Gehörlosigkeit/Hörbeeinträchtigung

it4: (gbegrspr): Sprechbeeinträchtigung (z. B. Stottern)

it5: (gbegrpsy): psychische Erkrankung (z. B. Depression, Essstörung)

it6: (gbegrchron): körperliche länger dauernde/chronische Krankheit (z. B. Rheuma, MS, Darmerkrankung)

it7: (gbegrtls): Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

it8: (gbegrson): Andere Beeinträchtigung/Erkrankung, und zwar: [gbegrsono] [offenes Eingabefeld; 250 Zeichen]

it9: (gbegrka): Beeinträchtigung ohne Zuordnung

st:

ao1: 1: sehr schwach

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr stark

mv: -11: gar nicht

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

fo: mv als erste, etwa abgesetzte Spalte, danach Skala.

tr:

        <zofar:transitions>
            <zofar:transition target="C2_2"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_2
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: bedno; bedbau; bedauss; bedsich; bedruh; bedmed; bedelearn; bedpers ; bedtech; bedand

qt: Mehrfachnennung mit vertikalen ao

hl:

in:

q: Haben Sie aufgrund Ihrer Beeinträchtigung besondere Anforderungen an Bau und Ausstattung Ihrer Hochschule und/oder Bedarf an Unterstützungsangeboten?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (bedno): nein [EK]

ao2: (bedbau): bauliche Barrierefreiheit der Gebäude (z. B. Rampen, Aufzüge, barrierefreies WC, Leitsysteme)

ao3: (bedauss): spezielle technische Ausstattungen an der Hochschule (z. B. unterfahrbare Tische, Großbildschirme)

ao4: (bedsich): störungsarme Sicht-, Hör- und Belüftungsverhältnisse

ao5: (bedruh): Ruhe-/Rückzugsräume

ao6: (bedmed): barrierefrei aufbereitete Medien (z. B. Dokumente, Literatur, Webseiten)

ao7: (bedelearn): E-Learning-Angebote

ao8: (bedpers): personelle Assistenzen (z. B. Mitschreibkraft, Gebärdensprachdolmetscher\*in)

ao9: (bedtech): technische Hilfsmittel zum individuellen Gebrauch (z. B. Screen Reader, FM-Anlage)

ao10: (bedand): andere Anforderung

mv:

ka: (ao2 TO ao10): Ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo: Bitte über ao2 "Ja, und zwar:" positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="C2_3"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_2a
====

tc: IF bedbau=1 OR bedauss=1 OR bedsich=1 OR bedruh=1 OR bedmed=1 OR bedelearn=1 OR bedpers=1 OR bedtech=1 OR bedand=1

vn: erfbedbau; erfbedauss; erfbedsich; erfbedruh; erfbedmed; erfbedelearn; erfbedpers; erfbedtech ; erfbedand

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwiefern sind Ihre beeinträchtigungsbezogenen Anforderungen an Bau, Ausstattung und Unterstützung an Ihrer Hochschule erfüllt?

is:

it1: (erfbedbau): bauliche Barrierefreiheit der Gebäude (z. B. Rampen, Aufzüge, barrierefreies WC, Leitsysteme)

it2: (erfbedauss): spezielle technische Ausstattungen an der Hochschule (z. B. unterfahrbare Tische, Großbildschirme)

it3: (erfbedsich): störungsarme Sicht-, Hör- und Belüftungsverhältnisse

it4: (erfbedruh): Ruhe-/Rückzugsräume

it5: (erfbedmed): barrierefrei aufbereitete Medien (z. B. Dokumente, Literatur, Webseiten)

it6: (erfbedelearn): E-Learning-Angebote

it7: (erfbedpers): personelle Assistenzen (z. B. Mitschreibkraft, Gebärdensprachdolmetscher\*in)

it8: (erfbedtech): technische Hilfsmittel zum individuellen Gebrauch (z. B. Screen Reader, FM-Anlage)

it9: (erfbedand): andere Anforderung
 
st:

ao1: 1: gar nicht erfüllt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: voll und ganz erfüllt

mv: -12: weiß ich nicht

ka:

vc1: SHOW it1 IF bedbau=1

vc2: SHOW it2 IF bedauss=1

vc3: SHOW it3 IF bedsich=1

vc4: SHOW it4 IF bedruh=1 

vc5: SHOW it5 IF bedmed=1

vc6: SHOW it6 IF bedelearn=1

vc7: SHOW it7 IF bedpers=1 

vc8: SHOW it8 IF bedtech=1 

vc9: SHOW it9 IF bedand=1 

av:

kh:

fv:

hv:

fo: Bitte mv als letzte etwas abgesetzte Spalte.

tr:

hi:

\--------------------------------

C2_3
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: bezeit; bezeitj

qt: Einfachauswahl mit vertikalen ao; offene Angabe

hl:

in:

q: Seit wann sind Sie beeinträchtigt?

is: Sofern Ihre Beeinträchtigungen zu unterschiedlichen Zeitpunkten aufgetreten sind, beziehen Sie Ihre Antwort bitte auf die zuerst aufgetretene studienerschwerende Beeinträchtigung.

it:

st:

ao1: (bezeit): 1: seit meiner Geburt

ao2: (bezeit): 2: seit meinem [(bezeitj); 2-stellig: 1 TO 99, number; 0,5 cm]. Lebensjahr

mv:

ka:

vc: SHOW is IF h_gartcount > 1

av: 

kh: Bitte tragen Sie eine Zahl zwischen 1 und 99 ein.

fv:

hv:

fo: 

tr:

        <zofar:transitions>
            <zofar:transition target="C2_4"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_4
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: bewahr

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist für andere wahrnehmbar, dass Sie eine Beeinträchtigung haben?

is:

it:

st:

ao1: 1: nein

ao2: 2: Ja, nach einiger Zeit.

ao3: 3: Ja, bei der ersten Begegnung.

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
            <zofar:transition target="C2_5" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="C2_6" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_5
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: beausw; beauswo

qt: Einfachauswahl mit vertikalen ao; offene Angabe

hl:

in:

q: Haben Sie einen Schwerbehindertenausweis?

is:

it:

st:

ao1: (beausw): 1: Nein, habe ich nicht beantragt.

ao2: (beausw): 2: Nein, weil keine Behinderung festgestellt wurde.

ao3: (beausw): 3: Nein, weil der Grad der Behinderung niedriger als 50 eingestuft wurde.

ao4: (beausw): 4: Ja, mit einem Grad der Behinderung von [(beauswo): number, 3-stellig: 1 to 100]

mv:

ka:

vc:

av: 

kh: Bitte tragen Sie den Grad der festgestellten Behinderung ein (1 bis 100).

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="C2_7"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_7
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: schwleist; schwwieei; schwanwes; schwlv; schwselbst; schwgrup; schwflex; schwdicht; schwwieho; schwdauer; schwprart; schwprbed; schwno

qt: Mehrfachauswahl mit vertikalen ao und mit Überkategorien/Zwischenüberschriften

hl:

in:

q: Wenn Sie an Ihr Studium denken: Was bereitet oder bereitete Ihnen im Zusammenhang mit Ihrer Beeinträchtigung Schwierigkeiten?

is: Bitte denken Sie dabei auch an Schwierigkeiten, die – z. B. durch einen Nachteilsausgleich oder individuelle Absprachen – bereits ausgeglichen wurden. Bitte alles Zutreffende auswählen.

it:

st:

ao1: (schwleist): Leistungspensum/festgelegte Studienordnung

ao2: (schwwieei): Wiedereinstieg ins Studium (z. B. nach Klinikaufenthalten)

ao3: (schwanwes): Anwesenheitspflicht

ao4: (schwlv): Gestaltung von Lehrveranstaltungen (Medien, Methoden, Interaktionsformen)

ao5: (schwselbst): Selbstlernphasen (z. B. Aufbereitung der Lernmaterialien)

ao6: (schwgrup): Gruppen-/Teamarbeiten (z. B. Terminkoordination, Kommunikation)

ao7: (schwflex): mangelnde Flexibilität der Lehrenden

ao8: (schwdicht): Prüfungsdichte

ao9: (schwwieho): Wiederholung/Verschiebung von Prüfungen

ao10: (schwdauer): Prüfungsdauer/Abgabefristen

ao11: (schwprart): Prüfungsart

ao12: (schwprbed): Prüfungsbedingungen

ao13: (schwno): Ich habe und hatte keine Schwierigkeiten. [EK]

mv:

ka1: (ao1 TO ao3): !!Studienorganisation!!

ka2: (ao4 TO ao7): !!Lehre und Lernen!!

ka3: (ao8 TO ao12): !!Prüfungen/Leistungsnachweise!!

vc:

av:

kh:

fv:

hv:

fo1: "Studienorganisation" in fett über ao1 platzieren; "Lehre und Lernen" in fett über ao4 platzieren; "Prüfungen/Leistungsnachweise" in fett über ao8 platzieren. 

fo2: schwno/"Ich habe und hatte keine Schwierigkeiten." als EK absetzen

tr:

        <zofar:transitions>
            <zofar:transition target="C2_8"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_8
====

tc: IF schwleist=1 OR schwwieei=1 OR schwanwes=1 OR schwlv=1 OR schwselbst=1 OR schwgrup=1 OR schwflex=1 OR schwdicht=1 OR schwwieho=1 OR schwdauer=1 OR schwprart=1 

vn: ntaleist; ntawieei; ntaanwes; ntalv; ntaselbst; ntagrup; ntaflex; ntadicht; ntawieho; ntadauer; ntaprart; ntaprbed

qt: Einfachauswahlmatrix mit horizontalen ao und mit Überkategorien/Zwischenüberschriften

hl:

in:

q: Haben Sie in den von Ihnen benannten Bereichen um individuelle Anpassungen gebeten oder Nachteilsausgleiche beantragt? Und wurden diese bewilligt?

is: Wenn Schwierigkeiten häufiger aufgetreten sind, beziehen Sie sich bitte auf die letzte Situation. Bitte berücksichtigen Sie sowohl formale Antragstellungen als auch informelle Absprachen.

it1: (ntaleist): Leistungspensum/festgelegte Studienordnung

it2: (ntawieei): Wiedereinstieg ins Studium (z. B. nach Klinikaufenthalten)

it3: (ntaanwes): Anwesenheitspflicht

it4: (ntalv): Gestaltung von Lehrveranstaltungen (Medien, Methoden, Interaktionsformen)

it5: (ntaselbst): Selbstlernphasen (z. B. Aufbereitung der Lernmaterialien)

it6: (ntagrup): Gruppen-/Teamarbeiten (z. B. Terminkoordination, Kommunikation)

it7: (ntaflex): mangelnde Flexibilität der Lehrenden

it8: (ntadicht): Prüfungsdichte

it9: (ntawieho): Wiederholung/Verschiebung von Prüfungen

it10: (ntadauer): Prüfungsdauer/Abgabefristen

it11: (ntaprart): Prüfungsart

it12: (ntaprbed): Prüfungsbedingungen

st:

ao1: 1: beantragt und bewilligt

ao2: 2: beantragt, aber nicht bewilligt

ao3: 3: nicht beantragt

mv:

ka1: (it1 TO it3): !!Studienorganisation!!

ka2: (it4 TO it7): !!Lehre und Lernen!!

ka3: (it8 TO it11): !!Prüfungen/Leistungsnachweise!!

vc1: SHOW it1 IF schwleist=1

vc2: SHOW it2 IF schwwieei=1

vc3: SHOW it3 IF schwanwes=1

vc4: SHOW it4 IF schwlv=1 

vc5: SHOW it5 IF schwselbst=1

vc6: SHOW it6 IF schwgrup=1

vc7: SHOW it7 IF schwflex=1 

vc8: SHOW it8 IF schwdicht=1 

vc9: SHOW it9 IF schwwieho=1 

vc10: SHOW it10 IF schwdauer=1 

vc11: SHOW it11 IF schwprart=1 

vc12: SHOW it12 IF schwprbed=1

vc:

av:

kh:

fv:

hv:

fo: "Studienorganisation" in fett über ao1 platzieren; "Lehre und Lernen" in fett über ao4 platzieren; "Prüfungen/Leistungsnachweise" in fett über ao8 platzieren. 

tr:

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




tc: IF ntaleist=1 OR ntawieei=1 OR ntaanwes=1 OR ntalv=1 OR ntaselbst=1 OR ntagrup=1 OR ntaflex=1 OR ntadicht=1 OR ntawieho=1 OR ntadauer=1 OR ntaprart=1

vn: hilfleist; hilfwieei; hilfanwes; hilflv; hilfselbst; hilfgrup; hilfflex; hilfdicht; hilfwieho; hilfdauer; hilfprart

qt: Einfachauswahlmatrix mit horizontalen ao und mit Überkategorien/Zwischenüberschriften

hl:

in:

q: Wie hilfreich waren die zuletzt verabredeten individuellen Anpassungen/Nachteilsausgleiche?

is:

it1: (hilfleist): Leistungspensum/festgelegte Studienordnung

it2: (hilfwieei): Wiedereinstieg ins Studium (z. B. nach Klinikaufenthalten)

it3: (hilfanwes): Anwesenheitspflicht

it4: (hilflv): Gestaltung von Lehrveranstaltungen (Medien, Methoden, Interaktionsformen)

it5: (hilfselbst): Selbstlernphasen (z. B. Aufbereitung der Lernmaterialien)

it6: (hilfgrup): Gruppen-/Teamarbeiten (z. B. Terminkoordination, Kommunikation)

it7: (hilfflex): mangelnde Flexibilität der Lehrenden

it8: (hilfdicht): Prüfungsdichte

it9: (hilfwieho): Wiederholung/Verschiebung von Prüfungen

it10: (hilfdauer): Prüfungsdauer/Abgabefristen

it11: (hilfprart): Prüfungsart

it12: (hilfprbed): Prüfungsbedingungen

st:

ao1: 1: gar nicht hilfreich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr hilfreich

ka1: (it1 TO it3): !!Studienorganisation!!

ka2: (it4 TO it7): !!Lehre und Lernen!!

ka3: (it8 TO it11): !!Prüfungen/Leistungsnachweise!!

vc1: SHOW it1 IF ntaleist=1

vc2: SHOW it2 IF ntawieei=1

vc3: SHOW it3 IF ntaanwes=1

vc4: SHOW it4 IF ntalv=1

vc5: SHOW it5 IF ntaselbst=1

vc6: SHOW it6 IF ntagrup=1

vc7: SHOW it7 IF ntaflex=1

vc8: SHOW it8 IF ntadicht=1

vc9: SHOW it9 IF ntawieho=1

vc10: SHOW it10 IF ntadauer=1

vc11: SHOW it11 IF ntaprart=1

vc12: SHO it12 IF ntaprbed=1

av:

kh:

fv:

hv:

fo: "Studienorganisation" in fett über ao1 platzieren; "Lehre und Lernen" in fett über ao4 platzieren; "Prüfungen/Leistungsnachweise" in fett über ao8 platzieren. 

tr:

        <zofar:transitions>
            <zofar:transition target="C2_11" condition="zofar.asNumber(ntabau)==3 or zofar.asNumber(ntaorg)==3 or zofar.asNumber(ntapru)==3 or zofar.asNumber(ntaand)==3"/>
            <zofar:transition target="C2_12"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_10
=====

tc: IF ntaleist=3 AND ntawieei=3 AND ntaanwes=3 AND ntalv=3 AND ntaselbst=3 AND ntagrup=3 AND ntaflex=3 AND ntadicht=3 AND ntawieho=3 AND ntadauer=3 AND ntaprart=3

vn: nbkenn; nbfueh; nbunbek; nbextra; nblast; nbhemm; nbsecr; nbwen; nbaufw; nberlo; nbaend; nbnach
 
qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Weshalb haben Sie trotz Ihrer beeinträchtigungsbezogenen Schwierigkeiten nicht um individuelle Anpassungen gebeten bzw. keine Nachteilsausgleiche beantragt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (nbkenn): Ich bin nicht sicher, ob ich anspruchsberechtigt bin oder mein Antrag Chancen hat.

ao2: (nbfueh): Ich fühle mich nicht beeinträchtigt genug.

ao3: (nbunbek): Die Möglichkeit war mir nicht bekannt.

ao4: (nbextra): Ich will nicht bevorzugt behandelt werden.

ao5: (nblast): Ich möchte niemandem zur Last fallen.

ao6: (nbhemm): Ich hatte Hemmungen, mich an jemanden zu wenden.

ao7: (nbsecr): Ich wollte meine Beeinträchtigung nicht preisgeben.

ao8: (nbwen): Ich wusste nicht, wen ich um Unterstützung/Beratung hätte bitten können.

ao9: (nbaufw): Es wäre zu viel Aufwand gewesen.

ao10: (nberlo): Weil ich mich früher schon erfolglos darum bemüht habe.

ao11: (nbaend): Ich glaube nicht, dass sich meine Situation ändern lässt.

ao12: (nbnach): Weil ich dadurch Nachteile im weiteren Studium befürchtet habe.

mv:

ka:

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="C2_12"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_11
=====

tc: IF ntaleist=2 OR ntawieei=2 OR ntaanwes=2 OR ntalv=2 OR ntaselbst=2 OR ntagrup=2 OR ntaflex=2 OR ntadicht=2 OR ntawieho=2 OR ntadauer=2 OR ntaprart=2

vn: kbgrund; kbordn; kbwert; kbbev; kblehr; kbtech; kborga; kbatt; kbzeit; kbmem

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Weshalb wurden Ihre beantragten Nachteilsausgleiche bzw. individuellen Anpassungswünsche nicht bewilligt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (kbgrund): Meine Beeinträchtigung wurde nicht als Grund akzeptiert.

ao2: (kbordn): Anpassungswünsche/Nachteilsausgleiche wurden als nicht vereinbar mit der Prüfungsordnung angesehen.

ao3: (kbwert): Ersatzleistung wurde nicht als gleichwertig angesehen.

ao4: (kbbev): Anpassungswünsche/Nachteilsausgleiche wurden als Bevorzugung angesehen.

ao5: (kblehr): Lehrende\*r war nicht dazu bereit, Lehrroutinen zu ändern.

ao6: (kbtech): Aufgrund technischer Probleme (z. B. fehlende Ausstattung).

ao7: (kborga): Aufgrund organisatorischer Probleme (z. B. keine Raum- oder Prüfungsverlegung möglich).

ao8: (kbatt): Aufgrund fehlender Nachweise (z. B. fachärztliches Attest, Schwerbehindertenausweis).

ao9: (kbzeit): Anpassungswünsche/Nachteilsausgleiche wurden zu spät beantragt.

ao10: (kbmem): Wurde mir nicht mitgeteilt. [EK]

mv:

ka:

av:

kh:

fv:

hv:





fo: ao10: (kbmem): Wurde mir nicht mitgeteilt. als EK absetzen

tr:

        <zofar:transitions>
            <zofar:transition target="C2_12"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_11a
====

tc: IF h_gartcount >= 1 & beschwer=2

vn: bsuntkom; bsuntleh; bsuntfre; bsuntfam; bsuntaer; bsuntber

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Inwiefern werden Sie in Bezug auf Ihre beeinträchtigungsbedingten Schwierigkeiten unterstützt durch …

is:

it1: (bsuntkom): … Kommiliton\*innen?

it2: (bsuntleh): … Lehrende?

it3: (bsuntfre): … Freund\*innen/Bekannte?

it4: (bsuntfam): … Familienangehörige?

it5: (bsuntaer): … Ärzt\*innen/Therapeut\*innen?

it6: (bsuntber): … Beratungen/Coachings/Workshops?

st:

ao1: 1: überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: voll und ganz

mv: -11: nicht vorhanden

ka:

vc:

av:

kh:

fv:

hv:





fo1: mv/"nicht vorhanden" bitte als erste etwas abgesetzte Spalte platzieren (quasi links von der Spalte "überhaupt nicht").

fo2: Bitte in der Zeile der Kommiliton\*innen (it1: bsuntkom) und Lehrende (it2: bsuntleh) jeweils das Antwortkästchen für mv/"nicht vorhanden" nicht einblenden.

tr:

hi:

\--------------------------------

C2_12
=====

tc: IF h_gartcount >= 1 & beschwer=2

vn: beauftr; besoz; bepsy; bestud; beselb; beand

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Welche speziellen Anlaufstellen für eine persönliche Beratung zum Thema Studium und Beeinträchtigung kennen Sie bzw. haben Sie genutzt?

is:

it1: (beauftr): Beratungsstellen für Studierende mit Beeinträchtigungen der Hochschule

it2: (besoz): Beratungsstelle für Studierende mit Beeinträchtigungen des Studentenwerks

it3: (bepsy): psychologische Beratungsstelle des Studentenwerks/der Hochschule

it4: (bestud): Beratung für Studierende mit Beeinträchtigungen des AStA, StuRa, UStA etc.

it5: (beselb): studentische Behindertenselbsthilfe (u. a. BHSA, DVBS)

it6: (beand): studienbezogene Beratung anderer Selbsthilfevereinigungen

st:

ao1: 1: kenne ich nicht

ao2: 2: kenne ich, aber nicht genutzt

ao3: 3: habe ich genutzt

mv: -11: nicht vorhanden

ka:

vc:

av:

kh:

fv:

hv:

fo: mv/"nicht vorhanden" bitte als erste etwas abgesetzte Spalte platzieren (quasi links von der Spalte "kenne ich nicht").

tr:

        <zofar:transitions>
            <zofar:transition target="C2_13" condition="zofar.asNumber(beauftr)==3 or zofar.asNumber(besoz)==3 or zofar.asNumber(bepsy)==3 or zofar.asNumber(bestud)==3              or zofar.asNumber(beselb)==3 or zofar.asNumber(beand)==3"/>
            <zofar:transition target="A_16"/>
        </zofar:transitions>

hi:

\--------------------------------

C2_13
=====




tc: IF beauftr = 3 OR besoz = 3 OR bepsy = 3 OR bestud = 3 OR beselb = 3 OR beand = 3

vn: behauftr; behsoz; behpsy; behstud; behselb; behand

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie hilfreich waren diese Angebote für Sie?

is:

it1: (behauftr): Beratungsstellen für Studierende mit Beeinträchtigungen der Hochschule

it2: (behsoz): Beratungsstelle für Studierende mit Beeinträchtigungen des Studentenwerks

it3: (behpsy): psychologische Beratungsstelle des Studentenwerks/der Hochschule

it4: (behstud): Beratung für Studierende mit Beeinträchtigungen des AStA, StuRa, UStA etc.

it5: (behselb): studentische Behindertenselbsthilfe (u. a. BHSA, DVBS)

it6: (behand): studienbezogene Beratung anderer Selbsthilfevereinigungen

st:

ao1: 1: gar nicht hilfreich

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr hilfreich

mv:

ka:

vc1: SHOW it1 IF beauftr =3

vc2: SHOW it2 IF besoz =3

vc3: SHOW it3 IF bepsy =3

vc4: SHOW it4 IF bestud =3

vc5: SHOW it5 IF beselb =3

vc6: SHOW it6 IF beand =3

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_16"/>
        </zofar:transitions>

hi:


\--------------------------------

C2_14
=====

tc: IF h_gartcount >= 1 & beschwer=2

vn: belehrver; besoersch; bekomoff

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium mit Beeinträchtigung zu?

is:

it1: (belehrver): Die Lehrenden meines Studiengangs haben Verständnis für die Situation von Studierenden mit Beeinträchtigung.

it2: (besoersch): Die  Studienorganisation/-ordnung erschwert das Studieren mit Beeinträchtigung.

it3: (bekomoff): Mit meinen Kommiliton\*innen kann ich offen über meine beeinträchtigungsbedingten Schwierigkeiten im Studium sprechen.

st:

ao1: 1: trifft überhaupt nicht zu

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

hi:
