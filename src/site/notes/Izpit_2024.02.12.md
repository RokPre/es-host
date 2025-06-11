---
{"dg-publish":true,"permalink":"/izpit-2024-02-12/","tags":["unfinished"]}
---

![Izpit 2024.02.12.1.webp](/img/user/Attachments/izpiti/Izpit%202024.02.12.1.webp)
# Naloga 1
Trifazni transformator z podatki $S_{n} = 20kVA$, $U_{1n} = 10kV$, $U_{2n} = 0.4kV$, $f_{n} = 50Hz$ ima na sekundarni strani med sponkami b in n priključeno ohmsko breme z upornostjo $R_{b} = 20\Omega$.

## a) Kolikšen tok teče v ničlovodu in kakšna moč se troši na bremenu?
Medfazna napetost na sekundarni strani:
$$
U_{2n} = 400\ \text{V} \quad \Rightarrow \quad U_{2f} = \frac{400}{\sqrt{3}} \approx 230\ \text{V}
$$
Tok v bremenu:
$$
I_b = \frac{U_{2f}}{R_b} = \frac{230}{20} = 11{.}5\ \text{A}
$$
Ker je breme priključeno med eno fazo (b) in ničlo, teče ves tok $I_b$ skozi ničlovod. Torej:

Porabljena moč:
$$
P_b = U_{2f} \cdot I_b = 230 \cdot 11{.}5 = 2645\ \text{W}
$$
## b) Določite oznako (vezavo in fazno številko) transformatorja
Dyn7

# Naloga 2
Sinhrosnki turbo generator $S_{n} = 10MVA$, $U_{2n} = 3000V$, $50Hz$, $\cos(\varphi_{2n}) = 0.8$, $X_{sr} = 1.6$, $I_{1n} = 150A$ obratuje ne togem nazivnem omrežju. Dotok pare na turbino in vzbujanje sta nastavljena tako, da je generator obremenejen z nazivnim tokom pri $\cos(\varphi_{2}) = 1$. Izračunajte moč, ki jo generator daje v omrežje, kolesni kot in vzbujalni tok (obvezna skica kazalčnega diagrama).

$$
I_{2n} = \frac{S_n}{\sqrt{3} \cdot U_{2n}} = \frac{10\,000\,000}{\sqrt{3} \cdot 3000} \approx 1924{.}5\ \text{A}
$$


## 2. Aktivna moč v omrežje $P_{el}$

$$
P_{el} = \sqrt{3} \cdot U_2 \cdot I_2 \cdot \cos\varphi = \sqrt{3} \cdot 3000 \cdot 1924{.}5 \cdot 1 \approx  10\ \text{MW}
$$

## 3. Kolesni kot $\delta$

Uporabimo formulo:

$$
\tan\delta = \frac{I_2 \cdot X_{sr} \cdot \cos\varphi}{U_2 + I_2 \cdot X_{sr} \cdot \sin\varphi}
$$

Ker je $\cos\varphi = 1$ in $\sin\varphi = 0$, dobimo:

$$
\tan\delta = \frac{1924{.}5 \cdot 1{.}6 \cdot 1}{3000 + 0} = \frac{3079{.}2}{3000} = 1{.}0264
$$

$$
\delta = \arctan(1{.}0264) \approx 45{.}8^\circ
$$
## 4. Izračun $E_0'$ za $\cos\varphi = 1$

$$
E_0' = \sqrt{(U_2 + I_2 \cdot X_{sr} \cdot \sin\varphi)^2 + (I_2 \cdot X_{sr} \cdot \cos\varphi)^2}
$$

$$
E_0' = \sqrt{(3000)^2 + (1924{.}5 \cdot 1{.}6)^2} = \sqrt{9\,000\,000 + 9\,486\,118{.}4}  \approx 4300{.}7\ \text{V}
$$

## 5. Izračun $E_{0n}$ iz referenčnega stanja ($I_{2n}$, $\cos\varphi = 0.8$)

$$
\sin\varphi = \sqrt{1 - 0{.}8^2} = 0{.}6
$$

$$
E_{0n} = \sqrt{(3000 + 1924{.}5 \cdot 1{.}6 \cdot 0{.}6)^2 + (1924{.}5 \cdot 1{.}6 \cdot 0{.}8)^2}
$$

$$
E_{0n} \approx 5432\ \text{V}
$$

## 6. Razmerje za vzbujalni tok:

$$
\frac{I_1'}{I_{1n}} = \frac{E_0'}{E_{0n}} = \frac{4300{.}7}{5432} \approx 0{.}791
$$

$$
I_1' = 0{.}791 \cdot 150\ \text{A} \approx 118{.}7\ \text{A}
$$
# Naloga 3
Trifazni asinhronski motor s kratkostično kletko ima naslednje podatke:  
$P_n = 15\ \mathrm{kW}$, $U_n = 400\ \mathrm{V}$, $f = 50\ \mathrm{Hz}$,  
$I_n = 32\ \mathrm{A}$, $n_n = 570\ \mathrm{min}^{-1}$, $\cos\varphi = 0{.}80$,  
$\frac{M_{z}}{M_n} = 1{.}6$, $\frac{M_{max}}{M_n} = 2{.}8$, $\frac{I_z}{I_n} = 6$  
vezava: trikot.

### a) Določite nazivni navor, nazivni slip in maksimalni izkoristek motorja.
$$
M = \frac{P\cdot {60}}{2\pi n_{n}} = \frac{15000\cdot 60}{2\cdot \pi \cdot 570} = 251.3 Nm
$$
$$
s_{n} = \frac{n_{s} - n_{r}}{n_{s}} = \frac{600 - 570}{600} = 0.05 = 5\% 
$$
$$
\eta = \frac{P_{meh}}{P_{el}} = \frac{15000W}{400V \cdot 32A \cdot \sqrt{ 3 }\cdot 0.8} = 0.845\ldots  = 84.5\%
$$
### b) Kolikšna sta zagonski tok in zagonski navor, če motor zaganjamo v vezavi **zvezda**?
#### 1. Zagonski navor pri vezavi trikot

Podan je relativni zagonski navor:

$$
\frac{M_z^\Delta}{M_n} = 1{.}6 \quad \Rightarrow \quad M_z^\Delta = 1{.}6 \cdot M_n = 1{.}6 \cdot 251{.}3 \approx 402{.}1\ \text{Nm}
$$
#### 2. Navor pri zaganjanju v vezavi zvezda

V zvezdi je fazna napetost:

$$
U_Y = \frac{U_\Delta}{\sqrt{3}} = \frac{400}{\sqrt{3}} \approx 230{.}94\ \text{V}
$$

Ker je navor sorazmeren s kvadratom napetosti:

$$
M_z^Y = M_z^\Delta \cdot \left( \frac{U_Y}{U_\Delta} \right)^2 = 402{.}1 \cdot \left( \frac{230{.}94}{400} \right)^2 \approx 402{.}1 \cdot 0{.}333 \approx \boxed{133{.}9\ \text{Nm}}
$$
#### 3. Zagonski tok v vezavi zvezda

Zagonski tok v trikot:

$$
I_z^\Delta = I_n \cdot \frac{I_z}{I_n} = 6 \cdot 32 = 192\ \text{A}
$$

Zagonski tok je sorazmeren z navorom (v prvi aproksimaciji):

$$
I_z^Y = I_z^\Delta \cdot \frac{M_z^Y}{M_z^\Delta} = 192 \cdot \frac{133{.}9}{402{.}1} \approx \boxed{63{.}9\ \text{A}}
$$
### c) Kolikšen je slip motorja v trenutku zagona v vezavi **trikot** in kolikšen v vezavi **zvezda**?
Slip je 1 saj ob času zagona rotor stoji.

# Naloga 4
Enosmerni motor s serijskim vzbujanjem ima nazivne podatke: $U_{n} = 400V$, $P_{n} = 10kW$, $n_{n} = 1200\text{min}^{-1}$. Poganja delovni stroj, katerega bremenski navor je neodvisen od vrtilne hitrosti $M_{b} = konst$. Pri obratovnaju na nazivnem omrežju je motor nazivno obremnenjen in se nahaja še v nenasičenem področju magnetilne krivulje. Kakšna bo vrtilna hitrsot motorja, če se napajalna napetost zniža za $30\%$?
## Rešitev

$$
\frac{n'}{n_{n}} = \frac{E'}{E_{n}} =0.7\Rightarrow 1200\cdot 0.7 = 840 \text{min}^{-1}
$$


![izpit 2024.02.12.2.webp](/img/user/Attachments/izpiti/izpit%202024.02.12.2.webp)
# Naloga 5

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/izpit-2024-09-03/#naloga-5" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 5
Primarno navitje enofaznega transformatorja s podano napisno tablico je priključeno na nazivno napajanje. Napisna tablica:

| Parameter             | Vrednost       |
| --------------------- | -------------- |
| **Type**              | S              |
| **Class**             | CL. H150       |
| **Cat. No.**          | 15S2H          |
| **Rating**            | 15 kVA         |
| **HV (High Voltage)** | 240 V / 64.6 A |
| **LV (Low Voltage)**  | 120 V / 125 A  |

Opravili smo meritve transformatorja v prostem teku in pri obremenitvi z ohmskim bremenom pri približno polovici nazivne moči. Merilni rezultati so v spodnji tabeli.

|             | $U_1\ /\ \text{V}$ | $I_1\ /\ \text{A}$ | $P_1\ /\ \text{W}$ | $U_2\ /\ \text{V}$ | $I_2\ /\ \text{A}$ |
| ----------- | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| Prosti tek  | 240                | 1,71               | 105                | 122,8              | 0                  |
| Obremenitev | 240                | 32,9               | 7871               | 121,5              | 63,3               |

Kolikšne so izgube tega transformatorja pri obremenitvi z nazivno močjo?

## Rešitev
### 1. Izgube v železu (merjene pri prostem teku)
$
P_{\text{Fe}} = 105\ \text{W}
$

### 2. Izgube v bakru pri meritvi (pri $I_{2} = 63.3\ \text{A}$)
Skupne izgube pri obremenitvi:
$
P_{\text{izg,mer}} = P_{1,\text{obrem}} - P_{2,\text{obrem}} = 7871 - (121.5 \cdot 63.3) =  180\ \text{W}
$
Torej:
$
P_{\text{Cu,mer}} = P_{\text{izg,mer}} - P_{\text{Fe}} = 180 - 105 = 75\ \text{W}
$

### 3. Korekcija na nazivni tok ($I_{2n} = 125\ \text{A}$)
Ker veljajo **izgube v bakru $\propto I^2$**, lahko skaliramo:
$
P_{\text{Cu,n}} = P_{\text{Cu,mer}} \cdot \left( \frac{125}{63.3} \right)^2 = 75 \cdot \left( \frac{125}{63.3} \right)$
$
P_{\text{Cu,n}} \approx 75 \cdot 3.902 \approx 292.7\ \text{W}
$

### 4. Skupne izgube pri nazivni obremenitvi:
$
P_{\text{izg,n}} = P_{\text{Fe}} + P_{\text{Cu,n}} = 105 + 292.7 = 397.7\ \text{W}
$

</div></div>


# Naloga 6
Trifazni asinhrosnki motor s kratkostično kletko in podano napisno tablico ima možnost prevezave statorkih navitji za dve različni hitrosti vrtenja:

| Type    | T90 S4/2 IM B3 | 3 - MOTOR        |
| ------- | -------------- | ---------------- |
| Ser. No | G 763304       |                  |
|         | 1.0/1.25kW     | 1390/2900 min^-1 |
|         | 400V           | 50Hz             |
|         | 2.5/3.6A       |                  |
| cos(φ)  | 0.82/0.81      |                  |
| Ins. CL | F              | IP 54            |

S pomočjo Pronyjeve zavore bi radi izmerilill obremilno karakteristiko pri obeh crtilnih hitrostih. Na razpolago imamo tehtnico, ki lahko meri samo do $1kg$.

## a) 
Koliko najmanj mora biti dolga ročica Pronyjeve zavore?
Upoštevamo:
- maksimalna merljiva sila tehtnice: $F_{max} = 1\,\text{kg} \cdot 9.81\,\frac{\text{m}}{\text{s}^2} = 9.81\,\text{N}$
- želimo izmeriti nazivni navor pri **nižji hitrosti** ($n = 1390\,\text{min}^{-1}$, $P = 1.0\,\text{kW}$)

### 1. Izračun maksimalnega navora
$$
M = \frac{P \cdot 60}{2\pi n} = \frac{1000 \cdot 60}{2\pi \cdot 1390} \approx 6.88\,\text{Nm}
$$

### 2. Dolžina ročice
$$
r = \frac{M}{F_{max}} = \frac{6.88}{9.81} \approx 0.702\,\text{m}
$$

## b)
Pri kateri nazivni hitrosti je izkoristek večji?

Izračun izkoristka za vsako delovno točko:
### 1. Nižja hitrost ($P = 1.0\,\text{kW}$, $I = 2.5\,\text{A}$, $\cos\varphi = 0.82$)
$$
\eta_1 = \frac{1000}{\sqrt{3} \cdot 400 \cdot 2.5 \cdot 0.82} \approx \frac{1000}{1419.3} \approx 0.704
$$

### 2. Višja hitrost ($P = 1.25\,\text{kW}$, $I = 3.6\,\text{A}$, $\cos\varphi = 0.81$)
$$
\eta_2 = \frac{1250}{\sqrt{3} \cdot 400 \cdot 3.6 \cdot 0.81} \approx \frac{1250}{2011.5} \approx 0.621
$$
Pri nižji nazivni hitrosti vrtenja ima stroj višji izkoristek.