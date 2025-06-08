---
{"dg-publish":true,"permalink":"/izpit-1/","tags":["unfinished"]}
---

# Naloga 1
Transformatorja s podatki 10/0.4 kV, $f = 50\ \mathrm{Hz}$, vezave Yz5,   $S_{n1} = 350\ \mathrm{kVA}$, $u_{k1} = 4\ \%$,  $S_{n2} = 500\ \mathrm{kVA}$, $u_{k2} = 6\ \%$ obratujeta paralelno na nazivnem omrežju. Določite maksimalno skupno moč bremena, tako da se pri trajnem obratovanju noben izmed transformatorjev ne segreje preko dopustne temperature.  

## Rešitev
Skupna moč se izrazi kot:
$$
S_b = b_1 \cdot S_{n1} + b_2 \cdot S_{n2}
$$
Razmerje med relativnima obremenitvama transformatorjev je:
$$
\frac{b_1}{b_2} = \frac{u_{k2}}{u_{k1}} = \frac{6\%}{4\%} = \frac{3}{2}
$$
### S1 je S1n
Če je $S_{1} = S_{n}$ potem je $b_{1} = 1$. V tem primeru je $b_{2} = \frac{2}{3}$.

### S2 je S2n
Če je $S_{2} = S_{2,n}$ potem je $b_{2} = 1$. V tem primeru je $b_{1} = \frac{3}{2}$. To bi pomenilo, da je $S_{1}>S_{1, n}$, kar bi pomenilo preobremenitev.

$$
S_{b} = S_{1,n} +\frac{2}{3}S_{2,n} = 350000VA + \frac{2}{3}500000VA = 683333AV 
$$
# Naloga 2

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/kolokvij-2/#naloga-4" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 4
Sinhronski turbogenerator $S_n = 25\ \mathrm{MVA}$, $U_n = 6{.}3\ \mathrm{kV}$, $50\ \mathrm{Hz}$, $\cos\varphi_n = 0{.}6$, $X_{sr} = 1{.}8$ je obremenjen s polovico nazivnega toka pri $\cos\varphi = 0{.}8$ na togem omrežju nazivne napetosti in frekvence. Pri nespremenjenem vzbujanju počasi povečujemo dovod pare na turbino. Določite navidezno moč $S_{om}$ in delovno moč $P_{om}$ ter $\cos\varphi$ tik preden generator pade iz sinhronizma (obvezna skica obeh obratovalnih stanj).
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
Trifazni asinhronski motor z drsnimi obroči $P_n = 55\ \mathrm{kW}$, $U_1 = 380\ \mathrm{V}$, $f_1 = 50\ \mathrm{Hz}$, $I_n = 110\ \mathrm{A}$, $n_n = 731\ \mathrm{min}^{-1}$, $\cos\varphi_n = 0{.}85$, $\frac{M_{om}}{M_n} = 3$, $E_{20} = 280\ \mathrm{V}$, $I_{2n} = 120\ \mathrm{A}$, obratuje na nazivnem omrežju in se vrti z $n_B = 740\ \mathrm{min}^{-1}$.

## a) Določite bremenski navor $M_B$ in rotorski tok $I_{2B}$ v tem obratovalnem stanju.
$$
M_{b} = \frac{P \cdot 60}{2 \pi n_{b}} = \frac{55000 \cdot 60}{2\pi \cdot 740} = 709.7Nm
$$
$$
M_{n} = \frac{P \cdot 60}{2 \pi n_{n}} = \frac{55000 \cdot 60}{2\pi \cdot 731} = 718.4Nm 
$$
$$
\frac{M_{b}}{M_{n}} = \frac{I_{2,b}}{I_{2,n}} \Rightarrow I_{2,b} = I_{2,n} \frac{M_{b}}{M_{n}} = 120A \frac{709.7}{718.4} = 118.5 A 
$$


## b) Izračunajte dodatno upornost v rotorskem tokokrogu $R_{\text{dod}}$, tako da se bo motor vrtel z $n' = 500\ \mathrm{min}^{-1}$ pri obremenitvi z $M' = 1{.}5 \cdot M_n$.

### 1. Izračun nazivnega in novega slip-a

$$
s_n = \frac{750 - 731}{750} = 0{.}0253
\qquad
s' = \frac{750 - 500}{750} = 0{.}3333
$$

### 2. Rotorska upornost v prvem stanju

$$
R_2 = \frac{s_n \cdot E_{20}}{\sqrt{3} \cdot I_2} = 
\frac{0{.}0253 \cdot 280}{\sqrt{3} \cdot 120} \approx 0{.}0341\ \Omega
$$

### 3. Uporaba razmerja navorov

