\--------------------------------

KSM-phd01
==================

tc:

vn: 

qt:

hl:

in: Abschließend interessiert uns Ihre Meinung zu den Gründen für oder gegen eine Promotion.
Promovieren kann man in Deutschland unter ganz unterschiedlichen
Rahmenbedingungen. 

Im Folgenden schildern wir Ihnen einige mögliche
Konstellationen, in denen eine !!fachlich für Sie sehr interessante!! Promotion
an einer !!Hochschule in Deutschland!! möglich ist. Gehen Sie bitte davon aus,
dass die !!formalen Voraussetzungen!! an der Hochschule Ihrer Wahl erfüllt sind
und eine !!geeignete Betreuung der Arbeit!! gewährleistet ist. Die
!!Lebenshaltungskosten!! sind auf dem Niveau Ihres jetzigen Studienorts.

Bitte geben Sie an, wie attraktiv oder unattraktiv Sie die jeweiligen
Rahmenbedingungen einer Promotion aus Ihrer Sicht einschätzen. Uns interessiert
Ihre subjektive Bewertung.

in1: 

in2: 

in3: 

q:

is:

it:

st:

ao1:

ao2:

ao3:

ao4:

ao5:

ao6:

ao7:

ao8:

ao9:

ao10:

ao11:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 
GOTO pvig[deck]_1 IF h_deck_phd==[deck]

hi: 


\--------------------------------

pvig1[deck][vignr]
==================

tc:

vn: prombew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q: Diese Rahmenbedingungen für eine Promotion wären für mich …

is: Bei mobilen Endgeräten bitte die horizontale Ansicht verwenden.

it:

st:

ao1: 0: sehr unattraktiv

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr attraktiv

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: pvig2[deck][vignr]

hi: vigA, vigB und vigC sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert.

\--------------------------------

pvig2[deck][vignr]
==================

tc:

vn: prombew2

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in: 

in1: [vigA]

in2: [vigB]

in3: [vigC]

q: Diese Rahmenbedingungen für eine Promotion wären für mich …

is: Bei mobilen Endgeräten bitte die horizontale Ansicht verwenden.

it:

st:

ao1: 0: sehr unattraktiv

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr attraktiv

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-phd02



hi: vigA, vigB und vigC sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert.

\--------------------------------


KSM-phd02
=========

tc: 

vn: promgrund1- promgrund18; promgrund18o

qt: Einfachauswahlmatrix mit offener Angabe

hl:

in:

q: Es gibt Gründe, die für oder gegen eine Promotion sprechen. Bitte geben Sie an, inwiefern die folgenden Aussagen auf Sie persönlich zutreffen. 

is:

it1: (promgrund1): Ich will zu einem bestimmten Thema forschen.

it2: (promgrund2): Eine Promotion verbessert meine Berufsaussichten. 

it3: (promgrund3): Eine Promotion ist in meinem angestrebten Berufsfeld üblich. 

it4: (promgrund4): Ein Doktortitel besitzt ein hohes soziales Ansehen. 

it5: (promgrund5): Durch eine Promotion kann ich den Berufseinstieg hinausschieben.

it6: (promgrund6): Mein*/e Professor*/in hat mich dazu ermutigt. 

it7: (promgrund7): Mit einer Promotion kann ich meinen Berufswunsch erfüllen.

it8: (promgrund8): Eine Promotion sichert mir ein höheres Einkommen.

it9: (promgrund9): Durch eine Promotion kann ich mich persönlich entfalten.

it10: (promgrund10): Eine Promotion dauert zu lange.

it11: (promgrund11): Eine Promotion kann ich mir finanziell nicht leisten. 

it12: (promgrund12): Mit einer Promotion bin ich überqualifiziert. 

it13: (promgrund13): Das Anforderungsniveau für eine Promotion ist zu hoch.

it14: (promgrund14): Ich habe kein Interesse an einer wissenschaftlichen Tätigkeit. 

it15: (promgrund15): Ich will mich nicht so stark spezialisieren. 

it16: (promgrund16): Eine Promotion passt nicht in meine Lebens- und Familienplanung.

it17: (promgrund17): Eine Promotion ist mit einer zu großen psychischen Belastung verbunden.


it18: (promgrund18): Sonstiges, und zwar: [(promgrund18o), offene Angabe, 250 Zeichen]

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

tr: GOTO A_56 if mastersplit=2 OR mastersplit=4 OR mastersplit=6 OR mastersplit=8 OR mastersplit=10 OR mastersplit=12
GOTO A_50 if mastersplit=1 OR mastersplit=3 OR mastersplit=5 OR mastersplit=7 OR mastersplit=9 OR mastersplit=11


hi: Reihenfolge der Itemliste bitte randomisieren, aber Item 18 immer ans Ende setzen.

\--------------------------------



