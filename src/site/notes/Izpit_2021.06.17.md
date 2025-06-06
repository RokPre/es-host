---
{"dg-publish":true,"permalink":"/izpit-2021-06-17/","tags":["unfinished"]}
---

# Naloga 1

Trifazni distribucijski transformator ima naslednje nazivne podatke:  
$S_{n} = 100\ \text{kVA}$ | $U_{1n} = 21\ \text{kV}$ | $U_{2n} = 0.42\ \text{kV}$ | vezava: Yzn5.  

Na transformatorju smo opravili preizkus prostega teka in preizkus kratkega stika. Izmerjene vrednosti so:  
- **Prosti tek**: $U_{10} = U_{1n}$ | $I_{10} = 0{.}01 \cdot I_{n}$ | $P_{0} = 150\ \text{W}$  
- **Kratek stik**: $U_{1k} = 840\ \text{V}$ | $I_{1k} = I_{n}$ | $P_{k} = 1375\ \text{W}$

## a) Kolikšne so izgube v transformatorju pri nazivni obremenitvi?

Pri nazivni obremenitvi se upoštevajo izgube v železu (merjene pri prostem teku) in izgube v bakru (merjene pri kratkem stiku):

$$
P_{\text{izg}} = P_{Cu} + P_{Fe} = P_{k} + P_{0} = 1375\ \text{W} + 150\ \text{W} = 1525\ \text{W}
$$

