---------------------

end
=

tc: 

vn: countvar

qt: 

hl:

in: 

q: !!Vielen Dank für Ihre Teilnahme! !! 
	Sie haben uns mit Ihren Antworten sehr weitergeholfen. 
	Ihre Rückmeldungen helfen uns dabei eine Studierendenbefragung zu konzipieren, die die Situation verschiedener Studierendengruppen in Deutschland abbildet. Vielen Dank!

q1: ##[Adressabfrage](Verlinkung zur Adressabfrage für Target-Group)##

q2: ##[Adressabfrage](Verlinkung zur Adressabfrage)##

is: 

it: 

st:

ao: 

mv: 

ka: 

vc: 
q1 visible if countvar==1

q2 visible if countvar==0

av: 

kh: 

fv: 

hv: 

fo: 

tr: 

<zofar:transitions>
    <zofar:transition target="Addon_1" condition="(zofar.asNumber(vsbtyp11)==1 or zofar.asNumber(vsbtyp12)==1) and (countvar==1) "/>
    <zofar:transition target="Addon_3" condition="(zofar.asNumber(vsbtyp11)==1 or zofar.asNumber(vsbtyp12)==1) and (countvar==0) "/>
</zofar:transitions>

hi: 
countvar == 0 if ausspielbare Incentives nicht mehr vorhanden
countvar == 1 if ausspielbare Incentives vorhanden


---------------------

end-prom
=

tc: 

vn: 

qt: 

hl:

in: Herzlichen Dank, dass Sie sich die Zeit genommen haben, um an unserer Befragung teilzunehmen. Sie haben angegeben, dass Sie derzeit promovieren. Da wir mit unserer Befragung vor allem  
Studierende adressieren, richten sich alle weiteren Fragen lediglich an diese Gruppe. 

q: 

is: 

it: 

st:

ao: 

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



