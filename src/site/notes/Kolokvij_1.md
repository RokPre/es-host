---
{"dg-publish":true,"permalink":"/kolokvij-1/","tags":["unfinished"]}
---

![Kolokvij 1.1.jpg](/img/user/Attachments/izpiti/Kolokvij%201.1.jpg)
# Naloga 1
Na osnovi podane vezalne sheme doloćite vezno skupino in fazno številko trifaznega transformatorja s podatki $S_{n} = 250kVA$, $U_{1n} = 10kV$, $u_{k} = 4\%$. Ali je vezava pravilna (odgovor obvezno utemeljite)? Določite sekundarno medfazno napetost $U_{2n}$, če se v posamezni sekundarni tuljavici inducira napetost $200V$. K temu transformatorju želimo paralelno priključiti transfomator s podakti $S_{n} = 200kVA$, $10/0.5kV$, $u_{k} = 6\%$, $Dz6$. Ali je takšno pararelno obratovanje dopustno (odgovor obeno utemeljite)?
### 1. Vezna skupina
Iz kazalčnega diagrama in podanih faznih kotov ugotovimo, da gre za:
$$
\text{Vezna skupina:} \quad Yz5
$$
### 2. Ali je vezava pravilna?
Da, vezava je pravilna. Kazalci faznih napetosti na sekundarni strani tvorijo enakostranični trikotnik z medsebojnimi koti $120^\circ$ in enakimi amplitudami, kar pomeni, da je sistem **simetričen**, zaporedje faz pa **desnosučno**.
### 3. Sekundarna medfazna napetost
Če je napetost posamezne sekundarne tuljavice (fazna napetost pri cikcak vezavi):
$$
U_{2f} = 200\ \text{V}
$$
potem je medfazna napetost (cikcak):
$$
U_{2mf} = \sqrt{3} \cdot U_{2f} = \sqrt{3} \cdot 200\ \text{V} \approx 346{.}4\ \text{V}
$$
### 4. Ali je možno paralelno obratovanje?
Vzporedno (paralelno) obratovanje **ni možno**, saj se fazni številki transformatorjev ne ujemata.

Za uspešno paralelno obratovanje mora biti izpolnjen pogoj:
$$
(n_1 - n_2)\mod 4 = 0
$$
V našem primeru:
$$
(6 - 5)\mod 4 = 1 \ne 0
$$
Zato med transformatorjema obstaja **fazen zamik**, ki onemogoča delovanje brez krožnih tokov.

# Naloga 2
Pri preizkusu prostega teka transofmatorja na nazivnem omrežju izmerimo izgube $P_{0} = 300W$. Pri preizkusu kratkega stika pri nazivnem tokku imerimo izgube $P_{ks} = 900W$. Izračunajte na katero nadtemperaturo $\vartheta_{max,0}$ se segreje neobremenjen transofmator priključne na nazivno omrežje, će se pri nazivni obremenitivi segreje na nadtemeraturo $\vartheta_{man,n} = 80^{\circ}C$.

## Rešitev
Pri nazivni obremenitvi so skupne izgube:
$$
P_{\text{izg},n} = P_{Fe} + P_{Cu} = 300 + 900 = 1200\ \text{W}
$$
Pri prostem teku so prisotne **samo izgube v železu**:
$$
P_{\text{izg},0} = P_{Fe} = 300\ \text{W}
$$
Nadtemperatura v transformatorju je sorazmerna s skupnimi izgubami:
$$
\frac{\vartheta_{\text{max},0}}{\vartheta_{\text{max},n}} = \frac{P_{Fe}}{P_{Fe} + P_{Cu}} = \frac{300}{1200} = \frac{1}{4}
$$
Zato:
$$
\vartheta_{\text{max},0} = \frac{1}{4} \cdot 80^\circ\text{C} = 20^\circ\text{C}
$$

# Naloga 3
Sinhronski turbogenerator $S_n = 200\ \mathrm{MVA}$, $U_n = 15\ \mathrm{kV}$, $\cos\varphi_{2n} = 0{.}8$, $X_{sr} = 1{.}4$, $I_n = 300\ \mathrm{A}$ obratuje na togem nazivnem omrežju pri obremenitvi $S' = 100\ \mathrm{MVA}$, $\cos\varphi_{2}' = 0{.}6$. Za to obratovalno stanje določite potreben vzbujalni tok $I_1'$ in oba kolesna kota $\delta_n$ in $\delta'$ (obvezna tudi skica obeh obratovalnih stanj).

