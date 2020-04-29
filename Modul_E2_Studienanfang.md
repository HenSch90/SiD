\------------------------------------------------------------

KSM-anf01
=========

tc: Einstiegsseite

vn: 

qt: 

hl: 

in: 
Übergang an die Hochschule: 
Der Übergang an die Hochschule kann mit verschiedenen Herausforderungen und Schwierigkeiten verbunden sein. Im Folgenden werden wir Ihnen daher Fragen zu Ihrer Studienanfangsphase stellen.

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

tr: GOTO KSM-anf02 IF mastersplit <> 1, 2, 3, 4, 5, 6, 13
GOTO KSM-anf03 IF mastersplit = 1, 2, 3, 4, 5, 6, 13

hi: Wäre es möglich, diesen Eingangstext etwas größer darzustellen als es sonst für die Einleitung üblich ist?

\------------------------------------------------------------

KSM-anf02
=========

tc:

vn: paba; pama ; paphd ; pajob

qt: Einfachauswahlmatrix

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie…

is:

it1: (paba): … einen Hochschulabschluss erreichen?

it2: (pama): … einen Master erreichen?

it3: (paphd): … einen Doktortitel erreichen?

it4: (pajob): … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: sehr unwichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

ao6: -12: weiß ich nicht

mv: 

ka:

vc: SHOW it2 IF sabsan = 1

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

vn: intsoc1; intinv1; intinv2; intart1; intart2; intent1; intent2; intconv2; intreal1; intreal2; intsoc3; intsoc4; intinv4; intart4; intent3; intconv3; intconv4; intreal3

qt: Einfachauswahlmatrix

hl:

in:

q: Bitte geben Sie an, wie sehr Sie sich für folgende Tätigkeiten interessieren.

is:

it1: (intreal1): untersuchen, wie Dinge funktionieren

it2: (intinv4): Lösungen für komplexe Probleme finden

it3: (intart1): kreativ/gestaltend tätig sein

it4: (intsoc1): anderen Menschen helfen

it5: (intent1): Unternehmen gründen oder leiten

it6: (Intconv2): sich mit rechtlichen Fragen auseinandersetzen

it7: (intreal2): innovative technische Lösungen entwickeln

it8: (intinv2): Unbekanntes erforschen, experimentieren

it9: (intart2): sich mit Kunst und Kultur befassen

it10: (intsoc3): sich mit den Lebenslagen von Menschen auseinandersetzen

it11: (intent3): andere Menschen anleiten oder führen

it12: (intconv3): Arbeitsprozesse planen

it13: (intreal3): an Soft- oder Hardware arbeiten

it14: (intinv1): etwas genau beobachten und analysieren

it15: (intart4): etwas sprachlich ansprechend formulieren

it16: (intsoc4): mit Menschen (zusammen)arbeiten

it17: (intent2): andere von einer Sache überzeugen

it18: (intconv4): mit Zahlen oder Statistiken arbeiten

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

tr: GOTO KSM-anf04

hi: 

\------------------------------------------------------------

KSM-anf04
=========

tc:

vn: erwfach; erwwiss; erwleis; erweiglei; erwori; erwatmo; erwdid; erwauss; erwansp

qt: Einfachauswahlmatrix

hl:

in:

q: Welche Erwartungen an das Studium hatten Sie vor Ihrer Studienaufnahme?
Ich habe erwartet, dass … 

is:

it1: (erwfach): ich interessante Fachinhalte lerne

it2: (erwwiss): ich viel wissenschaftlich arbeite

it3: (erwleis): ich hohe Leistungen erbringen muss

it4: (erweiglei): ich die Leistungsanforderungen meistern kann

it5: (erwori): ich durch die Hochschule gut betreut werde

it6: (erwatmo): ich Anschluss zu anderen Studierenden finde

it7: (erwdid): die Lehrenden Fachinhalte gut vermitteln

ao8: (erwauss): die Ausstattung (Seminarräume, Bibliothek, Labore) sehr gut ist

ao9: (erwansp): die Lehrenden sich um Studierende kümmern

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

tr: KSM-anf05

hi:

\------------------------------------------------------------

KSM-anf05
=========

tc:

vn: massnahm1; massnahm2; massnahm3; massnahm4; massnahm5; massnahm6

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Haben Sie vor der Aufnahme Ihres aktuellen Studiums an folgenden Maßnahmen teilgenommen? 

is:

it1: (massnahm1): Tests zur fachlichen Eignung (Online Self Assessment, Studicheck, Wissenstest, Studium-Interessentests)

it2: (massnahm2): Aufnahmeprüfungen

it3: (massnahm3): Aufnahmegespräche

it4: (massnahm4): Probestudium

it5: (massnahm5): Schüleruni, Schnupperstudium

it6: (massnahm6): E-Learning-Angebote im bundesweiten Onlineportal Studiport

st:

ao1: 1: nicht teilgenommen

ao2: 2: teilgenommen


mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf06 IF massnahm1 = 2 
GOTO KSM-anf07 IF massnahm1 <> 2 

hi:


\------------------------------------------------------------

KSM-anf06
=========

tc:

vn: pflicht1

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Waren die Maßnahmen verpflichtend oder freiwillig?

is:

it1: (pflicht1): Tests zur fachlichen Eignung (Online Self Assessment, Studicheck, Wissenstest, Studium-Interessentests)

st:

ao1: 1: verpflichtend

ao2: 2: freiwillig

mv: 

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf07

hi:


\------------------------------------------------------------

KSM-anf07
=========

tc:

vn: angeb1; angeb2; angeb3; angeb4; angeb5; angeb6; angeb7

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Welche Angebote gibt es Ihres Wissens an Ihrer Hochschule? An welchen haben Sie teilgenommen?

is:

it1: (angeb1): Betreuung bei Studienaufnahme (Einschreibung, Zimmersuche)

it2: (angeb2): studienvorbereitende Tage, Camps oder Orientierungswochen

it3: (angeb3): „Brückenkurse“ zur Aufarbeitung fachlicher Wissenslücken

it4: (angeb4): studentische Ansprechpartner zu Fragen rund ums Studium (z.B. Tutorien-, Buddy- Programme

it5: (angeb5): Beratung von Lehrenden zum Studienverlauf (z.B. Mentoringprogramme)

it6: (angeb6): Studienberatung

it7: (angeb7): Psychologische Beratung

st:

ao1: 1: kenne ich nicht

ao2: 2: gab es nicht

ao3: 3: gab es, habe nicht teilgenommen

ao4: 4: gab es, habe teilgenommen

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf08 IF angeb1 = 4 OR angeb2 = 4 OR angeb3 = 4 OR angeb4 = 4 OR angeb5 = 4 OR angeb6 = 4 OR angeb7 = 4
GOTO KSM-anf09 IF angeb1 <> 4 AND angeb2 <> 4 AND angeb3 <> 4 AND angeb4 <> 4 AND angeb5 <> 4 AND angeb6 <> 4 AND angeb7 <> 4

hi:


\------------------------------------------------------------

KSM-anf08
=========

tc:

vn: nutz1; nutz2; nutz3; nutz4; nutz5; nutz6; nutz7

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie beurteilen Sie den Nutzen dieser Angebote für Ihren Studienfortgang?

is:

it1: (nutz1): Betreuung bei Studienaufnahme (Einschreibung, Zimmersuche)

it2: (nutz2): studienvorbereitende Tage, Camps oder Orientierungswochen

it3: (nutz3): „Brückenkurse“ zur Aufarbeitung fachlicher Wissenslücken

it4: (nutz4): studentische Ansprechpartner zu Fragen rund ums Studium (z.B. Tutorien-, Buddy- Programme

it5: (nutz5): Beratung von Lehrenden zum Studienverlauf (z.B. Mentoringprogramme)

it6: (nutz6): Studienberatung

it7: (nutz7): Psychologische Beratung

st:

ao1: 1: nicht nützlich

ao2: 2: 

ao3: 3: 

ao4: 4: 

ao5: 5: sehr nützlich

mv: 

ka:

vc: SHOW nutz1 IF angeb1 = 4 
SHOW nutz2 IF angeb2 = 4
SHOW nutz3 IF angeb3 = 4
SHOW nutz4 IF angeb4 = 4
SHOW nutz5 IF angeb5 = 4
SHOW nutz6 IF angeb6 = 4
SHOW nutz7 IF angeb7 = 4

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf09

hi:


\------------------------------------------------------------

KSM-anf09
=========

tc:

vn: studall1; studall2; studall3; studall4; studall5; studall6; studall7; 

qt: Einfachauswahlmatrix

hl:

in: 

q:  Der Studienanfang bringt verschiedene Herausforderungen mit sich. Inwiefern bereiten Ihnen folgende Aspekte des Alltags Schwierigkeiten?

is:

it1: (studall1): Wechsel der Umgebung

it2: (studall2): Wohnungssuche

it3: (studall3): Einrichten an der Hochschule (Immatrikulation, Seminarplan)

it4: (studall4): Heimweh (Familie, Freunde)

it5: (studall5): Mit meinen finanziellen Mitteln auskommen

it6: (studall6): Alltagsorganisation (Haushaltsführung, Behördengänge)

it7: (studall7): Eigenverantwortung

st:

ao1: 1: überhaupt keine

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr große

ao6: -12: trifft nicht zu

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf10

hi:

\------------------------------------------------------------

KSM-anf10
=========

tc:

vn: schwstud1; schwstud2; schwstud3; schwstud4; schwstud5; schwstud6; schwstud7; schwstud8; schwstud9; schwstud10; schwstud11

qt: Einfachauswahlmatrix

hl:

in:

q: Und inwiefern bereiten Ihnen folgende Aspekte des Studiums Schwierigkeiten?

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

ao6: -12: kann ich nicht beurteilen

mv: 

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf11

hi:

\------------------------------------------------------------

KSM-anf11
=========

tc:

vn: abbruch1; abbruch2

qt: Einfachauswahlmatrix

hl:

in: 

q:  Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu? 

is:

it1: (abbruch1): Ich habe schon öfter daran gedacht, das Studium abzubrechen.

it2: (abbruch2): Wenn ich nochmals wählen könnte, würde ich mich für ein anderes Studienfach entscheiden.

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


