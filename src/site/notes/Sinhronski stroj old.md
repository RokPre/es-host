---
{"dg-publish":true,"permalink":"/sinhronski-stroj-old/","tags":["unfinished"]}
---

# Shema


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# 50%

</div>



==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


Na zgornji sliki vidi osnovno shemo rotorja sinhronskega stroja s izrazenimi poli. S oranzno so obarvana navitja, s zeleno pa potek magnetnega polja. Na sredinin rotorja vidi napajalno navitje, ki je povezano s ostalim preko krtack.

Obstajajo rotrji s neizrazenimi poli, ter rotorji s trajnimi magneti.

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# 50%

</div>



==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>

# Hitrost vrtenja
Tipicna lastnost sinhronskih strojev je, da se vrtijo v sinhronizmu s vrtilnim magnetnim poljem.
$$n = \frac{f}{p}$$
V zgornji enacbi je $n$ hitrost vrtenja v $\frac{vrt}{min}$, $f$ je frekvenca omrezja in $p$ je stevilo polovih parov v rotorju.

# Statorsko navitje
Imamo razlicne opcije kako lahko navije tauljave v statorju. V statorju je lahko ogromno tuljav, vendar se jih vedno da modelirati samo s 3-mi, ko imamo trifazni izhod.

Ce hocemo omrezno frekvenco $50Hz$, in imamo turbino, ki se vrti s 600 vrtnjaji na minuto, potem potrebujemo $p = 60\frac{f}{n} = 60\frac{50}{600} =5$. Torej potrebujemo 5 polovih parov. Nizja kot je hitrost vrtenja turbine/osi, vec polovih parov potrebuje da dosezemo omrezno frekvenco.
## Vezavi zvezda

> [!image] Title
> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>

> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


# Sinhroniziranje

> [!image]
> Sinhronizacija je postopek, ki je potreben pri priklopu sinhronskega stroja na omrezno napetost. Izpoljneni morajo biti naslednji pogoji: izhodna napetost troja se mora ujemati s omrezno napetostjo(amplituda, faza, frekvenca). To dosezemo s primernimi meritvami, in s stikalom, ki ga sklenemom, ko so vsi pogoji izpounjeni. 
> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


# Generatorsko obratovanje
Na spodnjem grafu je vidna karakteristika sinhronskega stroja, ki se vrti s konstantno hitrojstijo. $I_{r}$ je magnetilni tok, ta tece po tuljavah na rotorju, na $y$ osi imamo na inducirano napetost. Ker se stroj vrti s konstantno hitrostjo, je induciranan napetost odvisna samo od toka. 

![[magic formula\|magic formula]]

$U_{sN}$ je nazivna napetost. Do nazivne napetosti lahko pridemo na dva razlicna nacina s tokom rotorja $I_{r}$. Najprej je lahko tok tak, da dobimo napetost $U_{N}$ s pommocjo k.z.r., s drugim nacinom lahko dobimo $U_{N}$ s k.p.t.. Pogosto se uporablje k.z.r. ker je linearna premica. 


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# 60%

</div>



==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


Spodnja slika prikazuje razlicne velicina v odvisnosti od casa. Vidimo da je flux $\phi$ vzporeden s tokom $I_{r}$, kar pomeni da stav fazi. Inducirana napetost pa zaostaja za $90^{\circ}$, saj je v izracunu za napetost prisoten odvod, ki spremeni $\sin$ v $\cos$.


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


## Nadomestno vezje
$$
E_{f} =  U + I X_{s} = U + IX_{a} +IX_{\sigma}
$$
Zgornja enacba predstavlja napetostne razmere v sinhronem stroju. Uporabimo jo za izpeljavo nadomestne sheme.
- $E_{f}$ je fiktivna inducirana napetost, ta je prisotna le v prostem teku. Je simbolicni vir napetosti, ki je posledica indukcije.
- $U$ je napetost omrezja, ta je togo in se ne spreminja,
- $X_{s}$ je sinhronska relaktanca, ko jo pomnozimo s tokom $I$ dobimo padec napetosti na notranji polni upornosti,
- $X_{a}$ je relaktanca, ki predstavlja vpliv reaklcije indukta na statorski strani,
- $X_{\sigma}$ relaktanca zaradi rasutja magnetnega polja.

Na nadomestnem vezju nimamo predstavljenih ohmskih izgub, saj so te zanemarljivo majhne v primerjavi s reaktance navitja.



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>

## Prosti tek
V prostem teku ni noeben obremenitnve $Z_{b} = 0$. Posledicno je tok $I = 0$. Ker ni toka, tudi ni padca napetosti na reluktancah in velja $E_{f} = U$.

### Preuzbujanje
Ce imamo stroj, ki je povezan na omrezno napetost, in obratuje brez obremenitve, ter mu nato povisamo vzbujani tok se bo posledicno zvisala $E_{f}$, vendar $U$ bo ostal enak, saj je ta dolocen s strani omrezja. Ker je sedaj razlika med $E_{f} - U = \Delta U$ se pojavi padec napetosti. Ker se ta padec napetosti pozna na tuljavi $X_{s}$, bo stekel tok. Ta tok bo zaostajal za $90 ^{\circ}$ od napetosti in $180 ^{\circ}$ za vzbujalnim tokom $I_{v}$. $I = \frac{\Delta U}{X_{s}}$

V tem primeru omrezje vidi stroj kot kondenzator.

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


### Poduzbujanje
Zmanjsamo vzbujanlni tok $I_{v}$, posledicno se zmanja $E_{f}$ ter se ustvari padec napetosti $\Delta U$. Ker je sedaj $E_{f} \lt U$, tece tok v drugo smer kot v primeru ko je stroj preuzbujan. To pomeni, da ima tok negativni predznak, in je tudi vbrnjen v drugo smer na kazalcnem diagramu. 

Posledicno ga omrezje vidi kot dusilko. Temu drugace recemo "*kompenzator jalove energije*".

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>


[[Shift transformers\|Shift transformers]]

## Kazalcni diagram obremenitve


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements


</div></div>


- $E_{0}$ je namisljena napetost, ki v resnici ne obstaja, je pa nam v pomoc, da si lazje razlozimo delovnaje stroja in njegove izgube,
- $I_{1}$ je vzbujalni tok,
- $I_{10}$ je vzbujanli tok, od katerega je odstet namisljeni tok, ki "nastane" zaradi reakcije indukta in izgub v navitju.
- $I_{1a}$ je rezultat padca toka $I_{1}$ za $I_{2}'$, zaradi reakcije indukta,
- $E_{a}$ je navidezni induktivni padec zaradi bremenskega toka $I_{2}$. Za $X_{a}$ ponazorimo delovanje reakcije indukta. 
- $I_{2 \sigma}'$ je za koliko se zmanjsa vzbujalni tok, zaradi izgub v navitjih.
- $I_{2}$ je tok na sekundarni strani, ki ga doloca breme,
- $I_{2}'$ je tok zaradi reakcije indukta,
- $\delta$ je kolesni kot
- $\varphi_{2}$ je fazni kot med $U_{2}$ in $I_{2}$, ki je odvisen od karakteristike bremena. $\cos(\varphi_{2})$.
- $U_{2}$ je izhodna napetost generatorja.
- $E_{2}$ je inducirana napetost na statorju. Od nje odstejemo izgube navitji in dobimo izhodno napetost.
- $X_{a}$ je reaktanca zaradi reakcije indukta,
- $X_{\sigma2}$ je reaktanca stresanega magnetnega polja. $\omega L_{\sigma_{2}}$.
- $R_{2}$ je upornost statorskega navitja.
- $\gamma$

# Kolesni kot


> [!image]
> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>

> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>

> 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Excalidraw Data
## Text Elements


</div></div>



> [!image]
> $1.\,$ Ko imamo zelezo in magnet se tadva hoceta poravnati. To stanje je vidno na levi strani slike. Na desni je pa vidno stanje, ko s silo potiskamo magnet, v tem primeru je to rotor, ki se rotira s pomocjo pare in turbine. Ko potiskamo s to silo se pojavi nek kot med statorjem in rotorjem. Temu pravimo kolesni kot.
> $2.\,$ Kolesni kot je pokazatelj obrementve rotorja. Ce bi prevec obremenili sinhronski stroj, bi se silnice magnetnega polja pretrgale, in bi stroj padel iz sinhronizma.
> $3.\,$ Za razliko od leve slike je tokrat padec napetosti obrnjen v drugo smer. Posledicno je tudi tok obrnjen v drugo smer, kar pomeni da je stroj v motornem delovanju. Kar pomeni da trosi elektricno energijo.




## Obremenitev
### Delovana obremenitev



### Reakcija indukta