\------------------------------------------------------------

KSM-fai01
=========

tc:

vn: faisoz

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Fragen zur sozialen Gerechtigkeit an der Hochschule und innerhalb der Gesellschaft. Dabei geht es nicht um richtig oder falsch, sondern um Ihre persönliche Meinung. Bitte lesen Sie dazu die Aussagen aufmerksam durch.

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

tr: GOTO KSM-fai02

hi:


\------------------------------------------------------------

KSM-fai02 
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

ao1: 1: gerecht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: ungerecht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai03

hi:


\------------------------------------------------------------

KSM-fai03 
=========

tc:

vn: faihs; faiein; faiunt

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stehen Sie zu den folgenden Aussagen?

is:

it1: (faihs): In Deutschland hat jede\*r die gleiche Chance auf einen Hochschulabschluss.

it2: (faiein): Nur wenn die Unterschiede im Einkommen und im sozialen Ansehen groß genug sind, gibt es auch einen Anreiz für persönliche Leistungen.

it3: (faiunt): Die Wirtschaft funktioniert nur, wenn die Unternehmen hohe Gewinne machen, und das kommt letzten Endes allen zugute.

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

tr: GOTO KSM-fai04

hi:


\------------------------------------------------------------

KSM-fai04 
=========

tc:

vn: faians; faiint; faiorg; faiausd; faisich; faiemo; faifina; faiglue; faiprof; faielt; fainat; faiges

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stark tragen, Ihrer Einschätzung nach, die angeführten Aspekte dazu bei, ob man im Studium erfolgreich ist?

is:

it1: (faians): eigene Anstrengung

it2: (faiint): Intelligenz, Begabung

it3: (faiorg): Organisationsfähigkeit

it4: (faiausd): Ausdrucksfähigkeit (in Wort und Schrift)

it5: (faisich): selbstsicheres Auftreten

it6: (faiemo): emotionale Unterstützung von anderen

it7: (faifina): finanzielle Unterstützung

it8: (faiglue): Zufall/Glück

it9: (faiprof): fachliche Unterstützung durch Professor\*innen

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

tr: GOTO KSM-fai05

hi: Reihenfolge der Items randomisieren.


\------------------------------------------------------------

KSM-fai05 
=========

tc:

vn: faischuet; faimut; faiausl; faiprot; faimei; faians1

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern stimmen Sie folgenden Aussagen zum Thema Meinungsfreiheit zu?

is:

it1: (faischuet): Hochschulen sind verpflichtet, ihre Studierenden vor Äußerungen und Ideen zu schützen, die als beleidigend oder verstörend empfunden werden könnten.

it2: (faimut): An meiner Hochschule wird der freie Austausch von ganz unterschiedlichen Sichtweisen ermutigt und gefördert.

it3: (faiausl): Gastredner\*innen sollten wieder ausgeladen werden, wenn einige Studierende es fordern.

it4: (faiprot): Kontroverse Gastredner\*innen zu stören oder am Reden zu hindern ist eine legitime Form des Protests.

it5: (faimei): Bei kontroversen Diskussionen in Seminaren oder anderen Anlässen meiner Hochschule vermeide ich es lieber, meine ehrliche Meinung zu sagen.

it6: (faians1): Die meisten Lehrenden und Studierenden an meiner Hochschule haben politische Ansichten, die meinen eigenen sehr ähnlich sind.

st:

ao1: 1: lehne völlig ab

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: stimme völlig zu 

ao6: -12: kann ich nicht beurteilen 

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

hi: @ZOFAR: t5 wird in der QML response Domain nicht benannt. Bitte t5 labeln.


\------------------------------------------------------------

KSM-fai06 
=========

tc:

vn: faiwige

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden. 

Absolvent\*innen wirtschaftswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 43.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen wirtschaftswissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Geisteswissenschaften?

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

tr: GOTO KSM-fai16

hi:


\------------------------------------------------------------

KSM-fai07 
=========

tc:

vn: faiinge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:
 
in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Geisteswissenschaften?

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

tr: GOTO KSM-fai17

hi:


\------------------------------------------------------------

KSM-fai08 
=========

tc:

vn: faimedge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Geisteswissenschaften?

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

tr: GOTO KSM-fai18

hi:


\------------------------------------------------------------

KSM-fai09 
=========

tc:

vn: fairecge

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen rechtswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 46.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Geisteswissenschaften verdienen demgegenüber durchschnittlich ca. 35.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen rechtswissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Geisteswissenschaften?

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

tr: GOTO KSM-fai19

hi:


\------------------------------------------------------------

KSM-fai10 
=========

tc:

vn: faimedrec

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Rechtswissenschaften verdienen demgegenüber durchschnittlich ca. 46.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Rechtswissenschaften?

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

tr: GOTO KSM-fai20

hi:


\------------------------------------------------------------

KSM-fai11 
=========

tc:

vn: faimedin

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Ingenieurwissenschaften verdienen demgegenüber durchschnittlich ca. 47.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Ingenieurwissenschaften?

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

tr: GOTO KSM-fai21

hi:


\------------------------------------------------------------

KSM-fai12 
=========

tc:

vn: faimedwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen der Medizin verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 53.000 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen der Medizin direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

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

tr: GOTO KSM-fai22

hi:


\------------------------------------------------------------

KSM-fai13 
=========

tc:

vn: fairecwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen rechtswissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 46.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen rechtswissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

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

tr: GOTO KSM-fai23

hi:


\------------------------------------------------------------

KSM-fai14
=========

tc:

vn: faiinrec

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.  

Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Rechtswissenschaften verdienen demgegenüber durchschnittlich ca. 46.500 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Rechtswissenschaften?

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

tr: GOTO KSM-fai24

hi:


\------------------------------------------------------------

KSM-fai15 
=========

tc:

vn: faiinwi

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: Im Folgenden geht es um Gehaltsunterschiede zwischen Absolvent\*innen verschiedener Fächergruppen und darum, ob Sie diese Unterschiede als gerechtfertigt empfinden.

Absolvent\*innen ingenieurwissenschaftlicher Fächer verdienen nach ihrem Abschluss in Vollzeit durchschnittlich etwa 47.500 € pro Jahr (Bruttojahresgehalt). Absolvent\*innen der Wirtschaftswissenschaften verdienen demgegenüber durchschnittlich ca. 43.000 € im Jahr.

q: In welchem Ausmaß finden Sie es gerechtfertigt, dass Absolvent\*innen ingenieurwissenschaftlicher Studienfächer direkt nach ihrem Abschluss **mehr** verdienen als Absolvent\*innen der Wirtschaftswissenschaften?

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

tr: GOTO KSM-fai25

hi:


\------------------------------------------------------------

KSM-fai16 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Wirtschaftswissenschaften verdienen mehr als Absolvent*/innen der Geisteswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai17 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Ingenieurwissenschaften verdienen mehr als Absolvent*/innen der Geisteswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai18 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Medizin verdienen mehr als Absolvent*/innen der Geisteswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai19 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Rechtswissenschaften verdienen mehr als Absolvent*/innen der Geisteswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften.

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 


\------------------------------------------------------------

KSM-fai20 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Medizin verdienen mehr als Absolvent*/innen der Rechtswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai21 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Medizin verdienen mehr als Absolvent*/innen der Ingenieurwissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai22 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Medizin verdienen mehr als Absolvent*/innen der Wirtschaftswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen.

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai23 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Rechtswissenschaften verdienen mehr als Absolvent*/innen der Wirtschaftswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften.

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai24 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Ingenieurwissenschaften verdienen mehr als Absolvent*/innen der Rechtswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften.

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen.

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 

\------------------------------------------------------------

KSM-fai25 
=========

tc:

vn: faigefun; faifinan; faizeit; fainive; faivolk; failequal; faiveran; faikennt; faikompl; faiflex; faistre; faiand; faiando

qt: Mehrfachauswahl mit Exklusivkategorie

hl:

in:

q: Was könnte Ihrer Meinung nach den höheren Lohn in diesem Beispiel rechtfertigen?

is: Die Absolvent\*innen der Ingenieurwissenschaften verdienen mehr als Absolvent*/innen der Wirtschaftswissenschaften, weil sie …

it:

st:

ao1: (faigefun): eine wichtige gesellschaftliche Funktion übernehmen.

ao2: (faifinan): hohe finanzielle Erträge erwirtschaften. 

ao3: (faizeit): eine längere Wochenarbeitszeit haben.

ao4: (fainive): ein höheres Anforderungsniveau im Studium hatten.

ao5: (faivolk): eine Tätigkeit ausüben, die von größerer Bedeutung für die Volkswirtschaft ist.

ao6: (failequal): zur Sicherung der Lebensqualität in der Gesellschaft beitragen.

ao7: (faiveran): mehr Verantwortung im Beruf übernehmen. 

ao8: (faikennt): über am Arbeitsmarkt stärker nachgefragte Kenntnisse und Fertigkeiten verfügen.

ao9: (faikompl): komplexere Aufgaben im Beruf ausführen.

ao10: (faiflex): geringere zeitliche/räumliche Flexibilität in ihrer Tätigkeit haben.

ao11: (faistre): mehr Stress/Belastungen am Arbeitsplatz haben.

ao12: (faiando): Nichts davon. [Exklusivkategorie]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai26

hi: 




\------------------------------------------------------------

KSM-fai26 
=========

tc:

vn: faidisge; faidismig; faidissoz; faidisspra; faidisrel; faidissex; faidisbeein; faidiselt; faidiskorp

qt: Einfachauswahlmatrix

hl:

in:

q: Es ist nicht immer einfach, nach Abschluss des Studiums einen Job zu finden. Neben legitimen Gründen (z. B. Bewerberprofil passt nicht zur Stelle), kann auch Diskriminierung zu einer Absage führen. Diskriminierung bedeutet, dass eine Person schlechter behandelt wird als andere Menschen, ohne dass es dafür eine sachliche Rechtfertigung gibt. Aufgrund welcher Merkmale wird man Ihrer Meinung nach diskriminiert?

is:

it1: (faidisge): aufgrund des Geschlechts

it2: (faidismig): aufgrund des Migrationshintergrunds

it3: (faidissoz): aufgrund der sozialen Herkunft

it4: (faidisspra): aufgrund der sprachlichen Ausdrucksweise (Dialekt, weniger gewandt)

it5: (faidisrel): aufgrund religiöser Zugehörigkeit

it6: (faidissex): aufgrund der sexuellen Orientierung

it7: (faidisbeein): aufgrund körperlicher oder psychischer Beeinträchtigung

it8: (faidiselt): aufgrund von Elternschaft

it9: (faidiskorp): aufgrund des körperlichen Erscheinungsbilds

st:

ao1: 1: nein

ao2: 2: eher nein

ao3: 3: eher ja

ao4: 4: ja

ao5: -12: weiß nicht

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-fai27

hi:


\------------------------------------------------------------

KSM-fai27 
=========

tc:

vn: faierlge_s/_a; faierlmig_s/_a; faierlsoz_s/_a; faierlspra_s/_a; faierlrel_s/_a; faierlsex_s/_a; faierlbeein_s/_a; faierlelt_s/_a; faierlkorp_s/_a

qt: Mehrfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Haben Sie in Ihrem bisherigen Studium schon einmal Diskriminierung selbst erlebt oder bei anderen beobachtet?

is:

it1: selbst erlebt

it2: bei anderen beobachtet

ao1: (faierlge_s, fairlge_a): aufgrund des Geschlechts

ao2: (faierlmig_s, faierlmig_a): aufgrund des Migrationshintergrunds

ao3: (faierlsoz_s, faierlsoz_a): aufgrund der sozialen Herkunft

ao4: (faierlspra_s, faierlspra_a): aufgrund der sprachlichen Ausdrucksweise (Dialekt, weniger gewandt)

ao5: (faierlrel_s, faierlrel_a): aufgrund religiöser Zugehörigkeit

ao6: (faierlsex_s, faierlsex_a): aufgrund der sexuellen Orientierung

ao7: (faierlbeein_s, faierlbeein_a): aufgrund körperlicher oder psychischer Beeinträchtigung

ao8: (faierlelt_s, faierlelt_a): aufgrund von Elternschaft

ao9: (faierlkorp_s, faieerlkorp_a): aufgrund des körperlichen Erscheinungsbilds

st:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:GOTO KSM-fai28

hi:

\------------------------------------------------------------

KSM-fai28 
=========

tc:

vn: diskjane (diskjane1; diskjane2; diskjane3; diskjane4; diskjane5; diskjane6; diskjane7; diskjane8; diskjane9; diskjane10; diskjane11; diskjane12; diskjane12o; diskjane13)

qt: Mehrfachauswahlmatrix mit Exklusivkategorie und offener Angabe

hl:

in:

q: Welche der folgenden Erfahrungen haben Sie im Rahmen Ihres Studiums bereits gemacht? 
Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu. 

is:

ao1: (diskjane1): Leistungen wurden mir nicht zugetraut.

ao2: (diskjane2): Von mir erbrachte Leistungen wurden herabgesetzt (z. B. ungerecht bewertet).

ao3: (diskjane3): Regeln/Verfahren wurden so gestaltet, dass ich benachteiligt wurde.

ao4: (diskjane4): Ich wurde ausgegrenzt oder übergangen (z. B. in Arbeitsgruppen).

