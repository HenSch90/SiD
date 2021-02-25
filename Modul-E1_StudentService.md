\--------------------------------

E1_0 
====

tc: wohnfo = 4 | 5 | 6 | 7

vn: stuwotrae

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: In welcher Trägerschaft ist das Studierendenwohnheim, in dem Sie wohnen?

is:

it:

st:

ao1: 1: Studierendenwerk/Studentenwerk

ao2: 2: andere gemeinnützige Trägerschaft (z. B. kirchliche)

ao2: 2: private Trägerschaft

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" bitte etwas absetzen.

tr:

hi:

\--------------------------------

E1_1
====

tc:

vn: moftfrue; moftvorm; moftmitt; moftnach; moftaben

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig gehen Sie im Laufe einer für Sie typischen Woche zum Essen in eine Mensa oder Cafeteria Ihrer Hochschule?

is:

it1: (moftfrue): zum Frühstück (07:00 - 09:00 Uhr)

it2: (moftvorm): zu einer Zwischenmahlzeit am Vormittag (09:00 - 11:30 Uhr)

it3: (moftmitt): zum Mittagessen (11:30 - 14:30 Uhr)

it4: (moftnach): zu einer Zwischenmahlzeit am Nachmittag (14:30 - 17:00 Uhr)

it5: (moftaben): zum Abendessen (17:00 - 20:00 Uhr)

st:

ao1: 0: 0-mal

ao2: 1: 1-mal

ao3: 2: 2-mal

ao4: 3: 3-mal

ao5: 4: 4-mal

ao6: 5: 5-mal

ao7: 6: 6-mal

ao8: 7: 7-mal

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
            <zofar:transition target="E1_2"/>
        </zofar:transitions>

hi:


\--------------------------------

E1_2
====

tc:

vn: mzufges; mzufqual; mzufausw; mzufprl; mzufpraes; mzufatmo; 
mzufsitz; mzuflage; mzufwart; mzufserv; mzufverl; mzufoeff; mzufkomm;
mzufbarf; mzufkind

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie zufrieden sind Sie mit Ihrer Mensa/Cafeteria hinsichtlich der folgenden Aspekte?

is:

it1: (mzufges): Geschmack und Frische

it2: (mzufqual): Ernährungsqualität und Gesundheitswerte

it3: (mzufausw): Auswahl- und Kombinationsmöglichkeiten

it4: (mzufprl): Preis-Leistungs-Verhältnis

it5: (mzufpraes): Präsentation des Essensangebots

it6: (mzufatmo): Atmosphäre und Raumgestaltung

it7: (mzufsitz): Verfügbarkeit von Sitzplätzen

it8: (mzuflage): Lage und Erreichbarkeit

it9: (mzufwart): Wartezeiten

it10: (mzufserv): Service

it11: (mzufverl): zeitliche Vereinbarkeit mit Lehr-/Veranstaltungsplan

it12: (mzufoeff): Öffnungszeiten

it13: (mzufkomm): Ort der Kommunikation

it14: (mzufbarf): Barrierefreiheit

it15: (mzufkind): Kinderfreundlichkeit

st:

ao1: 1: gar nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr zufrieden

mv:

ka:

vc1: SHOW it14 IF h_gartcount >= 1

vc2: SHOW it15 IF dkinja = 2

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="E1_3"/>
        </zofar:transitions>

hi:


\--------------------------------

E1_3
====

tc:

vn: indergenu; indersatt; inderprei; inderwich; inderplan; inderzuha; 
inderprob; inderschn; inderunwe; inderkoch; indergese

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Nun geht es um Ihre Einstellung zum Thema Essen: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1: (indergenu): Essen hat für mich vor allem mit Genuss zu tun.

it2: (indersatt): Essen muss vor allem satt machen.

it3: (inderprei): Mein Essen muss preiswert sein.

it4: (inderwich): Meine Ernährung ist mir wichtig.

it5: (inderplan): Ich orientiere mich an einem Ernährungsplan.

it6: (inderzuha): Ich ernähre mich so, wie ich es von Zuhause gewöhnt bin.

it7: (inderprob): Ich probiere gerne Speisen aus anderen Kulturkreisen aus.

it8: (inderschn): Mein Essen muss schnell zubereitet sein.

it9: (inderunwe): Ich esse häufig unterwegs (to go).

it10: (inderkoch): Meistens koche ich mein Essen selbst.

it11: (indergese): Ich esse am liebsten in geselliger Runde.

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
            <zofar:transition target="E1_4"/>
        </zofar:transitions>

hi:


\--------------------------------

E1_3a
====

tc:

vn: inderflei; inderfisch; indervege; indervega; inderoeko; inderfair; inderregi; inderzuck; inderkalo; inderfris

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Nun geht es um Ihr allgemeines Ernährungsverhalten: Inwieweit treffen die folgenden Aussagen auf Ihre persönliche Ernährung zu?

is:

it1: (inderflei): Fleisch gehört für mich zum Essen dazu.

it2: (inderfisch): Fisch gehört für mich zum Essen dazu.

it3: (indervege): Ich ernähre mich vegetarisch.

it4: (indervega): Ich ernähre mich vegan.

it5: (inderoeko): Ich achte bei Lebensmitteln darauf, dass sie EU-Öko-/Bio-zertifiziert sind.

it6: (inderfair): Ich achte darauf, dass Lebensmittel fair gehandelt sind.

it7: (inderregi): Ich konsumiere vor allem regionale/saisonale Lebensmittel.

it8: (inderzuck): Ich versuche, den Konsum von Zucker zu vermeiden.

it9: (inderkalo): Beim Essen achte ich darauf, wie viele Kalorien ich zu mir nehme.

it10: (inderfris): Ich koche vor allem mit frischen Lebensmitteln.

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

hi:


\--------------------------------

E1_6
===
tc:

vn: ibedsfin; ibedfinbs; ibedfinwo; ibedkv; ibedafin; ibedpart; ibedfamu; ibeddep; ibedsuch; ibedvbew;
ibedvbki; ibedvbhc; ibedllpran; ibedaoz; ibedabersw; ibedaorg; ibedabs; ibebsln; ibebssu;

qt: Einfachauswahlmatrix/5er-Skala mit Zwischenüberschriften und horizontalen ao

hl:

in:

q: Inwieweit hatten Sie in den letzten zwölf Monaten Fragen bis hin zu Schwierigkeiten hinsichtlich folgender Themen?

is:

it1: (ibedsfin): Finanzierung des Studiums

it2: (ibedfinbs): Finanzierungsfragen im Zusammenhang mit meiner Beeinträchtigung

it3: (ibedfinwo): Finanzierung der Wohnung

it4: (ibedkv): Krankenversicherung

it5: (ibedafin): Finanzierung eines studienbezogenen Auslandsaufenthalts

it6: (ibedpart): Partnerschaftsprobleme

it7: (ibedfamu): Probleme im familiären Umfeld

it8: (ibeddep): depressive Verstimmungen

it9: (ibedsuch): Suchtprobleme

it10: (ibedvbew): Vereinbarkeit von Studium und Erwerbstätigkeit

it11: (ibedvbki): Vereinbarkeit von Studium und Kind

it12: (ibedvbhc): Vereinbarkeit von Studium und Behinderung/chronischer Krankheit

it13: (ibedllpran): Lern-/Leistungsprobleme, Prüfungsangst

it14: (ibedaoz): Arbeitsorganisation, Zeitmanagement

it15: (ibedabersw): Studienorganisation, Studienganggestaltung/-wechsel

it16: (ibedaorg): Organisation eines studienbezogenen Auslandsaufenthalts

it17: (ibedabs): Studienabschlussprobleme

it18: (ibebsln): Nachteilsausgleiche in Studium und Prüfungen

it19: (ibebssu): Umgang mit längeren beeinträchtigungsbedingten Studienunterbrechungen

st:

ao1: 1: gar nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: in hohem Maße

mv: 

ka1: (it1 TO it5): !!finanzierungsbezogene Themen!!

ka2: (it6 TO it9): !!persönliche Themen!!

ka3: (it10 TO it19): !!studienbezogene Themen!!

vc1: SHOW it2, it12, it18, it19 IF h_gartcount >= 1

vc2: SHOW it6 IF demofam = 2 | 3

vc3: SHOW it10 IF eaktsens = 2 | 3 | 4

vc4: SHOW it11 IF dkinja = 2

av:

kh:

fv:

hv:

fo1: Bitte über it1 "finanzierungsbezogene Themen" linksbündig positionieren.

fo2: Bitte über it6 "persönliche Themen" linksbündig positionieren.

fo3: Bitte über it10 "studienbezogene Themen" linksbündig positionieren.

