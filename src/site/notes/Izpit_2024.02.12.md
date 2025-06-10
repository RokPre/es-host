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
Ker je breme priključeno **med eno fazo (b) in ničlo**, teče ves tok $I_b$ skozi ničlovod. Torej:

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
P_{el} = \sqrt{3} \cdot U_2 \cdot I_2 \cdot \cos\varphi = \sqrt{3} \cdot 3000 \cdot 1924{.}5 \cdot 1 \approx 10\,000\,000\ \text{W} = 10\ \text{MW}
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
## 4. Izračun EMN $E_0'$ za $\cos\varphi = 1$

$$
E_0' = \sqrt{(U_2 + I_2 \cdot X_{sr} \cdot \sin\varphi)^2 + (I_2 \cdot X_{sr} \cdot \cos\varphi)^2}
$$

$$
E_0' = \sqrt{(3000)^2 + (1924{.}5 \cdot 1{.}6)^2} = \sqrt{9\,000\,000 + 9\,486\,118{.}4} \approx \sqrt{18\,486\,118{.}4} \approx 4300{.}7\ \text{V}
$$

## 5. Izračun $E_{0n}$ iz referenčnega stanja ($I_{2n}$, $\cos\varphi = 0.8$)

$$
\sin\varphi = \sqrt{1 - 0{.}8^2} = 0{.}6
$$

$$
E_{0n} = \sqrt{(3000 + 1924{.}5 \cdot 1{.}6 \cdot 0{.}6)^2 + (1924{.}5 \cdot 1{.}6 \cdot 0{.}8)^2}
$$

$$
E_{0n} = \sqrt{(3000 + 1847{.}5)^2 + (2463{.}36)^2} = \sqrt{(4847{.}5)^2 + (2463{.}36)^2} \approx 5432\ \text{V}
$$

---

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
vezava: **trikot**.

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
#### 2. Navor pri zaganjanju v **vezavi zvezda**

V zvezdi je fazna napetost:

$$
U_Y = \frac{U_\Delta}{\sqrt{3}} = \frac{400}{\sqrt{3}} \approx 230{.}94\ \text{V}
$$

Ker je navor sorazmeren s kvadratom napetosti:

$$
M_z^Y = M_z^\Delta \cdot \left( \frac{U_Y}{U_\Delta} \right)^2 = 402{.}1 \cdot \left( \frac{230{.}94}{400} \right)^2 \approx 402{.}1 \cdot 0{.}333 \approx \boxed{133{.}9\ \text{Nm}}
$$
#### 3. Zagonski tok v **vezavi zvezda**

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
Enosmerni motor s serijskim vzbujanjem ima nazivne podatke: $U_{n} = 400V$, $P_{n} = 10kW$, $n_{n} = 1200\text{min}^{-1}$. Poganja delovni stroj, katerega bremenski navor je neodvisen od vrtilne hitrosti $M_{b} = konst$. Pri obratovnaju na nazivnem omrežju je motor nazivno obremnenjen in se nahaja še v nenasičenem področju magnetilne krivulje. Kakšna bo vrtilna hitrsot motorja, će se napajalna napetost zniža za $30\%$?
## Rešitev

### 1. Ključne fizikalne povezave

- V serijskem motorju velja: $\Phi \sim I$
- Navor: $M \sim \Phi \cdot I \sim I^2$
- Ker je $M_b = \text{konst.} \Rightarrow I = \text{konst.}$ in tudi $\Phi = \text{konst.}$
- Elektromotorna napetost: $E = k \cdot \Phi \cdot n \Rightarrow n \sim E$
- Ker je $I$ konstanten, je tudi padec napetosti na notranji upornosti ($I R$) in na ščetkah konstanten
### 2. Napetostna enačba
$$
n = \frac{U}{k_{e}k_{\phi}\sqrt{ \frac{M}{k_{m}k_{\phi}} }}
$$
Za serijski motor velja:
$$
U = E + I \cdot R + \Delta U_{\text{šč}}
$$
Ker so $I$, $R$ in $\Delta U_{\text{šč}}$ konstantni, lahko zapišemo razmerje za EMN:
$$
\frac{n'}{n_n} = \frac{E'}{E_n} = \frac{U' - \text{konst.}}{U_n - \text{konst.}}
$$

Če je $\text{konst.}$ majhna v primerjavi z $U$, lahko zapišemo:

$$
\frac{n'}{n_n} \approx \frac{U'}{U_n}
$$
### 3. Izračun

Znižanje napetosti za 30 % pomeni:

$$
U' = 0{.}7 \cdot U_n = 0{.}7 \cdot 400\ \mathrm{V} = 280\ \mathrm{V}
$$

$$
\frac{n'}{n_n} = \frac{280}{400} = 0{.}7 \quad \Rightarrow \quad n' = 0{.}7 \cdot 1200 = \boxed{840\ \mathrm{min}^{-1}}
$$
---
![izpit 2024.02.12.2.webp](/img/user/Attachments/izpiti/izpit%202024.02.12.2.webp)
# Naloga 5