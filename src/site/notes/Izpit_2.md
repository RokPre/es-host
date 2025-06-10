---
{"dg-publish":true,"permalink":"/izpit-2/","tags":["unfinished"]}
---

![Izpit.2.1.png](/img/user/Attachments/izpiti/Izpit.2.1.png)
# Naloga 1
Trifazni distribucijski transfomator ima nazivne podakte: $S_{n} = 1000kVA$ | $U_{1,n} = 21kV$|$U_{2,n} = 0.42kV$ | $Dyn5$. Na transformatorju je bil opravljen preizkus kratkega stika, katerega rezultati so: $U_{1,k} = 126V$ | $I_{1,k} = I_{n}$ | $P_{1,k} = 13.2kW$.
Transformator je priključen na omrežje nayivne napetosti pri frekvenci $60 Hz$.
## a) Kolikšna je napetost med priključkoma $2V$ in $2N$, ko transformator na omenjenem omrežju obratuje v prostem teku?
Nazivna linijska napetost sekundarja: $U_{2,n} = 0.42\ \text{kV} = 420\ \text{V}$.
Fazna napetost sekundarja (napetost med fazo in nevtralno točko v zvezdi):
$$U_{2,f} = \frac{U_{2,n}}{\sqrt{3}}$$
$$U_{2,f} = \frac{420\ \text{V}}{\sqrt{3}} \approx \mathbf{242.49\ \text{V}}$$

## b) Kolikšne so izgube v navitjih transformatorja, če ga na sekundarni strani obremenimo s čistim ohmskim bremenom in s polovičnim nazivnim tokom?
Bakrene izgube pri nazivnem toku: $P_{Cu,n} = P_{1,k} = 13.2\ \text{kW} = 13200\ \text{W}$.
Transformator je obremenjen s polovičnim nazivnim tokom, kar pomeni, da je relativni tok $I'/I_n = 0.5$.
Izgube v navitjih pri polovičnem toku ($P_{Cu}'$) se izračunajo kot:
$$\frac{P_{Cu}'}{P_{Cu,n}} = \left(\frac{I'}{I_n}\right)^2$$
$$P_{Cu}' = P_{Cu,n} \cdot \left(\frac{I'}{I_n}\right)^2$$
$$P_{Cu}' = 13200\ \text{W} \cdot (0.5)^2$$
$$P_{Cu}' = 13200\ \text{W} \cdot 0.25$$
$$P_{Cu}' = \mathbf{3300\ \text{W}}$$

## c) Kolikšna je kratkostična impedanca transformatorja?
Nazivna moč: $S_n = 1000\ \text{kVA} = 10^6\ \text{VA}$.
Nazivna primarna linijska napetost: $U_{1,n} = 21\ \text{kV} = 21000\ \text{V}$.
Nazivni primarni tok ($I_{1,n}$) za trifazni transformator:
$$I_{1,n} = \frac{S_n}{\sqrt{3} \cdot U_{1,n}}$$
$$I_{1,n} = \frac{10^6\ \text{VA}}{\sqrt{3} \cdot 21000\ \text{V}}$$
$$I_{1,n} = \frac{10^6\ \text{VA}}{36376.3\ \text{V}} \approx 27.49\ \text{A}$$
Kratkostična impedanca ($Z_k$):
$$Z_k = \frac{U_{1,k}}{I_{1,k}}$$
$$Z_k = \frac{126\ \text{V}}{27.49\ \text{A}}$$
$$Z_k \approx \mathbf{4.58\ \Omega}$$
# Naloga 2
Trifazni sinhrosnki turbogenerator z nazivnimi podatki: $S_{n} = 40kVA$ | $U_{n} = 400V$ | $f_{n} = 50Hz$ | $n_{n} = 1500\text{min}^{-1}$ | $\cos(\varphi_{n} = 0.85)$ obratuje na nazivnem omrežju in v omrežje oddaja električno moč $P = 40kW$. Pri tem je vzbujanje nastavljeno na dvakratno vrednost vzbujalnega toka prostega tek.
## a) Kolikšen je statorksi tok v tem obratovlanem stanju generatorja?
$I_{2}' = ?$
$I_{1}' = 2\cdot I_{1,n}$
$U_{2}' = U_{2,n}$
$$
I_{2}' = \frac{S'}{S_{n}}I_{2,n} = \frac{47058.8VA}{40000VA} \cdot 57.7A = 67.9A
$$
$$
I_{2,n} = \frac{S_{n}}{\sqrt{ 3 }U_{2,n}} = \frac{40000}{\sqrt{ 3 } 400} = 57.7A
$$
$$
S' = \frac{P}{\cos(\varphi_{n})} = \frac{40000}{0.85} = 47058.8VA
$$
## b) Kolikšna je relativna vrednost sinhrosnke reaktance generatorja?
$$
X_{sr} = ?
$$
NE ZNAM!
# Naloga 3
Trifaznemu asinhronskemu motorju s kratkostično kletko in z nazivnimi podatki: $P_{n} = 5.5kW$ | $U_{n} = 400V$ | $f_{n} = 50Hz$ | $I_{n} = 10.5A$ | $\cos(\varphi_{n}) = 0.88$ | $n_{n} = 2900\text{min}^{-1}$ ima statorke fazne tuljvae vezane v trikot, imzmerjna upornost vsake posamezne tuljave pa je $0.7\Omega$.
## a)
Kolikšne so izgube v statroskem navitju motorja v nazivnem obratovalnem stanju?
### Odgovor
$$
P_{cu,n} = ?
$$
Ker imamo trikot vezavo deljimo z $\sqrt{ 3 }$, ker gre samo toliko toka skozi eno navitje. Pomnožimo z 3, ker imamo 3 navitja.
$$
P_{cu,n} = 3 \cdot \left(\frac{I_{n}}{\sqrt{ 3 }}\right)^{2} R =3\left( \frac{10.5}{\sqrt{ 3 }} \right)^{2}0.7 = 77.2W
$$

