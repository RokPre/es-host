---
{"dg-publish":true,"permalink":"/izpit-2022-09-01/","tags":["unfinished"]}
---

# Naloga 1

Transformator ima izgube v navitju $P_{cu} = 1750\ \text{W}$ in izgube v prostem teku $P_0 = 350\ \text{W}$. Njegova toplotna časovna konstanta znaša $T = 2\ \text{h}$. Pri nespremenjeni napajalni napetosti transformator obremenimo z **dvakratnim nazivnim tokom**.

Po kolikšnem času mora izklopiti **termična zaščita**, da ne pride do pregrevanja preko dopustne (nazivne) temperature stroja?


## Rešitev

Obremenitev transformatorja je:

$$
x = \frac{I}{I_n} = 2
$$

Ker so izgube v navitju odvisne od kvadrata toka, se povečajo za faktor $x^2 = 4$. Skupne izgube transformatorja pri novi obremenitvi so:

$$
P_{\text{izg}}' = P_0 + x^2 \cdot P_{cu} = 350 + 4 \cdot 1750 = 7450\ \text{W}
$$

Temperatura transformatorja v času $t$ narašča po eksponentni funkciji:

$$
\Theta(t) = \Theta_{\max}' \cdot \left(1 - e^{-t/T} \right)
$$

Zanima nas čas $t_0$, pri katerem nova temperatura doseže **nazivno dopustno temperaturo**, torej:

$$
\Theta(t_0) = \Theta_{\max, n}
$$

Pri tem pa velja:

$$
\frac{\Theta_{\max}'}{\Theta_{\max, n}} = \frac{1 + x^2 \cdot \xi}{1 + \xi}
$$

kjer je $\xi$ razmerje med izgubami v navitju in izgubami v železu (prostem teku):

$$
\xi = \frac{P_{cu}}{P_0} = \frac{1750}{350} = 5
$$

Zato:

$$
\frac{\Theta_{\max}'}{\Theta_{\max, n}} = \frac{1 + 4 \cdot 5}{1 + 5} = \frac{21}{6} = 3{.}5
$$

Torej se nova maksimalna temperatura dvigne na:

$$
\Theta_{\max}' = 3{.}5 \cdot \Theta_{\max, n}
$$

Vstavimo v enačbo za naraščanje temperature:

$$
\Theta(t_0) = \Theta_{\max}' \cdot \left(1 - e^{-t_0/T} \right) = \Theta_{\max, n}
$$

Delimo z $\Theta_{\max}'$:

$$
\frac{\Theta_{\max, n}}{\Theta_{\max}'} = 1 - e^{-t_0/T}
$$

Izoliramo eksponentni člen:

$$
e^{-t_0/T} = 1 - \frac{1}{3{.}5} = \frac{2{.}5}{3{.}5} = \frac{5}{7}
$$

Logaritemsko:

$$
-\frac{t_0}{T} = \ln\left(\frac{5}{7}\right) \quad \Rightarrow \quad t_0 = -T \cdot \ln\left(\frac{5}{7}\right)
$$

Vstavimo $T = 2\ \text{h}$:

$$
t_0 = -2 \cdot \ln\left(\frac{5}{7}\right) \approx -2 \cdot (-0{.}3365) = 0{.}673\ \text{h} \approx 40{.}4\ \text{min}
$$

**Termična zaščita mora izklopiti transformator najpozneje po $40{.}4\ \text{min}$**, da ne pride do preseganja dopustne nazivne temperature.

# Naloga 2

Sinhronski turbogenerator ima naslednje nazivno podane podatke: $S_n = 10\ \text{MVA}$, $U_{2n} = 3000\ \text{V}$, $f_n = 50\ \text{Hz}$, $\cos\varphi_{2n} = 0{.}7$, $X_s = 2\ \Omega$ (sinhronska reaktanca), $I_{vn} = 100\ \text{A}$. Generator deluje na **togo omrežje** z napetostjo $U_2 = U_{2n}$, vzbujanje in dotok mehanske moči sta nastavljena tako, da je generator obremenjen z **nazivnim tokom** $I_2 = I_{2n} = 100\ \text{A}$, vendar z faktorjem moči $\cos\varphi_2 = 1$ (brez jalove moči, ohmska obremenitev).

## a) Električna moč oddana v omrežje
Pri $\cos\varphi = 1$ velja:

$$
P = \sqrt{3} \cdot U_2 \cdot I_2 \cdot \cos\varphi = \sqrt{3} \cdot 3000 \cdot 100 \cdot 1 = 519\,615\ \text{W} \approx 519{.}6\ \text{kW}
$$

Torej je oddana moč generatorja v omrežje $P_{el} = 519{.}6\ \text{kW}$.

## b) Kolesni kot
Za sinhronski generator, ki napaja togo omrežje in ima $\cos\varphi = 1$, uporabimo razmerje iz kazalčnega diagrama:

Kazalec $U_2$ je vodilni (leži na realni osi), tok $I_2$ je v fazi z napetostjo (ker $\varphi = 0$), reaktiven padec napetosti $jX_s I_2$ pa zavije navzgor (90° zamik), kar povzroči, da je $E_0$ napetost nad $U_2$ z navidezno rotacijo za kot $\delta$.

Formula za kolesni kot:

$$
\tan\delta = \frac{I_2 X_s \cdot \cos\varphi}{U_2 + I_2 X_s \cdot \sin\varphi}
$$

Pri $\cos\varphi = 1$ in $\sin\varphi = 0$ postane:

$$
\tan\delta = \frac{I_2 X_s}{U_2} = \frac{100 \cdot 2}{3000} = \frac{200}{3000} = 0{.}0667
$$

Torej:

$$
\delta = \arctan(0{.}0667) \approx 3{.}82^\circ
$$
Kolesni kot je: $3{.}82^\circ$ 

## c) Potreben vzbujalni tok
Najprej izračunamo inducirano EMN generatorja $E_0$ iz kazalčnega trikotnika:

$$
E_0 = \sqrt{(U_2 + I_2 X_s \cdot \sin\varphi)^2 + (I_2 X_s \cdot \cos\varphi)^2}
$$

Ker je $\sin\varphi = 0$, $\cos\varphi = 1$:

$$
E_0 = \sqrt{U_2^2 + (I_2 X_s)^2} = \sqrt{3000^2 + (100 \cdot 2)^2} = \sqrt{9\,040\,000}
$$

$$
E_0 \approx 3006\ \text{V}
$$

Nazivna EMN v režimu z $\cos\varphi_n = 0{.}7$:

$$
E_{0n} \approx 3163\ \text{V} \quad \text{(podana)}
$$

Iz razmerja:

$$
\frac{I_v}{I_{vn}} = \frac{E_0}{E_{0n}} = \frac{3006}{3163} \approx 0{.}95
$$

$$
I_v = 0{.}95 \cdot I_{vn} = 0{.}95 \cdot 100 = 95{.}0\ \text{A}
$$

Potreben vzbujalni tok je $I_v \approx 95{.}0\ \text{A}$

# Naloga 3
Trifazni asinhronski motor s kratkostično kletko ima podane naslednje nazivne podatke:
$P_n = 15\ \text{kW}$ , $n_n = 576\ \text{min}^{-1}$ , $U_n = 400\ \text{V}$ , $f_n = 50\ \text{Hz}$ , $\cos\varphi_n = 0{.}78$ , $I_n = 34\ \text{A}$ , $P_{tr+vent} = 100\ \text{W}$ , $\frac{I_Z}{I_n} = 7$ , $\frac{M_Z}{M_n} = 1{.}8$ , Vezava: $\Delta$

## a) Določite: izkoristek, slip, nazivni navor, ter vsoto izgub v statorju (Cu + Fe)
### 1. Sinhronska hitrost $n_s$
Za motor z $n_n = 576\ \text{min}^{-1}$ in frekvenco $f = 50\ \text{Hz}$ domnevamo, da je $n_s = 600\ \text{min}^{-1}$, kar ustreza **$p = 5$ polparom**:

$$
n_s = \frac{60 \cdot f}{p_p} = \frac{60 \cdot 50}{5} = 600\ \text{min}^{-1}
$$
### 2. Slip (zdrs)
$$
s = \frac{n_s - n_n}{n_s} = \frac{600 - 576}{600} = \frac{24}{600} = 0{.}04 = 4\%
$$
### 3. Mehanska moč in nazivni navor $M_n$
Mehanska moč na gredi:
$$
P_{meh} = P_n = 15\,000\ \text{W}
$$
Nazivni navor:
$$
M_n = \frac{P_{meh}}{\omega} = \frac{P_{meh}}{2\pi \cdot \frac{n_n}{60}} = \frac{15\,000}{2\pi \cdot \frac{576}{60}} = \frac{15\,000}{60{.}32} \approx 248{.}8\ \text{Nm}
$$
### 4. Vhodna moč $P_{cel}$
$$
P_{cel} = \sqrt{3} \cdot U \cdot I \cdot \cos\varphi = \sqrt{3} \cdot 400 \cdot 34 \cdot 0{.}78 \approx 18\,393\ \text{W}
$$
### 5. Izkoristek $\eta$
Izkoristek je razmerje med močjo na gredi in električno dovodeno močjo:
$$
\eta = \frac{P_n}{P_{cel}} = \frac{15\,000}{18\,393} \approx 0{.816} = 81{.6}\%
$$
### 6. Skupne izgube v statorju
Skupne izgube so:
$$
P_{izg} = P_{cel} - P_n = 18\,393 - 15\,000 = 3\,393\ \text{W}
$$
Ker je del teh izgub trenje in ventilacija ($P_{tr+vent} = 100\ \text{W}$), so izgube v statorju:
$$
P_{s,cu} + P_{s,fe} = 3\,393 - 100 = 3\,293\ \text{W}
$$
## b) Kolikšna sta zagonski tok in navor, če motor zaganjamo v vezavi $Y$ pri 25 % nazivni napetosti?
### 1. Zagonski tok
Pri vezavi $\Delta$ je nazivni tok $I_n = 34\ \text{A}$. Zagonski tok pri tej vezavi bi bil:
$$
I_Z^{\Delta} = 7 \cdot I_n = 238\ \text{A}
$$
Če motor zaženemo v **vezavi $Y$**, potem je napetost na navitju **nižja za faktor $\sqrt{3}$**, tok pa prav tako:
$$
I_Z^Y = \frac{I_Z^{\Delta}}{\sqrt{3}} \approx \frac{238}{1{.}732} \approx 137{.}4\ \text{A}
$$
Če je napetost **znižana na 25 %**:
$$
I_Z = 0{.}25 \cdot 137{.}4 \approx 34{.}4\ \text{A}
$$
### 2. Zagonski navor

Zagonski navor pri nazivni napetosti v vezavi $\Delta$ je podan z razmerjem:

$$
M_{Z,\Delta} = 1.8 \cdot M_n = 1.8 \cdot 248.8 = 497.6\ \text{Nm}
$$

Pri zaganjanju v **vezavi $Y$** in znižani napajalni napetosti na **25 %** nazivnega nivoja ($0.25 \cdot U_L$), je napetost na **faznem navitju**:

$$
U_{Y,25\%} = \frac{0.25 \cdot U_n}{\sqrt{3}} = \frac{U_{\Delta}}{4 \cdot \sqrt{3}}
$$

Ker je zagonski navor sorazmeren s kvadratom fazne napetosti, se novi navor zmanjša za:

$$
M_{Z,Y25\%} = M_{Z,\Delta} \cdot \left(\frac{0.25}{\sqrt{3}}\right)^2 = 497.6 \cdot 0.0208 \approx 10.4\ \text{Nm}
$$
# Naloga 4
Enosmerni motor s tujim vzbujanjem ima naslednje nazivne podatke:
$P_n = 25\ \text{kW}$ , $n_n = 3000\ \text{min}^{-1}$ , $R_r = 0{.}05\ \Omega$ , $\eta_n = 0{.}95$ , $U_n = 230\ \text{V}$ , Padec napetosti na ščetkah: $\Delta U_{šč} = 2\ \text{V}$
Motor naj deluje kot **generator**, pri čemer je obremenjen s tokom:

$$
I_1 = \frac{1}{4} I_{nL}
$$

Želimo določiti **vrtilno hitrost** $n$, pri kateri mora delovati, da je napetost na sponkah enaka nazivni ($U = U_n$).

## Rešitev
### 1. Določimo nazivni tok
Pri nazivni moči $P_n$ in izkoristku $\eta_n$, je električna vhodna moč motorja:

$$
P_{in} = \frac{P_n}{\eta_n} = \frac{25\,000}{0{.}95} \approx 26\,316\ \text{W}
$$

Nazivni tok motorja:

$$
I_{nL} = \frac{P_{in}}{U_n} = \frac{26\,316}{230} \approx 114{.}42\ \text{A}
$$
### 2. Tok generatorja
Generator je obremenjen s četrtino nazivnega toka:

$$
I_1 = \frac{1}{4} \cdot 114{.}42 \approx 28{.}6\ \text{A}
$$
### 3. Napetostna enačba generatorja
Za enosmerni **generator** velja (vključno s ščetkami):
$$
E = U + I_1 \cdot R_r + \Delta U_{šč}
$$
Vstavimo znane vrednosti:
$$
E = 230\ \text{V} + 28{.}6 \cdot 0{.}05 + 2 = 230 + 1{.}43 + 2 = 233{.}43\ \text{V}
$$
### 4. Uporabimo linearno sorazmernost $E \sim n$

Ker je $E \sim n$ pri nespremenjenem vzbujanju, velja:

$$
\frac{E}{E_n} = \frac{n}{n_n}
$$

V nazivnem režimu motorja:

$$
E_n = U_n - I_{nL} \cdot R_r - \Delta U_{šč} = 230 - 114{.}42 \cdot 0{.}05 - 2 = 230 - 5{.}72 - 2 = 222{.}28\ \text{V}
$$

Zato:

$$
\frac{233{.}43}{222{.}28} = \frac{n}{3000} \quad \Rightarrow \quad n = 3000 \cdot \frac{233{.}43}{222{.}28} \approx 3149\ \text{min}^{-1}
$$

Stroj mora obratovati pri hitrosti približno: $n \approx 3149\ \text{min}^{-1}$