## b) Kolikšna je napetost med priključkoma $2U$ in $2N$, ko transformator deluje v prostem teku pri nazivni napetosti?
[[Predavanje 7#Yzn5\|Predavanje 7#Yzn5]]

Vezava Yzn5 pomeni, da je sekundarna stran vezana cikcak s faznim zamikom 150°. Pri prostem teku je izhodna napetost enaka nazivni. Fazna napetost sekundarja se izračuna iz medfazne:

$$
U_{mf} = 0{.}42\ \text{kV} \quad \Rightarrow \quad U_{f} = \frac{U_{mf}}{\sqrt{3}} \approx 0{.}242\ \text{kV}
$$

Napetost med priključkoma $2U$ in $2N$ je torej:

$$
U_{2U,2N} = U_f \approx 242\ \text{V}
$$

## c) Kolikšna je relativna vrednost kratkostične impedance transformatorja?

Relativna kratkostična napetost $u_k$ je definirana kot:

$$
u_k = \frac{U_{1k}}{U_{1n}} = \frac{840\ \text{V}}{21\,000\ \text{V}} = 0{.}04 = 4\%
$$

# Naloga 2

Trifazni sinhronski turbogenerator ima podane naslednje nazivne podatke:  
$S_n = 214\ \text{MVA}$ | $U_n = 10{.}5\ \text{kV}$ | $f_n = 50\ \text{Hz}$ | $n_n = 3000\ \text{min}^{-1}$ | $\cos \varphi_n = 0{.}8$ | $I_{vn} = 2{.}1\ \text{kA}$  

V tehnični dokumentaciji je podana tudi sinhronska reaktanca generatorja:  
$X_s = 160\%$

## a) Kolikšen je statorski tok generatorja, ko je ta nazivno obremenjen?

Nazivni tok generatorja lahko izračunamo iz nazivne moči in napetosti:

$$
S_{n} = \sqrt{ 3 } U_{2n}I_{2n} = I_s = \frac{S_n}{\sqrt{3} \cdot U_n}
$$

Vstavimo vrednosti (pozor: pretvori v osnovne enote):

$$
I_s = \frac{214 \cdot 10^6\ \text{VA}}{\sqrt{3} \cdot 10{.}5 \cdot 10^3\ \text{V}} = \frac{214 \cdot 10^6}{18{.}186 \cdot 10^3} \approx 11{.}76\ \text{kA}
$$

Torej je:

$$
I_s \approx 11{.}76\ \text{kA}
$$

To je **nazivni statorski tok**, ki teče pri polni (nazivni) obremenitvi generatorja.

## b) Koliko polov ima magnetno polje, ki ga ustvari rotorsko navitje?

Za sinhronski stroj velja:

$$
n_n = \frac{f}{p_p} \cdot 60 \quad \Rightarrow \quad p_p = \frac{f \cdot 60}{n_n}
$$

kjer je $p_p$ število **polparov**. Torej:

$$
p_p = \frac{50 \cdot 60}{3000} = 1 \quad \Rightarrow \quad p = 2
$$

Generator ima torej **dva pola**, kar je značilno za **turbogeneratorje**, ki obratujejo pri visoki hitrosti (3000 vrt/min).

# Naloga 3

Trifazni asinhronski motor s kratkostično kletko ima naslednje nazivno podane podatke:  
$P_n = 3\ \text{kW}$ | $U_n = 400\ \text{V}$ | $f_n = 50\ \text{Hz}$ | $I_n = 6\ \text{A}$ | $\cos(\varphi_n) = 0{.}85$ | $n_n = 1440\ \text{min}^{-1}$

Izgube zaradi trenja in ventilacije v prostem teku znašajo $P_{tr+v} = 16\ \text{W}$.

## a) Kolikšen je nazivni izkoristek motorja?
Izkoristek motorja je podan kot razmerje med mehansko močjo na gredi in skupnim dovodom električne moči. Če upoštevamo le izgube trenja in ventilacije (kar je poenostavitev), velja:

$$
\eta = \frac{P_n - P_{\text{izg}}}{P_n} = \frac{3000 - 16}{3000} = \frac{2984}{3000} \approx 0{.}9947 = 99{.}5\%
$$

Opomba: v resnici bi morali upoštevati še izgube v bakru, železu in druge mehanske izgube, a ker naloga eksplicitno poda le $P_{\text{izg}} = 16\ \text{W}$, je rezultat veljaven v tem kontekstu.

## b) Kolikšna je hitrost vrtilnega magnetnega polja, ki ga ustvari statorski tok v nazivnem obratovanju?
Vrtilna hitrost magnetnega polja (sinhronska hitrost) je določena z:

$$
n_s = \frac{60 \cdot f}{p_p}
$$

kjer je $p_p$ število polparov. Ker je podana mehanska hitrost rotorja $n_n = 1440\ \text{min}^{-1}$, iščemo $n_s$, ki je malenkost višji. Najbližja možna sinhronska hitrost je:

$$
n_s = 1500\ \text{min}^{-1}
$$

kar ustreza dvopolnemu stroju ($p_p = 2$). To je torej **hitrost vrtilnega magnetnega polja statorja**.

## c) Kolikšen je zdrs (slip) motorja pri preizkusu kratkega stika?
Pri preizkusu kratkega stika (t. i. blokiran rotor) se rotor ne vrti, kar pomeni $n_r = 0$. Zdrs je definiran kot:

$$
s = \frac{n_s - n_r}{n_s} = \frac{1500 - 0}{1500} = 1
$$

Torej je zdrs pri kratkem stiku enak:

$$
s = 1 \quad \text{ali} \quad 100\%
$$
# Naloga 4

Tuje vzbujan enosmerni kolektorski generator ima podane naslednje nazivne podatke:  
$P_n = 40\ \text{kW}$ | $U_n = 200\ \text{V}$ | $n_n = 1500\ \text{min}^{-1}$ | $I_v = 12\ \text{A}$ | $U_v = 136\ \text{V}$

Generator se vrti z nazivno vrtilno hitrostjo, vzbujalni tok pa je nastavljen tako, da je inducirana napetost enaka nazivni, torej $E = U_n = 200\ \text{V}$.  
Na generator je priključeno breme z upornostjo $R_b = 1{.}8\ \Omega$, napetost na sponkah rotorja pa je $U = 180\ \text{V}$. Padec napetosti na ščetkah je zanemarjen.

---

## a) Kolikšna je oddana moč generatorja v tem obratovalnem stanju?

Ker je generator priključen na upornost $R_b$, lahko moč na bremenu izrazimo kot:

$$
P = \frac{U^2}{R_b} = \frac{180^2}{1{.}8} = \frac{32400}{1{.}8} = 18000\ \text{W} = 18\ \text{kW}
$$

Generator torej v tem stanju oddaja **18 kW** električne moči.

## b) Kolikšna je upornost statorskega navitja rotorja?
Uporaba osnovne enačbe za enosmerni stroj:

$$
U = E - I_r \cdot R_r
$$

kjer je:
- $U = 180\ \text{V}$ (spremljana napetost na sponkah),
- $E = 200\ \text{V}$ (inducirana napetost),
- $I_r$ ... tok skozi rotor, ki ga izračunamo iz:

$$
I_r = \frac{U}{R_b} = \frac{180}{1{.}8} = 100\ \text{A}
$$

Zdaj lahko izračunamo notranjo upornost rotorja:

$$
R_r = \frac{E - U}{I_r} = \frac{200 - 180}{100} = \frac{20}{100} = 0{.}2\ \Omega
$$

### Rezultat:
Upornost rotorskega navitja znaša:

$$
R_r = 0{.}2\ \Omega
$$