## b) 
Kolikšna je oddana moč motorja, če obratuje pri napetosti $380V$ in nazivni hitrosti vrtenja
### Odgovor
$$
P=?
$$
$$
U_{1}' = 380V
$$
$$
n' = n_{n}
$$
$$
P = M\cdot \omega = M \cdot \frac{2 \pi \cdot n}{60} =16.34 \frac{2 \pi 2900}{60}= 4962.250\ldots
$$
$$
M =M_{n}\left( \frac{380}{400} \right)^{2} = 18.11*\left( \frac{380}{400} \right)^{2} = 16.344\ldots
$$
$$
M_{n}=\frac{P*60}{2\pi \cdot n_{n}} =\frac{5500*60}{2*\pi*2900} = 18.110\ldots
$$
## c)
Kolikšen je slip tega motorja pri preizkusu kratkega stika?
### Odgovor
Kratek stik pomeni, da se rotor ne vrti: 
$$
n_{r} = 0 \Rightarrow s = \frac{n_{s} - n_{r}}{n_{s}} = 1
$$
# Naloga 4
Enosmerni kolektorski generator s paralelnim vzbujanjem in nazivnimi podatki: $P_{n} = 5kW$ | $U_{n} = 300V$ | $n_{n} = 1000\text{min}^{-1}$ | $U_{vzb} = 300V$ ima na kolektorju dve ščetki, katerih padec napetosti je zanemarljiv, upornost statorskega navitja je $550\Omega$.

Pogonski stroj zagotavlja konstantno vtilno hitrost, generator pa je obremenjen z grelom, katerega upornost je $25\Omega$. Pri tem je napetost na bremenu $310V$.
## a) Rotorski tok
Ker gre za generator s paralelnim vzbujanjem, velja:
$$
I_{b} = I_{v}+I_{i}
$$
Najprej izračunamo tok skozi breme:
$$
I_b = \frac{U_b}{R_b} = \frac{310}{25} = 12{,}4\,\text{A}
$$
Vzbujalni tok:
$$
I_i = \frac{U_{vzb}}{R_i} = \frac{310}{550} \approx 0{,}5636\,\text{A}
$$
Ker tok armaturnega navitja nosi razliko:
$$
I_v = I_b - I_i = 12{,}4 - 0{,}5636 \approx 11{,}8364\,\text{A}
$$


## b) Število polov magnetnega polja



