---
{"dg-publish":true,"permalink":"/kolokvij-1/","tags":["unfinished"]}
---

# Naloga 1
Na osnovi podane vezalne sheme doloćite vezno skupino in fazno številko trifaznega transformatorja s podatki $S_{n} = 250kVA$, $U_{1n} = 10kV$, $u_{k} = 4\%$. Ali je vezava pravilna (odgovor obvezno utemeljite)? Določite sekundarno medfazno napetost $U_{2n}$, če se v posamezni sekundarni tuljavici inducira napetost $200V$. K temu transformatorju želimo paralelno priključiti transfomator s podakti $S_{n} 200kVA$, $10/0.5kV$, $u_{k} = 6\%$, $Dz6$. Ali je zakšno pararelno obratovanje dopustno (odgovor obeno utemeljite)?
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
Sinhronski turbogeneator $S_{n} = 200MVA$, $U_{2n} = 15kV$, $\cos(\varphi_{2n}) = 0.8$, $X_{^{2}} = 1.4$, $I_{1n} = 300A$ obratuje na togem nazivnem omrežju pri obremenizvi $S' = 100MVA$, $\cos(\varphi_{2}')=0.6$. Za to obratovalno stanje določite potreben vzbujalni tok $I_{1}$ in oba kolesna kota $\delta_{n}$ in $\delta'$ (obvezna tudi skica obeh obratovlanih stanj).

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
## 1) Kolikšten je statorksi tok v tem obratovlanem stanju generatorja?
$I_{s} = ?$
$$
\frac{I_{1}'}{I_{n}} = \frac{E_{0}'}{E_{0,n}}
$$
$$
E_0 = \sqrt{(U_2 + I_2 X_s \cdot \sin\varphi)^2 + (I_2 X_s \cdot \cos\varphi)^2}
$$
