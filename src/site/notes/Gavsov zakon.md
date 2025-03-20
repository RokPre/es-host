---
{"dg-publish":true,"permalink":"/gavsov-zakon/","tags":["complete"]}
---

# Definicija
Gaussov zakon trdi, da je električni tok skozi zaprto površino sorazmeren z vsem nabojem znotraj te površine, deljenim s permitivnostjo vakuma. Električno polje, ki teče skozi površino, je povezano z naboji znotraj volumna, ki ga ta površina obdaja.

V matematični obliki to pomeni:
$$
\oint_{S}\vec{E}\;d\vec{A} = \frac{Q_{notranji}}{\epsilon_{0}}
$$
$S$ je zaprta površina (kontrolna površina), $\vec{E}$ je električno polje, $d\vec{A}$ pa je infinitesimalni vektor površine, ki je pravokoten na površino. $Q_{\text{notranji}}$ predstavlja neto naboj znotraj zaprtne površine, $\epsilon_0$ pa je permitivnost vakuma.

# Izvornost
Gaussov zakon nam tudi pove, da ima električno polje izvor, medtem ko magnetno polje nima izvora. To pomeni, da električne silnice izhajajo iz nabojev (ali se vanje vračajo), medtem ko magnetne silnice vedno tvorijo zaprte zanke.

Izvornost polja preverimo z divergenco. Divergenca električnega polja nam pove, ali polje ima izvor. Če je divergenca električnega polja enaka nič, polje nima izvora. V nasprotnem primeru pa je polje izvorno.
$$
\nabla \cdot \vec{E} = \frac{\rho}{\epsilon_{0}}
$$
kjer je $\rho$ gostota naboja.