---
{"dg-publish":true,"permalink":"/kolokvij-2/","tags":["unfinished"]}
---

![Kolokvij 2.1.webp](/img/user/Attachments/izpiti/Kolokvij%202.1.webp)
# Naloga 1

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/kolokvij-1/#naloga-1" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 1
Na osnovi podane vezalne sheme doloćite vezno skupino in fazno številko trifaznega transformatorja s podatki $S_{n} = 250kVA$, $U_{1n} = 10kV$, $u_{k} = 4\%$. Ali je vezava pravilna (odgovor obvezno utemeljite)? Določite sekundarno medfazno napetost $U_{2n}$, če se v posamezni sekundarni tuljavici inducira napetost $200V$. K temu transformatorju želimo paralelno priključiti transfomator s podakti $S_{n} = 200kVA$, $10/0.5kV$, $u_{k} = 6\%$, $Dz6$. Ali je takšno pararelno obratovanje dopustno (odgovor obeno utemeljite)?
### 1. Vezna skupina
Iz kazalčnega diagrama in podanih faznih kotov ugotovimo, da gre za:
$
\text{Vezna skupina:} \quad Yz5
$
### 2. Ali je vezava pravilna?
Da, vezava je pravilna. Kazalci faznih napetosti na sekundarni strani tvorijo enakostranični trikotnik z medsebojnimi koti $120^\circ$ in enakimi amplitudami, kar pomeni, da je sistem **simetričen**, zaporedje faz pa **desnosučno**.
### 3. Sekundarna medfazna napetost
Če je napetost posamezne sekundarne tuljavice (fazna napetost pri cikcak vezavi):
$
U_{2f} = 200\ \text{V}
$
potem je medfazna napetost (cikcak):
$
U_{2mf} = \sqrt{3} \cdot U_{2f} = \sqrt{3} \cdot 200\ \text{V} \approx 346{.}4\ \text{V}
$
### 4. Ali je možno paralelno obratovanje?
Vzporedno (paralelno) obratovanje **ni možno**, saj se fazni številki transformatorjev ne ujemata.

Za uspešno paralelno obratovanje mora biti izpolnjen pogoj:
$
(n_1 - n_2)\mod 4 = 0
$
V našem primeru:
$
(6 - 5)\mod 4 = 1 \ne 0
$
Zato med transformatorjema obstaja **fazen zamik**, ki onemogoča delovanje brez krožnih tokov.


</div></div>

# Naloga 2
Transfomator za nativno napeost $U_{1n} = 115V$, $f_{n} = 60 Hz$ ima na nazivniem omrežju v prostem teku $P_{0}=200W$ izgub. Želimo ga predelati ta priklop na omrežje $U_{1}' = 230V$, $f = 50 Hz$. Izračunajte potrebno spremembo števila ovojev primarnega navitja, da bodo na tako spremenjenem morežju izgube v prostem teku znašale $P_{0}' = 240W$. 

## Rešitev
Izgube v železu so sorazmerne z $f \cdot B^2$, gostota $B$ pa:
$$
B \propto \frac{U}{N f}
$$
Torej:
$$
P_0' = P_0 \cdot \frac{f'}{f} \cdot \left( \frac{U'/f'}{U/f} \cdot \frac{N}{N'} \right)^2
$$
Vstavimo podatke:
$$
240 = 200 \cdot \frac{50}{60} \cdot \left( \frac{230 \cdot 60}{115 \cdot 50} \cdot \frac{N}{N'} \right)^2
$$
Po poenostavitvi:
$$
\frac{N}{N'} = 0{.}5 \quad \Rightarrow \quad N' = 2 \cdot N
$$
# Naloga 3

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/kolokvij-1/#naloga-3" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Naloga 3
Sinhronski turbogenerator $S_n = 200\ \mathrm{MVA}$, $U_n = 15\ \mathrm{kV}$, $\cos\varphi_{2n} = 0{.}8$, $X_{sr} = 1{.}4$, $I_n = 300\ \mathrm{A}$ obratuje na togem nazivnem omrežju pri obremenitvi $S' = 100\ \mathrm{MVA}$, $\cos\varphi_{2}' = 0{.}6$. Za to obratovalno stanje določite potreben vzbujalni tok $I_1'$ in oba kolesna kota $\delta_n$ in $\delta'$ (obvezna tudi skica obeh obratovalnih stanj).

## 1. Izračun nazivnega toka $I_{2n}$

$
I_{2n} = \frac{S_n}{\sqrt{3} \cdot U_{2n}} = \frac{200 \cdot 10^6}{\sqrt{3} \cdot 15\,000} \approx 7698\ \text{A}
$
## 2. Kolesni kot $\delta_n$

$\cos\varphi_{2n} = 0.8 \Rightarrow \sin\varphi_{2n} = 0.6$

$
\tan\delta_n = \frac{I_{2n} \cdot X_s \cdot \cos\varphi_{2n}}{U_{2n} + I_{2n} \cdot X_s \cdot \sin\varphi_{2n}}
$

$
\tan\delta_n = \frac{7698 \cdot 1{.}4 \cdot 0{.}8}{15\,000 + 7698 \cdot 1{.}4 \cdot 0{.}6}\approx 0{.}4014
$

$
\delta_n \approx \arctan(0{.}4014) \approx 21{.}9^\circ
$
## 3. Kolesni kot $\delta'$

Za obremenitev $S' = 100\ \text{MVA}$ in $\cos\varphi_2' = 0.6$:

$
I_{2}' = \frac{S'}{\sqrt{3} \cdot U_{2n}} = \frac{100 \cdot 10^6}{\sqrt{3} \cdot 15\,000} \approx 3849\ \text{A}
$

$\sin\varphi_2' = 0.8$

$
\tan\delta' = \frac{3849 \cdot 1{.}4 \cdot 0{.}6}{15\,000 + 3849 \cdot 1{.}4 \cdot 0{.}8} = \frac{3229{.}18}{19\,308{.}48} \approx 0{.}1672
$

$
\delta' \approx \arctan(0{.}1672) \approx 9{.}5^\circ
$


</div></div>

# Naloga 4
Sinhronski turbogenerator $S_n = 25 \mathrm{MVA}$, $U_{zn} = 6.3\ \mathrm{kV}$, $f_n = 50\ \mathrm{Hz}$, $\cos\varphi_{2n} = 0.6$, $X_{sr} = 1.8$ je obremenjen s polovičnim nazivnim tokom pri $\cos\varphi_2 = 0.8$ na togem omrežju, nazivne napetosti in frekvence. Pri nespremenjenem vzbujanju nato počasi povečujemo dovod pare na turbino. Določite navidezno $S_{om}$ in delovno $P_{om}$ moč ter $\cos\varphi_2$ tik preden generator pade iz sinhronizma(obvezna skica obeh obratovalnih stanj).
## 1) Izračun nazivnega toka
$$
I_n = \frac{S_n}{\sqrt{3} \cdot U_n} = \frac{25 \cdot 10^6}{\sqrt{3} \cdot 6300} \approx 2291\ \mathrm{A}
$$
## 2) Začetno stanje
Obremenitev z:
- $I' = 0{.}5 \cdot I_n = 1145{.}5\ \mathrm{A}$
- $\cos\varphi' = 0{.}8$

To stanje je **referenčno** – tu si izračunamo inducirano EMN $E_0$, ki je **nato nespremenjena**.
## 3) Izračun inducirane napetosti $E_0$
Za tok $I'$ in $\cos\varphi = 0.8 \Rightarrow \sin\varphi = 0.6$:
$$
E_0 = \sqrt{(U + I' X_s \cdot \sin\varphi)^2 + (I' X_s \cdot \cos\varphi)^2}
$$
Vstavimo podatke:
- $U = 6300\ \mathrm{V}$
- $X_s = 1{.}8\ \Omega$
$$
E_0 = \sqrt{(6300 + 1145{.}5 \cdot 1{.}8 \cdot 0{.}6)^2 + (1145{.}5 \cdot 1{.}8 \cdot 0{.}8)^2}
$$
$$
E_0 = \sqrt{(6300 + 1236{.}3)^2 + (1649{.}5)^2} \approx 7722\ \mathrm{V}
$$

## 4) Kritično (mejno) stanje: $\delta = 90^\circ$

Takrat je:

$$
E_0 = I_{om} \cdot X_s \Rightarrow I_{om} = \frac{E_0}{X_s} = \frac{7722}{1{.}8} \approx 4290\ \mathrm{A}
$$


## 5) Izračun navidezne in delovne moči

$$
S_{om} = \sqrt{3} \cdot U \cdot I_{om} = \sqrt{3} \cdot 6300 \cdot 4290 \approx 46{.}8\ \mathrm{MVA}
$$

$$
\cos\varphi_{om} = \frac{U}{E_0} = \frac{6300}{7722} \approx 0{.}816
$$

$$
P_{om} = S_{om} \cdot \cos\varphi_{om} \approx 46{.}8 \cdot 0{.}816 \approx 38{.}2\ \mathrm{MW}
$$
# Lab
![Kolokvij.2.2.webp](/img/user/Attachments/izpiti/Kolokvij.2.2.webp)
# Naloga 5
Trifazni transformator s podano napisno tablico obratuje na nazivnem omrežju in napaja trifazni elektromotor.

Analizator moči na sekundarni strani kaže naslednje vrednosti:
- Medfazna napetost: $U_2 = 220{.}4\ \mathrm{V}$
- Linijski tok: $I_2 = 9{.}2\ \mathrm{A}$
- Faktor delavnosti: $\cos\varphi = 0{.}85$
### Napisna tablica transformatorja:
| Parameter | Vrednost          |
|----------|-------------------|
| Moč      | 5 kVA             |
| Primar   | 400 V / 7{.}3 A   |
| Sekundar | 220 V / 13{.}1 A  |
| Frekvenca| 50 Hz             |
| Vezava   | Dyn5              |

Kolikšen je izkoristek transformatorja v tem obratovalnem stanju,  
če ima:
- nazivno izgubo v jedru: $P_{Fe} = 45\ \mathrm{W}$  
- nazivno izgubo v navitjih: $P_{Cu} = 98\ \mathrm{W}$
## Rešitev
### 1. Izračun trenutne navidezne moči:
Ker gre za trifazni transformator:
$$
S' = \sqrt{3} \cdot U_2 \cdot I_2 = \sqrt{3} \cdot 220{.}4\ \mathrm{V} \cdot 9{.}2\ \mathrm{A} \approx 3511\ \mathrm{VA}
$$

(če uporabiš enofazno oceno $U \cdot I = 2027\ \mathrm{VA}$, to velja le za eno fazo — a za boljši približek upoštevamo trifazno vrednost)
### 2. Prilagoditev izgub v navitju

Ker je trenutni tok večji od nazivnega, se izgube v Cu povečajo sorazmerno s kvadratom toka:

$$
P_{Cu}' = P_{Cu,n} \cdot \left( \frac{I_2}{I_{2n}} \right)^2 = 98 \cdot \left( \frac{9{.}2}{13{.}1} \right)^2 \approx 48{.}3\ \mathrm{W}
$$
### 3. Skupne izgube:
$$
P_{\text{izg}}' = P_{Fe} + P_{Cu}' = 45 + 48{.}3 = 93{.}3\ \mathrm{W}
$$
### 4. Izkoristek:

$$
\eta = \frac{S' - P_{\text{izg}}'}{S'} = \frac{3511 - 93{.}3}{3511} \approx 0{.}973
$$