![Izpit.2.2.jpg](/img/user/Attachments/izpiti/Izpit.2.2.jpg)
# Naloga 5
[[Kolokvij_1#Naloga 5\|Kolokvij_1#Naloga 5]]

Za trifazni distribucijski transformator $S_{n} = 50kVA$, $U_{1,n} = 21kV$, $U_{2,n} = 0.42kV$, $f_{n} = 50Hz$, $Yzn_{5}$. Imamo na voljo rezultate meritev elektrićnih veličin na primarni strani pri preizkusu prostega teka, preizkus kratkega stika in obremenilnem preizkusu, vendar ni označeno, kateri rezulatai so za poosamezne obratovalno stanje:

- Meritev A: $U_{A} = 21.04kV$, $I_{A} = 0.012A$, $\cos(\varphi) = 0.186$
- Meritev B: $U_{B} = 21.03kV$, $I_{B} = 1.05A$, $\cos(\varphi) = 0.952$
- Meritev C: $U_{C} = 842.1V$, $I_{C} = 1.38A$, $\cos(\varphi) = 0.375$

Ugotovite in definirajte, kateri merilni rezultati ustrezajo posameznimu preizkusu. Izračunajte tudi, kolikšen je izkoristek transformatorja v izmerjenem obremenilnem stanju?

## Rešitev
A - prosti tek
B - Obremenitev
C - kratek stik

$$
P_{fe} = \sqrt{ 3 } \cdot 21040V \cdot 0.012A \cdot 0.186 = 81.3W
$$
$$
P_{cu} = \sqrt{ 3 } \cdot 842.1 \cdot 1.38 \cdot 0.375 = 754.8W
$$
$$
P_{cu}' = P_{cu}\left( \frac{I_{B}}{I_{C}} \right)^{2} = 754.8 \left( \frac{1.05}{1.38} \right)^{2}= 437W
$$
$$
\eta = \frac{\sqrt{ 3 }\cdot 21030 \cdot 1.05 \cdot 0.952 - (81.3+437)}{\sqrt{ 3 }\cdot 21030 \cdot 1.05 \cdot 0.952} = 0.985 = 98.5\%
$$

# Naloga 6
Trifazni sinhronski generator s cilindričnim rotorjem $S_{n} = 40\,\text{kVA}$, $U_{2,n} = 400\,\text{V}$, $f_{2,n} = 50\,\text{Hz}$, $n_{n} = 1500\,\text{min}^{-1}$, $\cos(\varphi_{2,n}) = 0.8$, ima v tehnični dokumentaciji podano tudi vrednost sinhronske reaktance $X_{sr} = 1.6$. Pogonski stroj zagotavlja nazivno in konstantno hitrost vrtenja rotorja.

Da smo pri preizkusu prostega teka na sponkah generatorja dobili nazivno napetost, smo vzbujalni tok nastavili na $I_{10} = 5\,\text{A}$. Pri nespremenjenem vzbujanju smo nato na generator priključili ohmsko breme, v katero je stekel tok $I_{2} = 30\,\text{A}$. Kolikšna sta napetost in moč na bremenu v tem obratovalnem stanju? Pri izračunu upoštevajte linearne magnetne razmere.

## Rešitev
$n_{0} =n_{n}$
$U_{0}=U_{n}$
$I_{1,0}'=5A$
$I_{2,b}'=30A$
$U_{b} =?$
$P_{b} =?$


### 1. Določitev elektromotorne sile $E_0$
Pri vzbujanju $I_{10} = 5\,\text{A}$ in napetosti v prostem teku $U_0 = 400\,\text{V}$ sledi:
$$
E = U_{f} = \frac{U_{mf}}{\sqrt{ 3 }} = \frac{U_{2,n}}{\sqrt{ 3 }}=\frac{400V}{\sqrt{ 3 }} = 231V
$$
$$
E_0 = 231\,\text{V}
$$
Ker predpostavljamo linearne magnetne razmere, se vrednost $E$ ne spremeni, če ostane vzbujevalni tok enak.

### 2. Napetost na bremenu $U_b$
Pri ohmskem bremenu je fazni kot $\varphi_2 = 0 \Rightarrow \cos(\varphi_2) = 1$, $\sin(\varphi_2) = 0$. Uporabimo formulo za razmerje med $E$, $U$ in $X_{sr}$:
$$
E^2 = U_b^2 + (I_2 X_{sr})^2
$$
Iz tega izrazimo napetost na bremenu:
$$
U_b = \sqrt{E^2 - (I_2 X_{sr})^2} = \sqrt{231^2 - (30 \cdot 1.6)^2} = 226V
$$

### 3. Moč na bremenu $P_b$
$$
P_b = \sqrt{3} \cdot U_b \cdot I_2 \cdot \cos(\varphi_2) = \sqrt{3} \cdot 226 \cdot 30 \cdot 1 = 11743W$$
