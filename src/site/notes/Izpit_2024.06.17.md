---
{"dg-publish":true,"permalink":"/izpit-2024-06-17/","tags":["unfinished"]}
---

# Naloga 1

Transformator ima nazivno moč $S_n = 200\ \text{MVA}$ in nazivni izkoristek $\eta_n = 0{.}98$. Razmerje izgub pri nazivnem obratovalnem stanju je: $\xi_{n} = \frac{P_{Cu,n}}{P_{Fe}} = 3$
Transformator se pri nazivni napetosti in frekvenci pri trajnem obratovanju segreje do nadtemperature: $\Theta_{\text{max,n}} = 100\ \text{K}$

Nato transformator priključimo na omrežje z znižano napetostjo $U = 0{.}8 \cdot U_n$ in povišano frekvenco $f = 1{.}2 \cdot f_n$, pri čemer ostane tok **enak nazivnemu**: $I = I_n$.

Vprašanje: **Do katere nadtemperature $\Theta_{\text{max}}'$ se bo transformator segrel pri trajnem obratovanju v novih razmerah?**

## Rešitev
### 1. Izgube v bakru
Izgube v bakru so sorazmerne kvadratu toka:
$$
P_{Cu}' = P_{Cu,n} \cdot \left( \frac{I}{I_n} \right)^2 = P_{Cu,n}
$$
Ker je $I = I_n$, ostanejo izgube v bakru **nspremenjene**.