Pri enakem toku ($I_2' = I_2$), velja:

$$
\frac{R_2'}{R_2} = \frac{s'}{s_{n}} \Rightarrow R_{2}' = 0.0341 \frac{0.3333}{0.0253} = 0.449 \Omega$$
$$
R_{dod} = R_{2}' - R_{2} =  0.449\Omega-0.0341\Omega = 0.414\Omega 
$$
# Naloga 4
Enosmerni serijski motor z nazivnimi podatki: **600 V**, **187 A**, **100 kW**, **1410 min⁻¹**, $R_i = 0{.}1\ \Omega$ , $R_v = 0{.}043\ \Omega$, $\Delta U_{\text{šč}} = 2{.}3\ \mathrm{V}$ obratuje v linearnem (nezasičenem) delu magnetilne karakteristike (nezasičeno področje). Izračunajte vrtilno hitrost motorja, če je pri napajanju z $U'= 550V$ obremenjen z $M_{B} = 500Nm$.
## Rešitev

### 1. Napetostna enačba

$$
U = E + I \cdot (R_i + R_v) + \Delta U_{\text{šč}}
$$

### 2. EMN v nazivnem stanju

$$
E_n = 600 - 187 \cdot (0{.}1 + 0{.}043) - 2{.}3 = 570{.}959\ \mathrm{V}
$$

### 3. EMN v novem stanju

$$
E' = 550 - 187 \cdot 0{.}143 - 2{.}3 = 520{.}959\ \mathrm{V}
$$

### 4. Sorazmerje hitrosti

Ker velja $E \sim n$ (nezasičeno področje):

$$
n' = n_n \cdot \frac{E'}{E_n} = 1410 \cdot \frac{520{.}959}{570{.}959} \approx 1285\ \mathrm{min}^{-1}
$$


# Naloga 5

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/kolokvij-1/#naloga-5" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 5
Za trigaztni transformator $S_{n} = 50kVA$, $U_{1n} = 20kV$, $U_{2n} = 0.4kV$, $f_{n} = 50Hz$, imamo na voljo rezultate meritve električnih veličin na primarni strani pri preizkusu prostega teka, preizkusu kratkega stika in obremenilnem preizkusu, vendar ni označeno, kateri rezultati so za posamezno obratovalno stanje:
- Meritev A: $U_{A} = 20.03kV$, $I_{A} = 1.05A$, $\cos(\varphi) = 0.952$
- Meritev B: $U_{B} = 824.3V$, $I_{B} = 1.38A$, $\cos(\varphi) = 0.375$
- Meritev C: $U_{C} = 20.04kV$, $I_{C} = 0.012A$, $\cos(\varphi) = 0.186$

Ugotovite in definirajte kateri merilni rezultati ustrezajo posameznemu preizkusu. Določite tudi, kolikšne so nazivne izgube v železu in v navitju transformatorja.
## Razvrstitev meritev:
- **Meritev C**:  
  Visoka napetost, zelo majhen tok → **prosti tek**
- **Meritev B**:  
  Nizka napetost, sorazmerno velik tok → **kratek stik**
- **Meritev A**:  
  Nazivna napetost, zmeren tok, visok $\cos\varphi$ → **obremenitveni preizkus**
## Izračun izgub
### 1. **Izgube v železu** $P_{Fe}$  
(iz meritve prostega teka = meritev **C**)
$
P_{Fe} = U_C \cdot I_C \cdot \cos\varphi = 20\,040 \cdot 0{.}012 \cdot 0{.}186 \approx \boxed{44{.}7\ \text{W}}
$
### 2. **Izgube v bakru** $P_{Cu}$  
(iz meritve kratkega stika = meritev **B**)
$
P_{Cu} = U_B \cdot I_B \cdot \cos\varphi = 824{.}3 \cdot 1{.}38 \cdot 0{.}375 \approx \boxed{426{.}5\ \text{W}}
$

</div></div>

# Naloga 6
Trifazni asinhronski motor s podano napisno tablico ima statorska navitja vezana v zvezdo.

| Type     | T132SA2IMB3 |             |
| -------- | ----------- | ----------- |
| Ser. No. | G944465     |             |
|          | 5.5kW       | 2900 min^-1 |
| Δ/Y      | 230V/400V   | 50Hz        |
|          | 18.2/10.5A  |             |
| cos(φ)   | 0.88        |             |
| Ins. Cl. | F           | IP 54       |

Na motorju sta bila opravljena:
- preizkus prostega teka: $I_{0} = 2.3A$, $P_{0}= 372W$
- preizkus kratkega stika: $U_{k} = 74.23V$, $P_{k} =530W$

Upornosti izmerjene med posameznimi priključnimi sponkami motorja U, V in W so približno enake in so $R_{UV} =R_{VW} = R_{WU} = 1.35\Omega$.

a) Kolikšno največjo vrednost toka lahko pričakujemo pri neposrednem vklopu motorja na nazivno omrežje?
$$
s = 1
$$
$$
I_{zag} = \frac{ U_{f}}{R} =\frac{400\cdot 2}{1.35\cdot \sqrt{ 3 }} = 342.1 A
$$
b) Kolikšen je izkoristek motorja v nazivnem obratovalnem stanju?
$$
\eta =\frac{P_{n}-(P_{0}+P_{k})}{P_{n}} = \frac{5500 - (372 + 530)}{5500} = 0.836
$$