## 1. Izračun nazivnega toka $I_{2n}$

$$
I_{2n} = \frac{S_n}{\sqrt{3} \cdot U_{2n}} = \frac{200 \cdot 10^6}{\sqrt{3} \cdot 15\,000} \approx 7698\ \text{A}
$$
## 2. Kolesni kot $\delta_n$

$\cos\varphi_{2n} = 0.8 \Rightarrow \sin\varphi_{2n} = 0.6$

$$
\tan\delta_n = \frac{I_{2n} \cdot X_s \cdot \cos\varphi_{2n}}{U_{2n} + I_{2n} \cdot X_s \cdot \sin\varphi_{2n}}
$$

$$
\tan\delta_n = \frac{7698 \cdot 1{.}4 \cdot 0{.}8}{15\,000 + 7698 \cdot 1{.}4 \cdot 0{.}6}\approx 0{.}4014
$$

$$
\delta_n \approx \arctan(0{.}4014) \approx 21{.}9^\circ
$$
## 3. Kolesni kot $\delta'$

Za obremenitev $S' = 100\ \text{MVA}$ in $\cos\varphi_2' = 0.6$:

$$
I_{2}' = \frac{S'}{\sqrt{3} \cdot U_{2n}} = \frac{100 \cdot 10^6}{\sqrt{3} \cdot 15\,000} \approx 3849\ \text{A}
$$

$\sin\varphi_2' = 0.8$

$$
\tan\delta' = \frac{3849 \cdot 1{.}4 \cdot 0{.}6}{15\,000 + 3849 \cdot 1{.}4 \cdot 0{.}8} = \frac{3229{.}18}{19\,308{.}48} \approx 0{.}1672
$$

$$
\delta' \approx \arctan(0{.}1672) \approx 9{.}5^\circ
$$

# Naloga 4
Trifazni sinhrnski generator z nazivnimi podatki $S_{n} = 50kVa$, $U_{2n} = 400V$ , $f_{n} = 50Hz$, $\cos(\varphi_{2n}) = 0.8$, $n_{n} = 1000\text{min}^{-1}$ obratuje na nazivnem omrežju in je obremenenjen z močjo $P' = 50kW$. Vzbujanje je nastavljeno na 2-kratno vrednost vzbujanjega toka prostega teka.

## 1) Kolikšen je statorski tok $I_s$ v tem obratovalnem stanju?
$U' = U_{n}$, $P' = S_{n} = 50kW, \Rightarrow \cos(\varphi_{2}') = 1$, $I_{v}' = 2I_{v,0}$.
$S' = \sqrt{ 3 } U' I' \Rightarrow I' = \frac{50000}{\sqrt{ 3 } \cdot 400} \approx 72A$

## 2) Kolikšna je relativna vrednost sinhronske reaktance generatorja?

Relativna sinhronska reaktanca:

$$
X_s = \frac{U_{2n}}{I_{2n}} = \frac{400}{72{.}17} \approx 5{.}54\ \Omega
$$

To je **osnovna vrednost reaktance**, lahko jo vzamemo kot baza za pretvorbo v per unit, če je to smiselno.
## 3) Koliko polov ima magnetno polje?
$$
n_n = \frac{f \cdot 60}{p_p} \Rightarrow p_p = \frac{f \cdot 60}{n_n} = \frac{50 \cdot 60}{1000} = 3
$$
Število polov:
$$
p = 2 \cdot p_p = 6
$$

![Kolokvij 1.2.jpg](/img/user/Attachments/izpiti/Kolokvij%201.2.jpg)

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
$$
P_{Fe} = U_C \cdot I_C \cdot \cos\varphi = 20\,040 \cdot 0{.}012 \cdot 0{.}186 \approx \boxed{44{.}7\ \text{W}}
$$
### 2. **Izgube v bakru** $P_{Cu}$  
(iz meritve kratkega stika = meritev **B**)
$$
P_{Cu} = U_B \cdot I_B \cdot \cos\varphi = 824{.}3 \cdot 1{.}38 \cdot 0{.}375 \approx \boxed{426{.}5\ \text{W}}
$$