### 2. Izgube v železu
Izgube v železu (v jedru) so odvisne od razmerja napetosti in frekvence:
$$
P_{Fe} \propto \left( \frac{U}{f} \right)^2
$$
Zato:
$$
\frac{P_{Fe}'}{P_{Fe}} = \left( \frac{0{.}8 U_n}{1{.}2 f_n} \cdot \frac{f_n}{U_n} \right)^2 = \left( \frac{0{.}8}{1{.}2} \right)^2 = \left( \frac{2}{3} \right)^2 = \frac{4}{9}
$$

### 3. Razmerje nadtemperatur
Ker je nadtemperatura v transformatorju pri trajnem stanju sorazmerna s skupnimi izgubami, velja:

$$
\frac{\Theta'}{\Theta_n} = \frac{P_{\text{izg}}'}{P_{\text{izg,n}}} = \frac{P_{Cu,n} + P_{Fe}'}{P_{Cu,n} + P_{Fe,n}}
$$

Po podatkih iz naloge je:

$$
P_{Cu,n} = 3 \cdot P_{Fe,n}
$$

Zato:

$$
\frac{\Theta'}{\Theta_n} = \frac{3 P_{Fe,n} + \frac{4}{9} P_{Fe,n}}{3 P_{Fe,n} + P_{Fe,n}} = \frac{3 + \frac{4}{9}}{4} = \frac{\frac{31}{9}}{4} = \frac{31}{36}
$$
### 4. Izračun nove nadtemperature
$$
\Theta' = \Theta_n \cdot \frac{31}{36} = 100\ \text{K} \cdot 0{.}861 \approx 86{.}1\ \text{K}
$$
# Naloga 2
Sinhrosnki turbogenerator $S_{n} = 200MVA$, $U_{2n} = 15kV$, $\cos(\varphi_{2n}) = 0.8$, $X_{sr} = 1.4$, $I_{1n} = 300A$ obratuje na togem nazivnem omrežju pri obremenitivi $S' = 100MVA$, $\cos(\varphi_{2})' = 0.6$. Za to obratovalno stanje določite potrebne vzbujalni tok $I_{1}'$ in oba kolesna kota $\delta_{n}$ in $\delta'$. Obvezna tudi skica obeh obratovlanih stanj.
## Izračuni

**1. EMN pri nazivnem stanju:**

$$
E_{0n} = \sqrt{(15\,252)^2 + 336^2} \approx 15\,253\ \text{V}
$$

**2. EMN pri $S' = 100$ MVA:**

$$
I_2' = \frac{100 \cdot 10^6}{\sqrt{3} \cdot 15\,000} \approx 3849\ \text{A}
$$

$$
E_0' = \sqrt{(19\,309)^2 + 3233^2} \approx 19\,601\ \text{V}
$$

**3. Vzbujalni tok:**

$$
I_1' = 300 \cdot \frac{19\,601}{15\,253} \approx 386\ \text{A}
$$

**4. Kolesna kota:**

$$
\delta_n = \arctan\left( \frac{336}{15\,252} \right) \approx 1{.}26^\circ
$$

$$
\delta' = \arctan\left( \frac{3233}{19\,309} \right) \approx 9{.}5^\circ
$$

# Naloga 3

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/izpit-2022-09-01/#naloga-3" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 3
Trifazni asinhronski motor s kratkostično kletko ima podane naslednje nazivne podatke:
$P_n = 15\ \text{kW}$ , $n_n = 576\ \text{min}^{-1}$ , $U_n = 400\ \text{V}$ , $f_n = 50\ \text{Hz}$ , $\cos\varphi_n = 0{.}78$ , $I_n = 34\ \text{A}$ , $P_{tr+vent} = 100\ \text{W}$ , $\frac{I_Z}{I_n} = 7$ , $\frac{M_Z}{M_n} = 1{.}8$ , Vezava: $\Delta$

## a) Določite: izkoristek, slip, nazivni navor, ter vsoto izgub v statorju (Cu + Fe)
### 1. Sinhronska hitrost $n_s$
Za motor z $n_n = 576\ \text{min}^{-1}$ in frekvenco $f = 50\ \text{Hz}$ domnevamo, da je $n_s = 600\ \text{min}^{-1}$, kar ustreza **$p = 5$ polparom**:

$
n_s = \frac{60 \cdot f}{p_p} = \frac{60 \cdot 50}{5} = 600\ \text{min}^{-1}
$
### 2. Slip (zdrs)
$
s = \frac{n_s - n_n}{n_s} = \frac{600 - 576}{600} = \frac{24}{600} = 0{.}04 = 4\%
$
### 3. Mehanska moč in nazivni navor $M_n$
Mehanska moč na gredi:
$
P_{meh} = P_n = 15\,000\ \text{W}
$
Nazivni navor:
$
M_n = \frac{P_{meh}}{\omega} = \frac{P_{meh}}{2\pi \cdot \frac{n_n}{60}} = \frac{15\,000}{2\pi \cdot \frac{576}{60}} = \frac{15\,000}{60{.}32} \approx 248{.}8\ \text{Nm}
$
### 4. Vhodna moč $P_{cel}$
$
P_{cel} = \sqrt{3} \cdot U \cdot I \cdot \cos\varphi = \sqrt{3} \cdot 400 \cdot 34 \cdot 0{.}78 \approx 18\,393\ \text{W}
$
### 5. Izkoristek $\eta$
Izkoristek je razmerje med močjo na gredi in električno dovodeno močjo:
$
\eta = \frac{P_n}{P_{cel}} = \frac{15\,000}{18\,393} \approx 0{.816} = 81{.6}\%
$
### 6. Skupne izgube v statorju
Skupne izgube so:
$
P_{izg} = P_{cel} - P_n = 18\,393 - 15\,000 = 3\,393\ \text{W}
$
Ker je del teh izgub trenje in ventilacija ($P_{tr+vent} = 100\ \text{W}$), so izgube v statorju:
$
P_{s,cu} + P_{s,fe} = 3\,393 - 100 = 3\,293\ \text{W}
$
## b) Kolikšna sta zagonski tok in navor, če motor zaganjamo v vezavi $Y$ pri 25 % nazivni napetosti?
### 1. Zagonski tok
Pri vezavi $\Delta$ je nazivni tok $I_n = 34\ \text{A}$. Zagonski tok pri tej vezavi bi bil:
$
I_Z^{\Delta} = 7 \cdot I_n = 238\ \text{A}
$
Če motor zaženemo v **vezavi $Y$**, potem je napetost na navitju **nižja za faktor $\sqrt{3}$**, tok pa prav tako:
$
I_Z^Y = \frac{I_Z^{\Delta}}{\sqrt{3}} \approx \frac{238}{1{.}732} \approx 137{.}4\ \text{A}
$
Če je napetost **znižana na 25 %**:
$
I_Z = 0{.}25 \cdot 137{.}4 \approx 34{.}4\ \text{A}
$
### 2. Zagonski navor

Zagonski navor pri nazivni napetosti v vezavi $\Delta$ je podan z razmerjem:

$
M_{Z,\Delta} = 1.8 \cdot M_n = 1.8 \cdot 248.8 = 497.6\ \text{Nm}
$

Pri zaganjanju v **vezavi $Y$** in znižani napajalni napetosti na **25 %** nazivnega nivoja ($0.25 \cdot U_L$), je napetost na **faznem navitju**:

$
U_{Y,25\%} = \frac{0.25 \cdot U_n}{\sqrt{3}} = \frac{U_{\Delta}}{4 \cdot \sqrt{3}}
$

Ker je zagonski navor sorazmeren s kvadratom fazne napetosti, se novi navor zmanjša za:

$
M_{Z,Y25\%} = M_{Z,\Delta} \cdot \left(\frac{0.25}{\sqrt{3}}\right)^2 = 497.6 \cdot 0.0208 \approx 10.4\ \text{Nm}
$

</div></div>



# Naloga 4
Enosmerni motor s tujim vzbujanjem ima nazivne podatke: $P_{n} = 22kW$, $U_{n} = 300V$, $n_{n} = 300\text{min} ^{-1}$, $R_{i} = 0.08\Omega$, $\eta = 0.92$. S kolikšno vtilno hitrostjo moramo poganjati stroj, da na nazivnem omrežju deluje kot generator z obremnitvijo, pri kateri je $I'_{i} = I_{i,n}$? Padec napetosti na ščetkah ni potrebno upoštevati.

## Rešitev

### 1. Nazivni tok:

$$
I_n = \frac{P_n}{\eta \cdot U_n} = \frac{22\,000}{0{.}92 \cdot 300} \approx 79{.}71\ \text{A}
$$

### 2. EMN v motorju (nazivno stanje):

$$
E_n = U_n - I_n \cdot R_i = 300 - 79{.}71 \cdot 0{.}08 \approx 293{.}62\ \text{V}
$$

### 3. EMN v generatorju (obratovalno stanje):

$$
E' = U_n + I_n \cdot R_i = 300 + 79{.}71 \cdot 0{.}08 \approx 306{.}38\ \text{V}
$$

### 4. Razmerje hitrosti:

$$
\frac{n'}{n_n} = \frac{E'}{E_n} = \frac{306{.}38}{293{.}62} \approx 1{.}0434
$$

$$
n' = 300 \cdot 1{.}0434 \approx 313\ \text{min}^{-1}
$$