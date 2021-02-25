\--------------------------------

B1_1
=

tc:

vn: sexorient; sexoriento

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Was beschreibt Ihre sexuelle Orientierung am ehesten?

is:

it:

st:

ao1: 1: heterosexuell

ao2: 2: schwul

ao3: 3: lesbisch

ao4: 4: bisexuell

ao5: 5: Präfix: Eine andere, und zwar: [offene Angabe, 25-stellig]

ao6: 6: unklar

mv: -13: Ich möchte diese Frage nicht beantworten.

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 

        <zofar:transitions>
            <zofar:transition target="B1_3a" condition="zofar.asNumber(h_split)==1"/>
            <zofar:transition target="B1_3b" condition="zofar.asNumber(h_split)==2"/>
        </zofar:transitions>

hi:

\--------------------------------

B1_2
=

tc:

vn: genidsach; genidloes; genidrat; genidlieb; genideinf; genidemo; genidrisk

qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Wenn Sie sich selbst beschreiben müssten: Inwiefern treffen die folgenden Eigenschaften auf Sie zu?

is:

it1: (genidloes): lösungsorientiert

it2: (genidlieb): liebevoll

it3: (genidsach): sachlich

it4: (genideinf): einfühlsam

it5: (genidrat): rational

it6: (genidemo): emotional

it7: (genidrisk): risikobereit

st:

ao1: 1: trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr:

        <zofar:transitions>
            <zofar:transition target="B1_1"/>
        </zofar:transitions>

hi:

\--------------------------------

B1_3a
==

tc: If demosex !=3 (?; tc bitte im Rahmen neugesetzten Seitenweiterleitungsbedingungen prüfen)

vn: besex1; besex3; besex5; hosex1; hosex2; hosex5

qt: Einfachauswahlmatrix

hl:

in:






q: Nachfolgend finden Sie eine Reihe von Aussagen über Frauen und Männer und ihre Beziehungen in der heutigen Gesellschaft. Bitte geben Sie an, in welchem Ausmaß Sie der jeweiligen Aussage zustimmen oder nicht zustimmen.

is:

it1: (besex1): Egal wie erfolgreich ein Mann auch sein mag, ohne die Liebe einer Frau fehlt ihm etwas ganz Wichtiges.

it2: (hosex1): Wenn Frauen in einem fairen Wettbewerb gegenüber Männern den Kürzeren ziehen, behaupten sie gerne, sie seien diskriminiert worden.

it3: (hosex2): Feministinnen stellen oftmals unberechtigte Forderungen an Männer.

it4: (besex3): Jeder Mann sollte eine Frau haben, die er über alles liebt.

it5: (besex5): Ein Mann sollte bereit sein, sein eigenes Wohl zu opfern, um für seine Frau sorgen zu können.

it6: (hosex5): Viele Frauen versuchen unter dem Deckmantel der Gleichberechtigung besondere Vergünstigungen zu erlangen, wie z. B. eine Bevorzugung bei der Besetzung von Arbeitsstellen.

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

tr:

	<zofar:transitions>
        <zofar:transition target="D3_13" condition="(zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6)"/>
        <zofar:transition target="A_54" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==13)"/>
    	</zofar:transitions>

hi:

\--------------------------------

B1_3b
==

tc:

vn: chldsuffer; malebread; wrkmumhome; chldben; fullmumtod; bothfull; fulldadtod


qt: Einfachauswahlmatrix mit horizontalen ao

hl:

in:

q: Über die Aufgaben von Müttern und Vätern gibt es verschiedene Meinungen. Bitte geben Sie an, inwiefern Sie den folgenden Aussagen zustimmen.

is:

it1: (chldsuffer): Ein Kleinkind wird sicherlich darunter leiden, wenn seine Mutter berufstätig ist.

it2: (malebread): Es ist für alle Beteiligten besser, wenn der Mann voll im Berufsleben steht und die Frau sich um den Haushalt und die Kinder kümmert.

it3: (chldben): Es ist für ein Kind gut, wenn seine Mutter berufstätig ist und sich nicht nur auf den Haushalt konzentriert.

it4: (wrkmumhome): Auch wenn beide Eltern erwerbstätig sind, ist es besser, wenn die Verantwortung für den Haushalt und die Kinder hauptsächlich bei der Frau liegt.
.
it5: (fullmumtod): Eine Vollzeit erwerbstätige Mutter kann zu ihrem Kleinkind normalerweise ein genauso inniges Verhältnis haben, wie eine Mutter, die nicht berufstätig ist.

it6: (bothfull): Die beste Arbeitsteilung in einer Familie ist die, dass beide Partner in gleichem Umfang arbeiten und sich gleichermaßen um den Haushalt und die Kinder kümmern.

it7: (fulldadtod): Ein Vollzeit erwerbstätiger Vater kann zu seinem Kleinkind normalerweise ein genauso inniges Verhältnis haben wie ein Vater, der nicht berufstätig ist.

st:

ao1: 1: stimme gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: stimme voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr:

        <zofar:transitions>
            <zofar:transition target="D3_13" condition="(zofar.asNumber(mastersplit)==3             or zofar.asNumber(mastersplit)==4             or zofar.asNumber(mastersplit)==5             or zofar.asNumber(mastersplit)==6)"/>
            <zofar:transition target="A_54" condition="(zofar.asNumber(mastersplit)==1             or zofar.asNumber(mastersplit)==2             or zofar.asNumber(mastersplit)==13)"/>
        </zofar:transitions>
        
hi:

\--------------------------------

B1_4a
==

tc: IF wohnpar=1

vn: atakhh_p; atakhh_i; atakhh_a; atakee_p; atakee_i; atakee_a; atakwe_p; atakwe_i; atakwe_a; atakkb_p; atakkb_i; atakkb_a

qt: Mehrfachauswahlmatrix mit horizontalen ao mit offener Nennung

hl:

in:

q: Wer trägt in Ihrer Partnerschaft in welchem Ausmaß zu folgenden Bereichen bei?

is: Bitte summieren Sie jeweils die ++Spaltenprozente++ auf 100 Prozent.

it1: (\_p): Partner\*in

it2: (\_i): ich selbst

it3: (\_a): andere Personen

st:

ao1 (atakhh): !!Haushalt!! [offene Angabe, 3-stellig: 0 TO 100, Suffix: %]

ao2 (atakee): !!Erwerbseinkommen!! [offene Angabe, 3-stellig: 0 TO 100, Suffix: %]

ao3 (atakwe): !!Treffen wichtiger Entscheidungen!! [offene Angabe, 3-stellig: 0 TO 100, Suffix: %]

ao4 (atakkb): !!Kinderbetreuung!! [offene Angabe, 3-stellig: 0 TO 100, Suffix: %]

mv:

ka:

vc: SHOW ao4 IF dkinja=2

av: 

kh: Bitte geben Sie den prozentualen Anteil an (0 bis 100).

fv:

hv:

fo: Bitte eine vierte Zeile programmieren, in der in der Itemspalte unter it3 ("andere Personen") "Summe" steht. In dieser vierten Zeile soll zudem für die vier ao-Spalten dann jeweils "100 %" als Text stehen. 

tr:

        <zofar:transitions>
            <zofar:transition target="B1_4b"/>
        </zofar:transitions>

hi:

\--------------------------------

B1_4b
==

tc: IF wohnpar=1

vn1: atakzufr

qt: Einfachauswahl mit ao

hl:

in: 

q: Alles in allem: Wie zufrieden sind Sie mit der derzeitigen Arbeitsteilung zwischen Ihnen und Ihrem/Ihrer Partner\*in in Ihrem Haushalt?

is: 

it: 

st:

ao1: 1: gar nicht zufrieden 

ao2: 2

ao3: 3

ao4: 4

ao5: 5: voll und ganz zufrieden

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
            <zofar:transition target="B1_2"/>
        </zofar:transitions>

hi:  


\--------------------------------

B1_5
==

tc:

vn: atihh; atiee; atiwe; atikb


qt: Einfachauswahlmatrix mit horizontalen ao

hl: 

in: 

q: In einem Haushalt fallen täglich eine Reihe von Aufgaben an, die es zu bewältigen gilt. Unabhängig davon, ob Sie aktuell in einer Partnerschaft leben: Bitte geben Sie an, wer Ihrer Meinung nach für die folgenden Haushaltsbereiche ++idealerweise++ zuständig sein sollte.

is: 

it1: (atihh): Haushalt

it2: (atiee): Erwerbseinkommen

it3: (atiwe): Treffen wichtiger Entscheidungen

it4: (atikb): Kinderbetreuung

st:

ao1: 1: ausschließlich mein\*e Partner\*in





ao2: 2: eher mein\*e Partner\*in

ao3: 3: wir beide gleichermaßen

ao4: 4: eher ich

ao5: 5: ausschließlich ich

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
            <zofar:transition target="B1_4a" condition="wohnpar.value"/>
            <zofar:transition target="B1_2" condition="!wohnpar.value or zofar.isMissing(wohnpar)"/>
        </zofar:transitions>
    
hi: 


\--------------------------------

B1_6
==

tc:

vn: athhm_m; athhm_v; athhm_i; athhm_a; ateem_m; ateem_v; ateem_i; ateem_a; atwem_m; atwem_v; atwem_i; atwem_a; atkbm_m; atkbm_v; atkbm_i; atkbm_a; atkam_m; atkam_v; atkam_i; atkam_a

qt: Mehrfachauswahlmatrix mit horizontalen ao mit offener Nennung

hl:

in:

q: Wenn Sie nun an Ihre Kindheit denken: Wer hat in Ihrer Familie in welchem Ausmaß zu den unterschiedlichen Bereichen beigetragen?

is: Bitte summieren Sie jeweils die ++Spaltenprozente++ auf 100 Prozent.

it1: (\_m): Mutter

it2: (\_v): Vater

it3: (\_i): ich selbst

it4: (\_a): andere Personen

st:

ao1 (athhm): !!Haushalt!! [offene Angabe, NUMBER, 3-stellig: 0 TO 100, Suffix: %]

ao2 (ateem): !!Erwerbseinkommen!! [offene Angabe, NUMBER, 3-stellig: 0 TO 100, Suffix: %]

ao3 (atwem): !!Treffen wichtiger Entscheidungen!! [offene Angabe, NUMBER, 3-stellig: 0 TO 100, Suffix: %]

ao4 (atkbm): !!Kinderbetreuung!! [offene Angabe, NUMBER, 3-stellig: 0 TO 100, Suffix: %]

mv:

ka:

vc:

av:

kh: Bitte geben Sie den prozentualen Anteil an (0 bis 100).

fv:

hv:

fo: Bitte eine fünfte Zeile programmieren, in der in der Itemspalte unter it4 ("andere Personen") "Summe" steht. In dieser fünften Zeile soll zudem für die vier ao-Spalten dann jeweils "100 %" als Text stehen.. 

tr:

        <zofar:transitions>
            <zofar:transition target="B1_8"/>
        </zofar:transitions>

hi:

\--------------------------------

B1_7
==

tc:

vn: ssanlehr

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wenn Sie an die Lehrenden in Ihren Lehrveranstaltungen denken: Wie hoch ist der Anteil an weiblichem Lehrpersonal?

is:

it:

st:

ao1: 1: 0 % bis 10 %

ao2: 2: 11 % bis 20 %

ao3: 3: 21 % bis 30 %

ao4: 4: 31 % bis 40 %

ao5: 5: 41 % bis 50 %

ao6: 6: 51 % bis 60 %

ao7: 7: 61 % bis 70 %

ao8: 8: 71 % bis 80 %

ao9: 9: 81 % bis 90 %

ao10: 10: 91 % bis 100 %

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
            <zofar:transition target="A_28"/>
        </zofar:transitions>

hi:

\--------------------------------

B1_8
==

tc:

vn: promgroßv; promgroßm; promvat; prommut; prombrud; promschw

qt: Einfachauswahl mit horizontalen ao

hl:

in:

q: Gibt es in Ihrem familiären Umfeld jemanden, der studiert bzw. promoviert (hat)?

is: Bitte geben Sie immer den höchsten Bildungsgang an.

it1: (promgroßv): Großvater

it2: (promgroßm): Großmutter

it3: (promvat): Vater

it4: (prommut): Mutter

it5: (prombrud): Bruder

it6: (promschw): Schwester

st:

ao1: 1: nein

ao2: 2: studiert

ao3: 3: promoviert

mv1: -12: weiß ich nicht

ka:

vc: SHOW it5, it6 IF dsibo >=1

av:

kh:

fv:

hv:

fo:

tr:

        <zofar:transitions>
            <zofar:transition target="A_34"/>
        </zofar:transitions>

hi:

