---
{"dg-publish":true,"permalink":"/izpit-2024-09-03/","tags":["unfinished"]}
---


![Izpit 2024.09.03.1.webp](/img/user/Attachments/izpiti/Izpit%202024.09.03.1.webp)
# Naloga 1
Transformator naziv­ne moči $S_n = 200\ \mathrm{MVA}$ z nazivnim izkoristkom $\eta_n = 0{.}98$, razmerjem izgub na nazivnem omrežju $\xi_n = 3$,  se med trajnim obratovanjem segreje do nadtemperature $\Theta_{\text{max}} = 100\ \mathrm{K}$. Transformator uporabimo na omrežju z: $U = 0{.}8 \cdot U_n$, $f = 1{.}2 \cdot f_n$. Do katere nadtemperature se bo transformator segrel pri trajnem obratovanju na novem omrežju, če je obremenjen s tokom $I' = I_n$?

## Rešitev
[[Izpit_2024.06.17#Rešitev\|Izpit_2024.06.17#Rešitev]]
### 1. Skupne izgube pri nazivnem obratovanju
$$
P_{\text{izg,n}} = (1 - \eta_n) \cdot S_n = 0{.}02 \cdot 200\,000\,000 = 4\,000\,000\ \mathrm{W}
$$
Delitev na železne in bakrene izgube:
$$
P_{Cu,n} = 3 \cdot P_{Fe,n} \Rightarrow P_{\text{izg,n}} = 4 \cdot P_{Fe,n}
\Rightarrow P_{Fe,n} = \frac{4\,000\,000}{4} = 1\,000\,000\ \mathrm{W}
$$

### 2. Prilagoditev izgub v železu
$$
P_{Fe}' = P_{Fe,n} \cdot \left( \frac{U'}{U_n} \right)^2 \cdot \left( \frac{f'}{f_n} \right)
= 1\,000\,000 \cdot (0{.}8)^2 \cdot 1{.}2 = 768\,000\ \mathrm{W}
$$
### 3. Bakrene izgube
Ker $I' = I_n$, velja:
$$
P_{Cu}' = P_{Cu,n} = 3 \cdot P_{Fe,n} = 3 \cdot 1\,000\,000 = 3\,000\,000\ \mathrm{W}
$$

### 4. Skupne izgube in razmerje temperatur
$$
P_{\text{izg}}' = P_{Cu}' + P_{Fe}' = 3\,000\,000 + 768\,000 = 3\,768\,000\ \mathrm{W}
$$
Razmerje:
$$
\frac{\Theta'_{\text{max}}}{\Theta_{\text{max,n}}} = \frac{P_{\text{izg}}'}{P_{\text{izg,n}}}
= \frac{3\,768\,000}{4\,000\,000} = 0{.}942
$$

### 5. Nova nadtemperatura
$$
\Theta_{\text{max}}' = 0{.}942 \cdot 100\ \mathrm{K} = \boxed{94{.}2\ \mathrm{K}}
$$
# Naloga 2

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/kolokvij-2/#naloga-4" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 4
Sinhronski turbogenerator $S_n = 25 \mathrm{MVA}$, $U_{zn} = 6.3\ \mathrm{kV}$, $f_n = 50\ \mathrm{Hz}$, $\cos\varphi_{2n} = 0.6$, $X_{sr} = 1.8$ je obremenjen s polovičnim nazivnim tokom pri $\cos\varphi_2 = 0.8$ na togem omrežju, nazivne napetosti in frekvence. Pri nespremenjenem vzbujanju nato počasi povečujemo dovod pare na turbino. Določite navidezno $S_{om}$ in delovno $P_{om}$ moč ter $\cos\varphi_2$ tik preden generator pade iz sinhronizma(obvezna skica obeh obratovalnih stanj).
## 1) Izračun nazivnega toka
$
I_n = \frac{S_n}{\sqrt{3} \cdot U_n} = \frac{25 \cdot 10^6}{\sqrt{3} \cdot 6300} \approx 2291\ \mathrm{A}
$
## 2) Začetno stanje
Obremenitev z:
- $I' = 0{.}5 \cdot I_n = 1145{.}5\ \mathrm{A}$
- $\cos\varphi' = 0{.}8$

To stanje je **referenčno** – tu si izračunamo inducirano EMN $E_0$, ki je **nato nespremenjena**.
## 3) Izračun inducirane napetosti $E_0$
Za tok $I'$ in $\cos\varphi = 0.8 \Rightarrow \sin\varphi = 0.6$:
$
E_0 = \sqrt{(U + I' X_s \cdot \sin\varphi)^2 + (I' X_s \cdot \cos\varphi)^2}
$
Vstavimo podatke:
- $U = 6300\ \mathrm{V}$
- $X_s = 1{.}8\ \Omega$
$
E_0 = \sqrt{(6300 + 1145{.}5 \cdot 1{.}8 \cdot 0{.}6)^2 + (1145{.}5 \cdot 1{.}8 \cdot 0{.}8)^2}
$
$
E_0 = \sqrt{(6300 + 1236{.}3)^2 + (1649{.}5)^2} \approx 7722\ \mathrm{V}
$

## 4) Kritično (mejno) stanje: $\delta = 90^\circ$

Takrat je:

$
E_0 = I_{om} \cdot X_s \Rightarrow I_{om} = \frac{E_0}{X_s} = \frac{7722}{1{.}8} \approx 4290\ \mathrm{A}
$


## 5) Izračun navidezne in delovne moči

$
S_{om} = \sqrt{3} \cdot U \cdot I_{om} = \sqrt{3} \cdot 6300 \cdot 4290 \approx 46{.}8\ \mathrm{MVA}
$

$
\cos\varphi_{om} = \frac{U}{E_0} = \frac{6300}{7722} \approx 0{.}816
$

$
P_{om} = S_{om} \cdot \cos\varphi_{om} \approx 46{.}8 \cdot 0{.}816 \approx 38{.}2\ \mathrm{MW}
$

</div></div>


# Naloga 3
Osem polni trifazni asinhronski motor z drsnimi obroči ima podatke:
$P_n = 30\ \mathrm{kW}$, $U_{1n} = 380\ \mathrm{V}$, $f_1 = 50\ \mathrm{Hz}$, $I_{1n} = 63\ \mathrm{A}$, $\cos\varphi_n = 0.8$, $E_{20} = 151\ \mathrm{V}$, $I_{2n} = 120\ \mathrm{A}$, $\frac{M_{om}}{M_n} = 2.5$, frekvenca rotorsko inducirane napetosti pri nazivni obremenitvi $f_2 = 1.33\ \mathrm{Hz}$. Določite: nazivni izkoristek motorja $\eta_n$, nazivno vrtilno hitrost $n_n$, omahni navor $M_{om}$, omahni slip $s_{om}$ omahno vrtilno hitrost $n_{om}$ rotorsko fazno upornost $R_2$.
## Rešitev
## 1. Nazivni izkoristek $\eta_n$
$$
P_{\text{el}} = \sqrt{3} \cdot U_1 \cdot I_1 \cdot \cos\varphi = \sqrt{3} \cdot 380 \cdot 63 \cdot 0.8 \approx 33\,193\ \mathrm{W}
$$
$$
\eta_n = \frac{P_n}{P_{\text{el}}} = \frac{30\,000}{33\,193} \approx \boxed{0.904\ (\text{ali } 90.4\%)}
$$

## 2. Nazivna vrtilna hitrost $n_n$
Za 8 polov:
$$
p = 8 \Rightarrow n_s = \frac{60 \cdot f_1}{p} = \frac{60 \cdot 50}{8} = 375\ \mathrm{min}^{-1}
$$
Slip iz $f_2$:
$$
s_n = \frac{f_2}{f_1} = \frac{1.33}{50} = 0.0266
$$
$$
n_n = n_s \cdot (1 - s_n) = 375 \cdot (1 - 0.0266) \approx \boxed{365\ \mathrm{min}^{-1}}
$$

## 3. Omahni navor $M_{om}$
$$
M_n = \frac{P_n \cdot 60}{2\pi \cdot n_n} = \frac{30\,000 \cdot 60}{2\pi \cdot 365} \approx 786.8\ \mathrm{Nm}
$$
$$
M_{om} = 2.5 \cdot M_n = 2.5 \cdot 786.8 = \boxed{1\,967\ \mathrm{Nm}}
$$
## 4. Omahni slip $s_{om}$
Omahni slip izračunamo z Klossovo enačbo:
$$
\frac{M_n}{M_{om}} = \frac{2}{\frac{s_n}{s_{om}} + \frac{s_{om}}{s_n}}
$$
Vstavimo:
$$
\frac{786.8}{1967} = \frac{2}{\frac{0.0266}{s_{om}} + \frac{s_{om}}{0.0266}} \Rightarrow s_{om}^2 - 0.133 s_{om} + 0.000707 = 0
$$
Rešitvi:
- $s_{om,1} = 0.0055$ ❌ (nefizična – manjša od $s_n$)
- $s_{om,2} = \boxed{0.1274}$ ✅ (pravilna – večja od $s_n$)

## 5. Omahna vrtilna hitrost $n_{om}$
$$
n_{om} = n_s \cdot (1 - s_{om}) = 375 \cdot (1 - 0.1274) = 327.225
$$

## 6. Rotorska fazna upornost $R_2$
Pri nazivni obremenitvi velja:
$$
R_2 = \frac{s_n \cdot E_{20}}{\sqrt{3} \cdot I_{2n}} = \frac{0.0266 \cdot 151}{\sqrt{3} \cdot 120} \approx \boxed{0.193\ \Omega}
$$
# Naloga 4
Enosmerni motor s tujim vzbujanjem ima nazivne podatke:  
$P_n = 40\ \text{kW}$, $U_n = 440\ \text{V}$, $\eta_n = 0{,}88$, $n_n = 1200\ \text{min}^{-1}$, $R_i = 0{,}11\ \Omega$, $\Delta U_{\text{šč}} = 2\ \text{V}$. Stroj uporabimo kot generator, ki obratuje na nazivnem omrežju in oddaja v omrežje tok: $I_1 = 0{,}9 \cdot I_n$. Določite vrtilno hitrost, s katero moramo za to obratovalno stanje poganjati stroj (vzbujevanje ostane nespremenjeno).

## Rešitev
### 1. Izračun nazivnega toka (motorni režim)
Pri motorju velja:
$$
\eta_n = \frac{P_{\text{meh}}}{P_{\text{el}}} \quad \Rightarrow \quad P_{\text{el}} = \frac{P_n}{\eta_n}
$$
$$
P_{\text{el}} = \frac{40\,000}{0{.}88} = 45\,454{.}55\ \text{W}
$$
$$
I_n = \frac{P_{\text{el}}}{U_n} = \frac{45\,454{.}55}{440} \approx 103{.}3\ \text{A}
$$

### 2. Tok v generatorskem režimu
$$
I' = 0{.}9 \cdot I_n = 0{.}9 \cdot 103{.}3 = 92{.}97\ \text{A}
$$

### 3. Napetostna konstanta EMN
#### a) Motorni režim (nazivna hitrost)
$$
E_n = U - I_n \cdot R_i - \Delta U_{\text{šč}} = 440 - 103{.}3 \cdot 0{.}11 - 2  = 426{.}64\ \text{V}
$$

#### b) Generatorski režim
$$
E' = U + I' \cdot R_i + \Delta U_{\text{šč}} = 440 + 92{.}97 \cdot 0{.}11 + 2 = 452{.}23\ \text{V}
$$

### 4. Razmerje hitrosti
Ker vzbujevanje ostane nespremenjeno, velja:
$$
\frac{E'}{E_n} = \frac{n'}{n_n}
$$
$$
n' = n_n \cdot \frac{E'}{E_n} = 1200 \cdot \frac{452{.}23}{426{.}64} \approx 1200 \cdot 1{.}0599 = 1271{.}9\ \text{min}^{-1}
$$

![Izpit 2024.09.03.2.webp](/img/user/Attachments/izpiti/Izpit%202024.09.03.2.webp)
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
$$
P_{\text{Fe}} = 105\ \text{W}
$$

### 2. Izgube v bakru pri meritvi (pri $I_{2} = 63.3\ \text{A}$)
Skupne izgube pri obremenitvi:
$$
P_{\text{izg,mer}} = P_{1,\text{obrem}} - P_{2,\text{obrem}} = 7871 - (121.5 \cdot 63.3) =  180\ \text{W}
$$
Torej:
$$
P_{\text{Cu,mer}} = P_{\text{izg,mer}} - P_{\text{Fe}} = 180 - 105 = 75\ \text{W}
$$

### 3. Korekcija na nazivni tok ($I_{2n} = 125\ \text{A}$)
Ker veljajo **izgube v bakru $\propto I^2$**, lahko skaliramo:
$$
P_{\text{Cu,n}} = P_{\text{Cu,mer}} \cdot \left( \frac{125}{63.3} \right)^2 = 75 \cdot \left( \frac{125}{63.3} \right)^2
$$
$$
P_{\text{Cu,n}} \approx 75 \cdot 3.902 \approx 292.7\ \text{W}
$$

### 4. Skupne izgube pri nazivni obremenitvi:
$$
P_{\text{izg,n}} = P_{\text{Fe}} + P_{\text{Cu,n}} = 105 + 292.7 = 397.7\ \text{W}
$$
# Naloga 6

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/izpit-2024-02-12/#naloga-6" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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
$
M = \frac{P \cdot 60}{2\pi n} = \frac{1000 \cdot 60}{2\pi \cdot 1390} \approx 6.88\,\text{Nm}
$

### 2. Dolžina ročice
$
r = \frac{M}{F_{max}} = \frac{6.88}{9.81} \approx 0.702\,\text{m}
$

## b)
Pri kateri nazivni hitrosti je izkoristek večji?

Izračun izkoristka za vsako delovno točko:
### 1. Nižja hitrost ($P = 1.0\,\text{kW}$, $I = 2.5\,\text{A}$, $\cos\varphi = 0.82$)
$
\eta_1 = \frac{1000}{\sqrt{3} \cdot 400 \cdot 2.5 \cdot 0.82} \approx \frac{1000}{1419.3} \approx 0.704
$

### 2. Višja hitrost ($P = 1.25\,\text{kW}$, $I = 3.6\,\text{A}$, $\cos\varphi = 0.81$)
$
\eta_2 = \frac{1250}{\sqrt{3} \cdot 400 \cdot 3.6 \cdot 0.81} \approx \frac{1250}{2011.5} \approx 0.621
$
Pri nižji nazivni hitrosti vrtenja ima stroj višji izkoristek.

</div></div>
