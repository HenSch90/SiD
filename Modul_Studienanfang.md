\------------------------------------------------------------

KSM-anf01
=========

tc: Einstiegsseite

vn: 

qt: 

hl: 

in: Der Übergang an die Hochschule kann mit verschiedenen Herausforderungen und Schwierigkeiten verbunden sein. Im Folgenden werden wir Ihnen daher abschließend Fragen zu Ihrer Studienanfangsphase sowie zu Ihren persönlichen Interessen stellen.

q: 

is:

it:

st:

ao1:

ao2:

ao3:

ao4:

ao5:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf02a IF sabsan = 1 OR sabsan = 2 AND mastersplit <> 1, 2, 3, 4, 5, 6, 13
GOTO KSM-anf02b IF IF sabsan <> 1 OR sabsan <> 2 AND mastersplit <> 1, 2, 3, 4, 5, 6, 13
GOTO KSM-anf02b IF sabsan=MISSING
GOTO KSM-anf03 IF mastersplit = 1, 2, 3, 4, 5, 6, 13

hi: Wäre es möglich, diesen Eingangstext etwas größer darzustellen als es sonst für die Einleitung üblich ist?

\------------------------------------------------------------

KSM-anf02a
=========

tc: sabsan = 1 OR sabsan = 2  

vn: paba / pama / paphd / pajob

qt: Einfachauswahlmatrix

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie…

is:

it1: (paba) … einen Bachelorabschluss erreichen?

it2: (pama) … einen Masterabschluss erreichen?

it3: (paphd) … einen Doktortitel erreichen?

it4: (pajob) … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: 1: sehr unwichtig

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr wichtig

mv:  6: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf03

hi:

\--------------------------

KSM-anf02b
=========

tc: IF sabsan <> 1 OR sabsan <> 2

vn: pa (pagrad / padoc / parjob)

qt: Einfachauswahlmatrix

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie…

is:

it1: (pagrad) … einen Hochschulabschluss erreichen?

It2: (padoc) … einen Doktortitel erreichen?

It3: (parjob) … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: 1: sehr unwichtig

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr wichtig

mv:  6: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf03

hi:

\--------------------------


KSM-anf03
=========

tc:

vn: intsoc1; intsoc2; intinv1; intinv2; intart1; intart2; intent1; intent2; intconv1; intconv2; intreal1; intreal2; intsoc3; intsoc4; intinv3; intinv4; intart3; intart4; intent3; intent4; intconv3; intconv4; intreal3; intreal4

qt: Einfachauswahlmatrix

hl:

in:

q: Bitte geben Sie an, wie sehr Sie sich für folgende Tätigkeiten interessieren.

is:

it1: (intsoc1): anderen Menschen helfen

it2: (intsoc2): sich mit gesellschaftlichen Themen befassen

it3: (intinv1): etwas genau beobachten und analysieren

it4: (intinv2): Unbekanntes erforschen, experimentieren

it5: (intart1): kreativ/gestaltend tätig sein

it6: (intart2): sich mit Kunst/Literatur/Sprache/ Musik/Design befassen

it7: (intent1): Unternehmen gründen oder leiten

it8: (intent2): andere von einer Sache überzeugen

it9: (intconv1): Dinge ordnen und verwalten

it10: (Intconv2): sich mit rechtlichen Fragen beschäftigen

it11: (intreal1): untersuchen, wie Dinge funktionieren

it12: (intreal2): innovative technische Lösungen entwickeln

it13: (intsoc3): sich mit den Lebenslagen von Menschen/Gruppen auseinandersetzen

it14: (intsoc4): mit Menschen (zusammen)arbeiten

it15: (intinv3): wissenschaftliche Aufsätze lesen

it16: (intinv4): Lösungen für komplexe Probleme finden

it17: (intart3): Gebäude, Landschaften oder Gegenstände designen

it18: (intart4): etwas sprachlich ansprechend formulieren

it19: (intent3): andere Menschen anleiten oder führen

it20: (intent4): Events organisieren oder leiten

it21: (intconv3): Arbeitsprozesse planen

it22: (intconv4): mit Zahlen oder Statistiken arbeiten

it23: (intreal3): an Soft- oder Hardware arbeiten

it24: (intreal4): Konstruktion von Bauwerken

st:

ao1: 1: überhaupt nicht

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

tr: KSM-anf04

hi: Itemliste bitte rotieren

\------------------------------------------------------------

KSM-anf04
=========

tc:

vn: erwfach; erwwiss; erwleis; erweiglei; erwori; erwatmo; erwdid; erwauss; erwansp

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern wurden Ihre Erwartungen, die Sie vor der Studienaufnahme hatten, hinsichtlich der folgenden Aspekte erfüllt?

is:

it1: (erwfach): fachliche Inhalte des Studiums

it2: (erwwiss): wissenschaftliches Arbeiten

it3: (erwleis): Höhe der Leistungsanforderungen

it4: (erweiglei): eigene Leistungsfähigkeit

it5: (erwori): Orientierungshilfe und Betreuung durch die Hochschule

it6: (erwatmo): Atmosphäre unter den Studierenden

it7: (erwdid): didaktische Fähigkeiten der Hochschullehrer\*innen

ao8: (erwauss): Ausstattung (Arbeits-, Bibliotheks-, Laborplätze)

ao9: (erwansp): Ansprechbarkeit der Lehrenden

st:

ao1: 1: überhaupt nicht

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

tr: KSM-anf05

hi:

\------------------------------------------------------------

KSM-anf05
=========

tc:

vn: studall1; studall2; studall3; studall4; studall5; studall6; studall7; studall8

qt: Einfachauswahlmatrix

hl:

in:

q: Bereiten Ihnen folgende Aspekte des __Alltags__ Schwierigkeiten?

is:

it1: (studall1): Wechsel der Umgebung

it2: (studall2): Wohnsituation

it3: (studall3): Einrichten an der Hochschule (Immatrikulation, Seminarplan)

it4: (studall4): Heimweh (Familie, Freunde)

it5: (studall5): Studienfinanzierung

it6: (studall6): Vereinbarkeit von Studium und Erwerbstätigkeit

it7: (studall7): Alltagsorganisation (Haushaltsführung, Behördengänge)

ao8: (studall8): Eigenverantwortung

st:

ao1: 1: überhaupt keine

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr große

mv: 6: trifft nicht zu

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: KSM-anf06

hi:

\------------------------------------------------------------

KSM-anf06
=========

tc:

vn: schwstud1; schwstud2; schwstud3; schwstud4; schwstud5; schwstud6; schwstud7; schwstud8; schwstud9; schwstud10; schwstud11

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern bereiten Ihnen folgende Aspekte Schwierigkeiten?

is:

it1: (schwstud1): Wissenschaftlichkeit (z.B. akademische Sprache, Denk- und Arbeitsweise)

it2: (schwstud2): sich an Diskussionen beteiligen

it3: (schwstud3): zeitliche Vorgaben erfüllen

it4: (schwstud4): Lernstrategien entwickeln

it5: (schwstud5): Veranstaltungsinhalten folgen

it6: (schwstud6): englische Sprache (Veranstaltungssprache, Literatur)

it7: (schwstud7): Prüfungsanforderungen bewältigen

ao8: (schwstud8): mit Misserfolgen umgehen

ao9: (schwstud9): die Menge an Lernstoff bewältigen

ao10: (schwstud10): eigene Interessen erkennen

ao11: (schwstud11): Kontakte zu Mitstudierenden knüpfen

st:

ao1: 1: überhaupt nicht

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr stark

mv: 6: kann ich nicht beurteilen

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:
