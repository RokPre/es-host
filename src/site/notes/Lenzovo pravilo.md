---
{"dg-publish":true,"permalink":"/lenzovo-pravilo/","tags":["unfinished"]}
---

**LENZOVO PRAVILO NAM POVE SAMO SMER INDUCIRANE NAPETOSI**.
**FARADEJEVO PRAVILO PA NAM POVE DA SE NAPETOST INDUCIRA**

Lenzovo pravilo pravi, da smer induciranega toka v zanki vedno nasprotuje spremembi, ki je povzročila ta tok. To pomeni, da inducirani tok poskuša nasprotovati vzroku, zaradi katerega nastane.

Če v magnetnem polju hitro premikamo magnet proti tuljavi žice, se v žici inducira tok. Lenzovo pravilo pravi, da bo smer toka tak, da bo ustvaril magnetno polje, ki bo poskušalo preprečiti premikanje magneta proti žici (torej, bo nastal tok, ki ustvarja magnetno polje nasprotne smeri).

Na ta način inducirani tok vedno deluje proti spremembi, ki povzroči njegov nastanek.

Če imamo fluks $\Phi(t)$, ki se spreminja z obliko $\sin(t)$ bo inducirana napetost $e(t)$ imela obliko $-\cos(x)$, ker velja $e(t) = -\frac{d\Phi(t)}{dt}$. Tako bo na kazalčnem diagramu inducirana napetost zaostjala za $\frac{\pi}{2} = 90°$.

```mathpad
plot(sin(x), -cos(x))==?
```
