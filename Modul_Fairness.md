\------------------------------------------------------------

KSM-fai01 (E3 - fai0101)
=========

tc:

vn: faisoz

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in:

q: Würden Sie die sozialen Unterschiede in Deutschland ganz allgemein als klein
oder groß bezeichnen?

is:

it:

st:

ao1: 1: klein

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: groß

mv:

ka:

vc:

av:

kh:

fv:

hv:

sv: s_fairsplit = 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 (einmalige Randomisierung; 1= 10%, 2= 10 %, 3= 10%, 4= 10%, 5= 10%, 6= 10%, 7= 10%, 8= 10%, 9= 10%, 10= 10%)

fo:

tr: KSM-fai02

hi:

\------------------------------------------------------------

KSM-fai02 (E3 - fai0201)
=========

tc:

vn: faibew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in:

q: Finden Sie die sozialen Unterschiede in Deutschland im Großen und Ganzen
gerecht oder ungerecht?

is:

it:

st:

ao1: 1: ungerecht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: gerecht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai03

hi:

\------------------------------------------------------------

KSM-fai03 (E3 - fai0301)
=========

tc:

vn: faihs; faiein; faiunt

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stehen Sie zu den folgenden Aussagen?

is:

it1: (faihs): In Deutschland hat Jede\*r die gleiche Chance auf einen Hochschulabschluss.

it2: (faiein): Nur wenn die Unterschiede im Einkommen und im sozialen Ansehen groß genug sind, gibt es auch einen Anreiz für persönliche Leistungen.

it3: (faiunt): Die Wirtschaft funktioniert nur, wenn die Unternehmen gute Gewinne machen, und das kommt letzten Endes Allen zugute.

st:

ao1: 1: stimme überhaupt nicht zu

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

tr: KSM-fai04

hi:

\------------------------------------------------------------

KSM-fai04 (E3 - fai0401)
=========

tc:

vn: faians; faiint; faiorg; faiausd; faisich; faiemo; faifina; faiglü; faiprof; faielt; fainat; faiges

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stark tragen die angeführten Aspekte dazu bei, ob man im Studium erfolgreich ist?

is:

it1: (faians): eigene Anstrengung

it2: (faiint): Intelligenz, Begabung

it3: (faiorg): Organisationsfähigkeit

it4: (faiausd): Ausdrucksfähigkeit (in Wort und Schrift)

it5: (faisich): selbstsicheres Auftreten

it6: (faiemo): emotionale Unterstützung von anderen

it7: (faifina): finanzielle Unterstützung

it8: (faiglü): Zufall/Glück

it9: (faiprof): Unterstützung durch Professor\*innen

it10: (faielt): Eltern, die studiert haben

it11: (fainat): Nationalität

it12: (faiges): Geschlecht

st:

ao1: 1: gar nicht

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

tr: KSM-fai05

hi:

\------------------------------------------------------------

KSM-fai05 (E3 - fai0501)
=========

tc:

vn: faischuet; faimut; faiausl; faiprot; faimei; faians

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern stimmen Sie folgenden Aussagen zum Thema Meinungsfreiheit zu oder lehnen Sie ab?

is:

it1: (faischuet): Hochschulen sind verpflichtet, ihre Studierenden vor Äußerungen und Ideen zu schützen, die als beleidigend oder verstörend empfunden werden könnten.

it2: (faimut): An meiner Hochschule wird der freie Austausch von ganz unterschiedlichen Sichtweisen ermutigt und gefördert.

it3: (faiausl): Kontroverse Gastredner\*innen sollten wieder ausgeladen werden, wenn einige Studierende es fordern.

it4: (faiprot): Kontroverse Gastredner\*innen zu stören oder am Reden zu hindern ist eine legitime Form des Protests.

it5: (faimei): Bei kontroversen Diskussionen in Seminaren oder anderen Anlässen meiner Hochschule vermeide ich es lieber, meine ehrliche Meinung zu sagen.

it6: (faians): Die meisten Lehrenden und Studierenden an meiner Hochschule haben politische Ansichten, die meinen eigenen sehr ähnlich sind.

st:

ao1: 1: lehne völlig ab

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: stimme völlig zu 

mv: 6: kann ich nicht beurteilen

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai06 if s_fairsplit= 1
GOTO KSM-fai07 if s_fairsplit= 2
GOTO KSM-fai08 if s_fairsplit= 3
GOTO KSM-fai09 if s_fairsplit= 4
GOTO KSM-fai10 if s_fairsplit= 5
GOTO KSM-fai11 if s_fairsplit= 6
GOTO KSM-fai12 if s_fairsplit= 7
GOTO KSM-fai13 if s_fairsplit= 8
GOTO KSM-fai14 if s_fairsplit= 9
GOTO KSM-fai15 if s_fairsplit= 10

hi: Ab hier sollen die Befragten zufällig einer der Seiten KSM-fai06 - KSM-fai16 zugewiesen werden. KSM-fai06 - KSM-fai16 beinhalten dieselbe Frage, aber mit verschiedenen Fächerkombinationen (10 insgesamt, also 10 einzelne Seiten), von denen jeweils eine Fächerkombination pro Seite angezeigt werden soll. Das heißt: Jeder Befragte wird per Zufall auf eine der Seiten verwiesen. Danach werden alle auf KSM-fai16 weitergeleitet mit den Gründen für das höhere Gehalt.

\------------------------------------------------------------

KSM-fai06 (E3 - fai0601)
=========

tc:

vn: faiwige

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden. 
Absolvent\*innen wirtschaftswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 43.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen wirtschaftswissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Geisteswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai07 (E3 - fai0701)
=========

tc:

vn: faiinge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:
 
in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Geisteswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai08 (E3 - fai0801)
=========

tc:

vn: faimedge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 52.700 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Geisteswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai09 (E3 - fai0901)
=========

tc:

vn: fairecge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen rechtswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 46.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen rechtswissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Geisteswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai10 (E3 - fai1001)
=========

tc:

vn: faimedrec

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Rechtswissenschaften verdienen demgegenüber durchschnittlich ca. 46.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Rechtswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai11 (E3 - fai1101)
=========

tc:

vn: faimedin

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Ingenieurwissenschaften verdienen demgegenüber durchschnittlich ca. 47.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Ingenieurwissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai12 (E3 - fai1201)
=========

tc:

vn: faimedwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai13 (E3 - fai1301)
=========

tc:

vn: fairecwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen rechtswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 46.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen rechtswissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai14 (E3 - fai1401)
=========

tc:

vn: faiinrec

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  
Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Rechtswissenschaften verdienen demgegenüber durchschnittlich ca. 46.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Rechtswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai15 (E3 - fai1501)
=========

tc:

vn: faiinwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss _mehr_ verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

is:

it:

st:

ao1: 1: gar nicht gerechtfertigt

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: völlig gerechtfertigt

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai16

hi:

\------------------------------------------------------------

KSM-fai16 (E3 - fai1601)
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand;  faiand_open

qt: Mehrfachauswahl mit vertikaler Antwortoption und offenem Feld

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen? *Die Absolvent\*innen ...*

is: 

it:

st:

ao1: (faigefun): übernehmen eine wichtige gesellschaftliche Funktion

ao2: (faifinan): erwirtschaften hohe finanzielle Erträge

ao3: (faizeit): haben eine längere Wochenarbeitszeit

ao4: (fainive): hatten ein höheres Anforderungsniveau im Studium

ao5: (faivolk): üben eine Tätigkeit aus, die von größerer Bedeutung für die Volkswirtschaft ist

ao6: (failequal): tragen zur Sicherung der Lebensqualität in der Gesellschaft bei

ao7: (faiveran): übernehmen mehr Verantwortung im Beruf

ao8: (faikennt): verfügen über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten

ao9: (faikompl): führen komplexere Aufgaben im Beruf aus

ao10: (faiflex): haben nur geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit

ao11: (faistre): haben mehr Stress/Belastungen am Arbeitsplatz

ao12: (faiand): anderer Grund, und zwar:_____\_

ao13: (faiand_open): 

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai17

hi: 
\------------------------------------------------------------

KSM-fai17 (E3 - fai1701)
=========

tc:

vn: faidisge; faidismig; faidissoz; faidisspra; faidisrel; faidissex; faidisbeein

qt: Einfachauswahlmatrix

hl:

in:

q: Es ist nicht immer einfach, nach Abschluss des Studiums einen Job zu finden. Neben legitimen Gründen für eine Absage (z.B. Bewerberprofil passt nicht zur Stelle), kann auch Diskriminierung für die Ablehnung verantwortlich sein. 
Aus welchen Gründen wird man Ihrer Meinung nach eher abgelehnt?

is:

it1: (faidisge): aufgrund des Geschlechts

it2: (faidismig): aufgrund des Migrationshintergrunds

it3: (faidissoz): aufgrund der sozialen Herkunft

it4: (faidisspra): aufgrund der sprachlichen Ausdrucksweise (Dialekt, weniger gewandt)

it5: (faidisrel): aufgrund religiöser Zugehörigkeit

it6: (faidissex): aufgrund der sexuellen Orientierung

it7: (faidisbeein): aufgrund physischer oder psychischer Beeinträchtigung

st:

ao1: 1: nein

ao2: 2: eher nein

ao3: 3: eher ja

ao4: 4: ja

mv: -98: weiß nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-fai18

hi:

\------------------------------------------------------------

KSM-fai18 (E3 - fai1801)
=========

tc:

vn: faierlge_s/_a; faierlmig_s/_a; faierlsoz_s/_a; faierlspra_s/_a; faierlrel_s/_a; faierlsex_s/_a; faierlbeein_s/_a

qt: Mehrfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Haben Sie in Ihrem bisherigen Studium an der Hochschule schon einmal Benachteiligung/Diskriminierung selbst erlebt oder bei anderen beobachtet?

is:

it1: (faierlge): aufgrund des Geschlechts

it2: (faierlmig): aufgrund des Migrationshintergrunds

it3: (faierlsoz): aufgrund der sozialen Herkunft

it4: (faierlspra): aufgrund der sprachlichen Ausdrucksweise (Dialekt, weniger gewandt)

it5: (faierlrel): aufgrund religiöser Zugehörigkeit

it6: (faierlsex): aufgrund der sexuellen Orientierung

it7: (faierlbeein): aufgrund physischer oder psychischer Beeinträchtigung

st:

ao1: 1: (_s) selbst erlebt

ao2: 2: (_a) bei anderen beobachtet

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:GOTO A_56

hi:
