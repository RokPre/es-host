---
{"dg-publish":true,"permalink":"/izpit-2024-06-28/","tags":["unfinished"]}
---

![Izpit 2024.06.28.1.webp](/img/user/Attachments/izpiti/Izpit%202024.06.28.1.webp)
# Naloga 1

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/izpit-1/#naloga-1" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 1
Transformatorja s podatki 10/0.4 kV, $f = 50\ \mathrm{Hz}$, vezave Yz5,   $S_{n1} = 350\ \mathrm{kVA}$, $u_{k1} = 4\ \%$,  $S_{n2} = 500\ \mathrm{kVA}$, $u_{k2} = 6\ \%$ obratujeta paralelno na nazivnem omrežju. Določite maksimalno skupno moč bremena, tako da se pri trajnem obratovanju noben izmed transformatorjev ne segreje preko dopustne temperature.  

## Rešitev
Skupna moč se izrazi kot:
$
S_b = b_1 \cdot S_{n1} + b_2 \cdot S_{n2}
$
Razmerje med relativnima obremenitvama transformatorjev je:
$
\frac{b_1}{b_2} = \frac{u_{k2}}{u_{k1}} = \frac{6\%}{4\%} = \frac{3}{2}
$
### S1 je S1n
Če je $S_{1} = S_{n}$ potem je $b_{1} = 1$. V tem primeru je $b_{2} = \frac{2}{3}$.

### S2 je S2n
Če je $S_{2} = S_{2,n}$ potem je $b_{2} = 1$. V tem primeru je $b_{1} = \frac{3}{2}$. To bi pomenilo, da je $S_{1}>S_{1, n}$, kar bi pomenilo preobremenitev.

$
S_{b} = S_{1,n} +\frac{2}{3}S_{2,n} = 350000VA + \frac{2}{3}500000VA = 683333AV 
$

</div></div>

# Naloga 2
[[Izpit_2024.02.12#Naloga 2\|Izpit_2024.02.12#Naloga 2]]

Sinhrosnki turbogenerator $S_{n} = 10MVA$, $U_{2n} = 3000V$, $50Hz$, $\cos(\varphi_{2,n}) = 0.7$, $X_{sr} = 2$, $I_{1,n} = 100A$ obratuje na togem nazivnem omrežju. Vzbujanje in dotok pare na turbino sta naravnan tako, da je generator obremenjen z nazivnim tokom pri $\cos(\varphi_{2} ) = 1$. Izračunajte moč, ki jo generator daje v omrežje, kolesni kot in vzbujalni tok (obvezen kazalčni diagram).

## Rešitev

### 2. Električna moč v omrežje

$P_{el} = S_{n}\cdot \cos(\varphi_{2}') = 10MW$
### 3. Kolesni kot $\delta$
$$
\tan\delta = \frac{I_2 \cdot X_s \cdot \cos\varphi}{U_2 + I_2 \cdot X_s \cdot \sin\varphi}
= \frac{1 \cdot 2 \cdot 1}{1 + 0} = 2
$$

$$
\delta = \arctan(2) = 63.4^{\circ}
$$
### 4. Vzbujalni tok
Izračun inducirane napetosti $E_0$ za obe stanji:
#### Novo stanje ($\cos\varphi = 1$):
$$
E_0' = \sqrt{(U_2)^2 + (I_2 \cdot X_s)^2} = \sqrt{1^2 + (1 \cdot 2)^2} = 2.2
$$

#### Nazivno stanje ($\cos\varphi = 0{.}7$):

$$
E_0 = \sqrt{(U_2 + I_2 \cdot X_s \cdot \sin\varphi)^2 + (I_2 \cdot X_s \cdot \cos\varphi)^2}
$$

$$
= \sqrt{(1 + 1 \cdot 2 \cdot 0.714)^2 + (1 \cdot 2 \cdot 0.7)^2} = 2.802\ldots 
$$

$$
\frac{I_v'}{I_{v,n}} = \frac{E_0'}{E_0} = \frac{2.2}{2.8} = 0.79
\quad \Rightarrow \quad I_v' = 0.79 \cdot 100 = \boxed{79\ \mathrm{A}}
$$
# Naloga 3

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/izpit-1/#naloga-3" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 3
Trifazni asinhronski motor z drsnimi obroči $P_n = 55\ \mathrm{kW}$, $U_1 = 380\ \mathrm{V}$, $f_1 = 50\ \mathrm{Hz}$, $I_n = 110\ \mathrm{A}$, $n_n = 731\ \mathrm{min}^{-1}$, $\cos\varphi_n = 0{.}85$, $\frac{M_{om}}{M_n} = 3$, $E_{20} = 280\ \mathrm{V}$, $I_{2n} = 120\ \mathrm{A}$, obratuje na nazivnem omrežju in se vrti z $n_B = 740\ \mathrm{min}^{-1}$.

## a) Določite bremenski navor $M_B$ in rotorski tok $I_{2B}$ v tem obratovalnem stanju.
$
M_{b} = \frac{P \cdot 60}{2 \pi n_{b}} = \frac{55000 \cdot 60}{2\pi \cdot 740} = 709.7Nm
$
$
M_{n} = \frac{P \cdot 60}{2 \pi n_{n}} = \frac{55000 \cdot 60}{2\pi \cdot 731} = 718.4Nm 
$
$
\frac{M_{b}}{M_{n}} = \frac{I_{2,b}}{I_{2,n}} \Rightarrow I_{2,b} = I_{2,n} \frac{M_{b}}{M_{n}} = 120A \frac{709.7}{718.4} = 118.5 A 
$


## b) Izračunajte dodatno upornost v rotorskem tokokrogu $R_{\text{dod}}$, tako da se bo motor vrtel z $n' = 500\ \mathrm{min}^{-1}$ pri obremenitvi z $M' = 1{.}5 \cdot M_n$.

### 1. Izračun nazivnega in novega slip-a

$
s_n = \frac{750 - 731}{750} = 0{.}0253
\qquad
s' = \frac{750 - 500}{750} = 0{.}3333
$

### 2. Rotorska upornost v prvem stanju

$
R_2 = \frac{s_n \cdot E_{20}}{\sqrt{3} \cdot I_2} = 
\frac{0{.}0253 \cdot 280}{\sqrt{3} \cdot 120} \approx 0{.}0341\ \Omega
$

### 3. Uporaba razmerja navorov

Pri enakem toku ($I_2' = I_2$), velja:

$
\frac{R_2'}{R_2} = \frac{s'}{s_{n}} \Rightarrow R_{2}' = 0.0341 \frac{0.3333}{0.0253} = 0.449 \Omega$
$
R_{dod} = R_{2}' - R_{2} =  0.449\Omega-0.0341\Omega = 0.414\Omega 
$

</div></div>


# Naloga 4
Enosmerni generator z paralelnim vzbujanjem ima karakteristiko prostega teka izmerjeno pri $n_{s} = 1200\text{min}^{-1}$. Določite dodatno uporanost $R_{dod}$, ki jo moramo vklučiti v vzbujalno tokokrog, da se pri vrtilni hitrosti $n_{s} = 1500\text{min}^{-1}$ na sponkah generatorja inducirana napetost $140V$. Upornost vzbujalnega navitja je $R_{V} = 18\Omega$.

| I_v[A] | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   |
| ------ | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| E[V]   | 20  | 45  | 72  | 99  | 119 | 133 | 144 | 152 | 158 | 
## Rešitev
Ker se zviša hitrost, bo pri istem vzbujalnem toku višja inducirana napetost:

| I_v[A] | 0   | 1     | 2   | 3      | 4      | 5      | 6   | 7   | 8     |
| ------ | --- | ----- | --- | ------ | ------ | ------ | --- | --- | ----- |
| E[V]'  | 25  | 56.25 | 90  | 123.75 | 148.75 | 166.25 | 180 | 190 | 192.5 | 

$$
E' = 140 \Rightarrow I_{v} = 3.65A
$$
$$
R_{skupna} = R_{v} + R_{dod} = \frac{E'}{I_{v}} = \frac{140}{3.65} = 38.3\Omega
$$
$$
R_{dod} = 38.3-18 = 20.3\Omega 
$$

![Izpit 2024.06.28.2.webp](/img/user/Attachments/izpiti/Izpit%202024.06.28.2.webp)
# Naloga 5
Trifazni sinhronski generator s clindričnim rotorjem ima podano napisno tablico:

| A.C. Generator |               |         |       |        |     |
| -------------- | ------------- | ------- | ----- | ------ | --- |
| type           | ES24-K1       | Output  | 40kVA |        |     |
| Volts          | 400V          | Amps    | 58A   | Phase  | 3   |
| Freq           | 50Hz          | RPM     | 1500  | cos(φ) | 0.8 |
| Conn           | star          | Ins. Cl | H     | IP     | 00  |
| S.N.           | ZGD300075-190 |         |       |        |     |

Pogonski stroj zagotavlja nazivno hitrost vrjtenja, generator pa z nazivno napetostjo in nazivnim toko napaja tri v zvzevdo vezana grela. Breme in vzbujalni tok nato spremenimo tako, da se pri isti napetosti oddana moč zmanjša na polvico prejšnje. Na kolikšen delž začetne vrednosti smo zmanjšali vzbujalni tok po spremembni bremna, če je relativna sinhrosnka reaktanca generatorja $X_{s} = 1.5$?

## Rešitev

### 1. Delovna moč (pred spremembo)

$$
P = U \cdot I = 400\ \mathrm{V} \cdot 58\ \mathrm{A} = 23200\ \mathrm{W}
$$

Po spremembi velja:

$$
P' = \frac{P}{2} = 11600\ \mathrm{W}
\quad \Rightarrow \quad I' = \frac{P'}{U} = \frac{11600}{400} = 29\ \mathrm{A}
$$

---

### 2. Uporabimo enačbo za EMN

Ker gre za grelno breme, kjer velja $\cos(\varphi) = 1$, in ker ostaja napetost nespremenjena ($U = 400\ \mathrm{V}$), izračunamo notranno EMN pred in po spremembi.

#### Pred spremembo:

$$
E_0 = \sqrt{ (U + I \cdot X_s \cdot \sin\varphi)^2 + (I \cdot X_s \cdot \cos\varphi)^2 }
$$

Ker $\varphi = 0 \Rightarrow \sin\varphi = 0,\ \cos\varphi = 1$, sledi:

$$
E_0 = \sqrt{ 400^2 + (58 \cdot 1.5)^2 } = \sqrt{160000 + 7569} = \boxed{409.35\ \mathrm{V}}
$$

#### Po spremembi:

$$
E_0' = \sqrt{ 400^2 + (29 \cdot 1.5)^2 } = \sqrt{160000 + 1892.25} = \boxed{402.36\ \mathrm{V}}
$$

---

### 3. Razmerje vzbujalnih tokov

Ker velja $\frac{I_v'}{I_v} = \frac{E_0'}{E_0}$ (v območju linearnosti), imamo:

$$
\frac{I_v'}{I_v} = \frac{402.36}{409.35} \approx \boxed{0.982}
$$
# Naloga 6
Statorska navitja trifaznega asinhronskega motorja s podano napisno tablico smo zvezali v trikot.  Ko je bil motor nazivno napajan in obremenjen z nazivno močjo, smo izmerili izkoristek 75 %.

|     |              |
| --- | ------------ |
| Moč | 0.27kW/0.5Hp |
| Rpm | 2730         |
| vez | Δ/Y          | 
| Nap | 230/400V     |
| Tok | 1.67/0.97A   |
## a) Kolikšen je faktor moči delovnosti motorja v nazibnem obratovalnrm dzsnju?
Skupna dovedena električna moč:
$$
P_{\text{el}} = \frac{P}{\eta} = \frac{270}{0{.}75} = 360\ \mathrm{W}
$$
Navidezna moč:
$$
S = \sqrt{3} \cdot U \cdot I = \sqrt{3} \cdot 230\ \mathrm{V} \cdot 1{.}67\ \mathrm{A} \approx 665\ \mathrm{VA}
$$

Faktor moči:

$$
\cos\varphi = \frac{P_{\text{el}}}{S} = \frac{360}{665} \approx \boxed{0{.}541}
$$
## b) Kolikšne so pri omenjenem obratovnaju izgube v statorskih navitjuh, če je upornost posameznega statorsgea faznega navitja $15 \Omega$?
Pri vezavi v trikot, velja:

- fazna napetost: $U_f = 230\ \mathrm{V}$
- fazni tok: $I_f = \frac{I_L}{\sqrt{3}} = \frac{1{.}67}{\sqrt{3}} \approx 0{.}964\ \mathrm{A}$


Izgube v statorju (skupno za 3 faze):

$$
P_{\text{Cu}} = 3 \cdot I_f^2 \cdot R = 3 \cdot (0{.}964)^2 \cdot 15 \approx \boxed{41{.}7\ \mathrm{W}}
$$