tr: 

        <zofar:transitions>
            <zofar:transition target="E1_7" condition="(zofar.asNumber(ibedsfin) gt 1         or zofar.asNumber (ibedkv) gt 1         or zofar.asNumber (ibedafin) gt 1         or zofar.asNumber (ibedpart) gt 1         or zofar.asNumber (ibedfamu) gt 1         or zofar.asNumber (ibeddep) gt 1         or zofar.asNumber (ibedaldr) gt 1         or zofar.asNumber (ibedvbew) gt 1         or zofar.asNumber (ibedvbki) gt 1         or zofar.asNumber (ibedvbhc) gt 1         or zofar.asNumber (ibedllpran) gt 1         or zofar.asNumber (ibedaoz) gt 1         or zofar.asNumber (ibedabersw) gt 1         or zofar.asNumber (ibedaorg) gt 1         or zofar.asNumber (ibedabs) gt 1         or zofar.asNumber (ibebsln) gt 1         or zofar.asNumber (ibebssu) gt 1         or zofar.asNumber (ibebsth) gt 1         or zofar.asNumber (ibebspa) gt 1         or zofar.asNumber (ibebsbh) gt 1         or zofar.asNumber (ibebsat) gt 1         or zofar.asNumber (ibebsrb) gt 1         or zofar.asNumber (ibedno) gt 1)"/>
            <zofar:transition target="E1_8"/>
        </zofar:transitions>

hi:


\--------------------------------

E1_7
====

tc: ibedsfin > 1 OR ibedfinbs > 1 OR ibedfinwo > 1 OR ibedkv > 1 OR ibedafin > 1 OR ibedpart > 1 OR ibedfamu > 1 OR ibeddep > 1 OR ibedsuch > 1 OR ibedvbew > 1 OR ibedvbki > 1 OR ibedvbhc > 1 OR ibedllpran > 1 OR ibedaoz > 1 OR ibedabersw > 1 OR ibedaorg > 1 OR ibedabs > 1 OR ibebsln > 1 OR ibebssu > 1 

vn: iinasfin; iinafinbs; iinafinwo; iinakv; iinaafin; iinapart; iinafamu; iinadep; iinasuch;
iinavbew; iinavbki; iinavbhc; iinallpran; iinaaoz; iinaabersw; iinaaorg; iinaabs; innabsln; iinabssu;
iinano;

qt: Einfachauswahlmatrix mit Zwischenüberschriften und horizontalen ao

hl:

in:

q: Haben Sie zu den zuvor genannten Themen in den letzten zwölf Monaten Beratung in Anspruch genommen?

is:

it1: (iinasfin): Finanzierung des Studiums

it2: (iinafinbs): Finanzierungsfragen im Zusammenhang mit meiner Beeinträchtigung 

it3: (iinafinwo): Finanzierung der Wohnung 

it4: (iinakv): Krankenversicherung

it5: (iinaafin): Finanzierung eines studienbezogenen Auslandsaufenthalts

it6: (iinapart): Partnerschaftsprobleme

it7: (iinafamu): Probleme im familiären Umfeld

it8: (iinadep): depressive Verstimmungen

it9: (iinasuch): Suchtprobleme

it10: (iinavbew): Vereinbarkeit von Studium und Erwerbstätigkeit

it11: (iinavbki): Vereinbarkeit von Studium und Kind

it12: (iinavbhc): Vereinbarkeit von Studium und Behinderung/chronischer Krankheit

it13: (iinallpran): Lern-/Leistungsprobleme, Prüfungsangst

it14: (iinaaoz): Arbeitsorganisation, Zeitmanagement

it15: (iinaabersw): Studienorganisation, Studienganggestaltung/-wechsel

it16: (iinaaorg): Organisation eines studienbezogenen Auslandsaufenthalts

it17: (iinaabs): Studienabschlussprobleme

it18: (innabsln): Nachteilsausgleiche in Studium und Prüfungen

it19: (iinabssu): Umgang mit längeren beeinträchtigungsbedingten Studienunterbrechungen

st:

ao1: 1: nein

ao2: 2: ja, innerhalb des Hochschulbereichs

ao3: 3: ja, außerhalb des Hochschulbereichs

ao4: 4: ja, innerhalb und außerhalb des Hochschulbereichs

mv:

ka1: (it1 TO it5): !!finanzierungsbezogene Themen!!

ka2: (it6 TO it9): !!persönliche Themen!!

ka3: (it10 TO it19): !!studienbezogene Themen!!

vc1: SHOW it1 IF ibedsfin > 1

vc2: SHOW it2 IF ibedfinbs > 1

vc3: SHOW it3 IF ibedfinwo > 1

vc4: SHOW it4 IF ibedkv > 1

vc5: SHOW it5 IF ibedafin > 1

vc6: SHOW it6 IF ibedpart > 1

vc7: SHOW it7 IF ibedfamu > 1

vc8: SHOW it8 IF ibeddep > 1

vc9: SHOW it9 IF ibedsuch > 1

vc10: SHOW it10 IF ibedvbew > 1

vc11: SHOW it11 IF ibedvbki > 1

vc12: SHOW it12 IF ibedvbhc > 1

vc13: SHOW it13 IF ibedllpran > 1

vc14: SHOW it14 IF ibedaoz > 1

vc15: SHOW it15 IF ibedabersw > 1

vc16: SHOW it16 IF ibedaorg > 1

vc17: SHOW it17 IF ibedabs > 1

vc18: SHOW it18 IF ibebsln > 1

vc19: SHOW it19 IF ibebssu > 1

av:

kh:

fv:

hv:

fo1: Bitte über it1 "finanzierungsbezogene Themen" linksbündig positionieren.

fo2: Bitte über it6 "persönliche Themen" linksbündig positionieren.

fo3: Bitte über it10 "studienbezogene Themen" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="E1_8"/>
        </zofar:transitions>
    
hi: Bitte Systemvariable "iinano" mit den folgenden Werten anlegen:
iinano = 0, wenn mind. ein Item/eine Variable auf E1_7 > 1 ist.
iinano = 1, wenn alle **angezeigten** Items/Variablen auf E1_7 = 1 sind.


\--------------------------------

E1_8
====

tc: IF iinano = 1

vn: ihinzeit; ihinaufw; ihingel; ihinkan; ihinpre; ihinfreu; ihinhil; ihinhem; ihinnac; ihinand

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Warum haben Sie kein Beratungsangebot in Anspruch genommen?

is: Bitte alles Zutreffende auswählen.

it1: (ihinzeit): ... ich keine Zeit dafür hatte.

it2: (ihinaufw): ... der Aufwand zu groß erschien.

it3: (ihingel): ... sich das Problem von alleine gelöst hat.

it4: (ihinkan): ... ich kein passendes Angebot gefunden habe.

it5: (ihinpre): ... ich mein Problem nicht preisgeben wollte.

it6: (ihinfreu): ... ich im privaten Umfeld Unterstützung gefunden habe.

it7: (ihinhil): ... ich nicht wusste, wen ich um Beratung hätte bitten können.

it8: (ihinhem): ... ich Hemmungen hatte, Hilfe in Anspruch zu nehmen.

it9: (ihinnac): ... ich dadurch Nachteile im weiteren Studium befürchtete.

it10: (ihinand): ... aus anderen Gründen.

st: 

ao:

mv:

ka: (it1 TO it10): !!Ich habe kein Beratungsangebot in Anspruch genommen, weil …!!

vc:

av:

kh:

fv:

hv:

fo: Bitte über it1 "Ich habe kein Beratungsangebot in Anspruch genommen, weil …" linksbündig positionieren.

tr:

        <zofar:transitions>
            <zofar:transition target="E1_9"/>
        </zofar:transitions>

hi:


\--------------------------------

E1_11
=====

tc:

vn: infoauvo; infofopr; infohosp; infostve; infopaho; infohole

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie gut informiert sind Sie über die folgenden Bereiche Ihrer Hochschule?

is:

it1: (infoauvo): außercurriculare Vortragsreihen (z. B. Studium generale)

it2: (Infofopr): Forschungsschwerpunkte Ihrer Professor\*innen

it3: (infohosp): Programm des Hochschulsports

it4: (infostve): politische Zusammensetzung der gegenwärtigen Studierendenvertretung

it5: (infopaho): Partys auf dem Hochschulcampus

if6: (infohole): Aufgaben der Hochschulleitung

st:

ao1: 1: gar nicht informiert

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut informiert

mv: -11: interessiert mich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: mv/"interessiert mich nicht" bitte etwas absetzen.

tr:

        <zofar:transitions>
            <zofar:transition target="A_56"/>
        </zofar:transitions>

hi: 

\--------------------------------