ao5: (diskjane5): Menschen wie ich wurden stereotyp/herabwürdigend dargestellt.

ao6: (diskjane6): Mir sind unangebrachte Bemerkungen zu meinem Privatleben begegnet.

ao7: (diskjane7): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

ao8: (diskjane8): Ich wurde beleidigt oder beschimpft.

ao9: (diskjane9): Ich habe unerwünschte sexualisierte Kommentare erlebt.

ao10: (diskjane10): Ich habe sexualisierte körperliche Übergriffe erlebt.

ao11: (diskjane11): Ich wurde körperlich bedroht oder angegriffen.

ao12: (diskjane12): Andere diskriminierende Erfahrung, und zwar: [(diskjane12o), offene Angabe, 250 Zeichen]

ao13: (diskjane13): Nichts davon.[Exklusivkategorie]

st:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:GOTO KSM-fai29 if  diskjane1=1 OR diskjane2=1 OR   diskjane3=1 OR  diskjane4=1 OR diskjane5=1 OR diskjane6=1 OR  diskjane7=1 OR diskjane8=1 OR diskjane9=1 OR diskjane10=1 OR diskjane11=1 OR diskjane12=1 GOTO ABSCHLUSSSEITE IF diskjane1=0 AND diskjane2=0 AND diskjane3=0 AND diskjane4=0 AND diskjane5=0 AND diskjane6=0 AND diskjane7=0 AND diskjane8=0 AND diskjane9=0 AND diskjane10=0 AND diskjane11=0 AND diskjane12=0 OR diskjane13=1

hi: Frage existiert in ähnlicher Form bereits (N_13), wurde dort gestrichen und nun in abgewandelter Form an diese Stelle verschoben. 
Satz "Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu." nicht fett drucken. 

\------------------------------------------------------------

KSM-fai29 
=========

tc:

vn: diskanza (diskanza1; diskanza2; diskanza3; diskanza4; diskanza5; diskanza6; diskanza7; diskanza8; diskanza9; diskanza10; diskanza11; diskanza12)

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie häufig haben Sie diese Erfahrungen im Rahmen des Studiums gemacht?

is:

it1: (diskanza1): Leistungen wurden mir nicht zugetraut.

it2: (diskanza2): Von mir erbrachte Leistungen wurden herabgesetzt (z. B. ungerecht bewertet).

it3: (diskanza3): Regeln/Verfahren wurden so gestaltet, dass ich benachteiligt wurde.

it4: (diskanza4): Ich wurde ausgegrenzt oder übergangen (z. B. in Arbeitsgruppen).

it5: (diskanza5): Menschen wie ich wurden stereotyp/herabwürdigend dargestellt.

it6: (diskanza6): Mir sind unangebrachte Bemerkungen zu meinem Privatleben begegnet.

it7: (diskanza7): Man hat abwertende Witze über mich gemacht oder mich ausgelacht.

it8: (diskanza8): Ich wurde beleidigt oder beschimpft.

it9: (diskanza9): Ich habe unerwünschte sexualisierte Kommentare erlebt.

it10: (diskanza10): Ich habe sexualisierte körperliche Übergriffe erlebt.

it11: (diskanza11): Ich wurde körperlich bedroht oder angegriffen.

it12: (diskanza12): Andere diskriminierende Erfahrung:

ao1: 1: einmal

ao2: 2: mehrmals

ao3: 3: regelmäßig

st:

mv:

ka:

vc1: SHOW it1 (diskanza1) IF diskjane1=1
vc2: SHOW it2 (diskanza2) IF diskjane2=1
vc3: SHOW it3 (diskanza3) IF diskjane3=1
vc4: SHOW it4 (diskanza4) IF diskjane4=1
vc5: SHOW it5 (diskanza5) IF diskjane5=1
vc6: SHOW it6 (diskanza6) IF diskjane6=1
vc7: SHOW it7 (diskanza7) IF diskjane7=1
vc8: SHOW it8 (diskanza8) IF diskjane8=1
vc9: SHOW it9 (diskanza9) IF diskjane9=1
vc10: SHOW itq10 (diskanza10) IF diskjane10=1
vc11: SHOW it11 (diskanza11) IF diskjane11=1
vc12: SHOW it12 (diskanza12) IF diskjane12=1


av:

kh:

fv:

hv:

fo:

tr:GOTO ABSCHLUSSSEITE 

hi: Frage existiert in ähnlicher Form bereits (N_14), wurde dort gestrichen und nun in abgewandelter Form an diese Stelle verschoben. 


