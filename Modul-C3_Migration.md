\--------------------------------

C3_1
=

tc:

vn: daltein

qt: Dropdown-Menü

hl:

in:

q: Wie alt waren Sie als Sie nach Deutschland gekommen sind?

is:

it:

st:

ao1: Alter

ao2: <1 Jahr

ao3: 1 Jahr

ao4: 2 Jahre

ao5: 3 Jahre

ao6: 4 Jahre

ao7: 5 Jahre

ao8: 6 Jahre

ao9: 7 Jahre

ao10: 8 Jahre

ao10: 9 Jahre

ao11: 10 Jahre

ao12: 11 Jahre

ao13: 12 Jahre

ao14: 13 Jahre

ao15: 14 Jahre

ao16: 15 Jahre

ao17: 16 Jahre

ao18: 17 Jahre

ao19: 18 Jahre

ao20: 19 Jahre

ao21: 20 Jahre

ao22: 21 Jahre

ao23: 22 Jahre

ao24: 23 Jahre

ao25: 24 Jahre

ao26: 25 Jahre

ao27: 26 Jahre

ao28: 27 Jahre

ao29: 28 Jahre

ao30: 29 Jahre

ao31: 30 Jahre

ao32: >30 Jahre

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
            <zofar:transition target="A_8"/>
        </zofar:transitions>

hi:

\--------------------------------

C3_2
=

tc:

vn: dnat (dnatv; dnatm)

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Welche Staatsangehörigkeit haben Ihre Eltern?

is:

it1: (dnatv): Vater

it2: (dnatm): Mutter

st:

ao1: 1: deutsche Staatsangehörigkeit

ao2: 2: deutsche und eine andere Staatsangehörigkeit

ao3: 3: andere Staatsangehörigkeit

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
            <zofar:transition target="C3_3"/>
        </zofar:transitions>

hi:

\--------------------------------

C3_3
=

tc:

vn: dsprelt

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Welche Sprache wird in Ihrem Elternhaus normalerweise gesprochen?

is:

it:

st:

ao1: 1: Deutsch

ao2: 2: Deutsch und eine andere Sprache

ao3: 3: eine andere Sprache

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
        <zofar:transition target="A_38" condition="zofar.asNumber(vsbdeba)==1"/>
        <zofar:transition target="A_38a" condition="zofar.asNumber(vsbdeba)==2"/>
        <zofar:transition target="A_38" condition="zofar.isMissing(vsbdeba)"/>    
       </zofar:transitions>

hi:
