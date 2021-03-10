\------------------------------------------------------------

KSM-anf01
=========

tc: Einstiegsseite

vn: 

qt: 

hl: 

in:  
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

hi:

\------------------------------------------------------------

KSM-anf02
=========

tc:

vn: bilaspabb / bilaspbab / bilaspmab / bilaspdrb / bilaspberb

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie …

is:

it1: (bilaspabb) … einen Hochschulabschluss erreichen?

it2: (bilaspbab) … einen Bachelorabschluss erreichen?

it3: (bilaspmab) … einen Master erreichen?

it4: (bilaspdrb) … einen Doktortitel erreichen?

it5: (bilaspberb) … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv: -12: weiß ich nicht

ka:

vc: SHOW it1 IF sabsan != 1 OR sabsan != 2 SHOW it2 IF sabsan = 1 OR sabsan = 2 SHOW it3 IF sabsan = 1 OR sabsan = 2

av:

kh:

fv:

hv:

fo: mv/"weiß ich nicht" absetzen

tr: GOTO KSM-anf03

hi:



\--------------------------

KSM-anf03
=========

tc:

vn: intsoc1 / intsoc3 / intsoc4 / intinv1 / intinv2 / intinv4 / intart1 / intart2 / intart4 / intent1 / intent2 / intent3 / Intconv2 / intconv3 / intconv4 / intreal1 / intreal2 / intreal3

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Bitte geben Sie an, wie sehr Sie sich für folgende Tätigkeiten interessieren.

is:

it1: (intsoc1): anderen Menschen helfen

it2: (intsoc3): sich mit den Lebenslagen von Menschen/Gruppen auseinandersetzen

it3: (intsoc4): mit Menschen (zusammen)arbeiten

it4: (intinv1): etwas genau beobachten und analysieren

it5: (intinv2): Unbekanntes erforschen, experimentieren

it6: (intinv4): Lösungen für komplexe Probleme finden

it7: (intart1): kreativ/gestaltend tätig sein

it8: (intart2): sich mit Kunst und Kultur befassen

it9: (intart4): etwas sprachlich ansprechend formulieren

it10: (intent1): Unternehmen gründen oder leiten

it11: (intent2): andere von einer Sache überzeugen

it12: (intent3): andere Menschen anleiten oder führen

it13: (Intconv2): sich mit rechtlichen Fragen beschäftigen

it14: (intconv3): Arbeitsprozesse planen

it15: (intconv4): mit Zahlen oder Statistiken arbeiten

it16: (intreal1): untersuchen, wie Dinge funktionieren

it17: (intreal2): innovative technische Lösungen entwickeln

it18: (intreal3): an Soft- oder Hardware arbeiten

st:

ao1: 1: überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

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

\--------------------------

KSM-anf04
=========

tc:

vn: stfwb (stfweinb / stfwartb / stfwaltb / stfwzeitb / stfwfamb / stfwberb / stfwbegab / stfwintb / stfwwissb / stfwverfb / stfwverbb / stfwandb / stfwandob)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen Studienfaches?

is:

it1: (stfweinb): Einkommens- und Karrierechancen

it2: (stfwartb): gute Aussichten auf sicheren Arbeitsplatz

it3: (stfwaltb): keine Zulassung im gewünschten Studienfach

it4: (stfwzeitb): kurze Studienzeiten

it5: (stfwfamb): Eltern/Familie haben mir dazu geraten

it6: (stfwberb): fester Berufswunsch

it7: (stfwbegab): eigene Begabung

it8: (stfwintb): spezielles Fachinteresse

it9: (stfwwissb): eine gute wissenschaftliche Ausbildung

it10: (stfwverfb): Vereinbarkeit von Familie mit späteren Beschäftigungsmöglichkeiten

it11: (stfwverbb): Vereinbarkeit meiner Beeinträchtigung(en) mit späteren Beschäftigungsmöglichkeiten

it12: (stfwandb): Anderes, und zwar: [(stfwando); 100 Zeichen]

st:

ao1: 1: gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv:

ka:

vc: SHOW it11 (stfwverbb) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf05

\--------------------------

KSM-anf05
=========

tc:

vn: hswb (hswkontb / hswbedb / hswattb / hswfachb / hswrankb / hswtradb / hswzulb / hswintb / hswtzb / hswsuppb / hswbarrb / hswandb / hswandob)

qt: Einfachauswahlmatrix/5er-Skala mit horizontalen ao

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen Hochschule?

is:

it1: (hswkontb): Freund*innen/Familie vor Ort

it2: (hswbedb): günstige Lebensbedingungen am Hochschulort

it3: (hswattb): Attraktivität von Stadt und Umgebung

it4: (hswfachb): gewünschte Fachrichtung

it5: (hswrankb): gute Platzierung meines Fachs in Rankings

it6: (hswtradb): Tradition und Ruf der Hochschule

it7: (hswzulb): keine Zulassung an Wunschhochschule

it8: (hswintb): internationale Ausrichtung der Hochschule

it9: (hswtzb): Möglichkeit, in Teilzeit studieren zu können

it10: (hswsuppb): hochschulspezifische Beratungs- und Unterstützungsangebote

it11: (hswbarrb): Barrierefreiheit der Hochschule

it12: (hswandb): Anderes, und zwar: [(hswando); 100 Zeichen]

st:

ao1: 1: gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr wichtig

mv:

ka:

vc: SHOW it11 (hswbarrb) IF gartmob=1 OR gartseh=1 OR gartohr=1 OR gartspr=1 OR gartpsy=1 OR gartsom=1 OR garttls=1 OR gartson=1 OR gartka=1

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-anf06

\------------------------------------------------------------

KSM-anf06
=========

tc:

vn: massnahm1; massnahm2; massnahm3; massnahm4; massnahm5; massnahm6

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Haben Sie vor der Aufnahme Ihres aktuellen Studiums an den folgenden Maßnahmen teilgenommen? 

is:

it1: (massnahm1): Tests zur fachlichen Eignung (Online Self Assessment, Studicheck, Wissenstest, Studium-Interessenstests)

it2: (massnahm2): Aufnahmeprüfungen

it3: (massnahm3): Aufnahmegespräche

it4: (massnahm4): Probestudium

it5: (massnahm5): Schüleruni, Schnupperstudium

it6: (massnahm6): E-Learning-Angebote im bundesweiten Onlineportal _Studiport_

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

tr: GOTO KSM-anf07 IF massnahm1 = 2 
GOTO KSM-anf08 IF massnahm1 <> 2 

hi:


\------------------------------------------------------------

KSM-anf07
=========

tc:

vn: pflicht1

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Waren die Maßnahmen verpflichtend oder freiwillig?

is:

it1: (pflicht1): Tests zur fachlichen Eignung (Online Self Assessment, Studicheck, Wissenstest, Studium-Interessenstests)

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

tr: GOTO KSM-anf08

hi:


\------------------------------------------------------------

KSM-anf08
=========

tc:

vn: angeb1; angeb2; angeb3; angeb4; angeb5; angeb6; angeb7

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Welche Angebote gibt es Ihres Wissens nach an Ihrer Hochschule? An welchen haben Sie teilgenommen?

is:

it1: (angeb1): Betreuung bei Studienaufnahme (Einschreibung, Zimmersuche)

it2: (angeb2): Studienvorbereitende Tage, Camps oder Orientierungswochen

it3: (angeb3): „Brückenkurse“ zur Aufarbeitung fachlicher Wissenslücken

it4: (angeb4): Studentische Ansprechpartner zu Fragen rund ums Studium (z.B. Tutorien-, Buddy-Programme)

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

tr: GOTO KSM-anf09 IF angeb1 = 4 OR angeb2 = 4 OR angeb3 = 4 OR angeb4 = 4 OR angeb5 = 4 OR angeb6 = 4 OR angeb7 = 4
GOTO KSM-anf10 IF angeb1 <> 4 AND angeb2 <> 4 AND angeb3 <> 4 AND angeb4 <> 4 AND angeb5 <> 4 AND angeb6 <> 4 AND angeb7 <> 4

hi:


\------------------------------------------------------------

KSM-anf09
=========

tc:

vn: nutz1; nutz2; nutz3; nutz4; nutz5; nutz6; nutz7

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wie beurteilen Sie den Nutzen dieser Angebote für Ihren Studienfortgang?

is:

it1: (nutz1): Betreuung bei Studienaufnahme (Einschreibung, Zimmersuche)

it2: (nutz2): Studienvorbereitende Tage, Camps oder Orientierungswochen

it3: (nutz3): „Brückenkurse“ zur Aufarbeitung fachlicher Wissenslücken

it4: (nutz4): Studentische Ansprechpartner zu Fragen rund ums Studium (z.B. Tutorien-, Buddy-Programme)

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

tr: GOTO KSM-anf10

hi:


\------------------------------------------------------------

KSM-anf10
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

it5: (studall5): mit meinen finanziellen Mitteln auskommen

it6: (studall6): Alltagsorganisation (Haushaltsführung, Behördengänge)

it7: (studall7): Eigenverantwortung

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

tr: GOTO KSM-anf12

hi:

\------------------------------------------------------------

KSM-anf12
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


