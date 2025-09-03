Rotační kužel o objemu 1970 cm^3 svírá strana kužele s rovinou podstavy úhel 60°, vypočtěte poloměr podstavy kužely.

Je dán kolmý hranol jehož podstavou je čtverec, tělesová úhlopříčka tohoto hranolu má délku $\sqrt{41}cm$ se čtvercovou podstavou svírá úhel $\phi=28°$
a) vypočítejte výšku hranolu
b) vypočítejte povrch hranolu

Železný váleček má obvod podstavy $28\pi$ cm, dělník do válečku vyvrtá díru, přičemž vrták byl celou dobu kolmo k podstavě. Po vyvrtání otvoru skrz váleček měl daný výrobek o 35% menší objem než původní váleček. Vypočítejte povrch vzniklého výrobku, víte-li, že obvod otvoru v podstavě je roven výšce válečku.

### Úloha 1 – Rotační kužel

Objem kužele je dán vzorcem  

$$
V=\frac{1}{3}\pi r^{2}h \;=\; 1970\;\text{cm}^{3}.
$$

Úhel mezi tvořící $l$ a rovinou podstavy je  

$$
\alpha = 60^{\circ}, \qquad 
\tan\alpha \;=\; \frac{h}{r}
\;\Longrightarrow\;
h \;=\; r\tan60^{\circ} \;=\; r\sqrt3.
$$

Dosadíme do vzorce pro objem:  

$$
\frac13\pi r^{2}(r\sqrt3) \;=\; \frac{\sqrt3}{3}\,\pi r^{3} \;=\; 1970
\;\Longrightarrow\;
r^{3} \;=\; \frac{5910}{\pi\sqrt3}.
$$

$$
\boxed{\,r \;=\; \Bigl(\tfrac{5910}{\pi\sqrt3}\Bigr)^{1/3}\ \text{cm} 
      \;\approx\; 10.28\ \text{cm}\,}.
$$



---

### Úloha 2 – Kolmý hranol se čtvercovou podstavou

Označme  
* $a$ – délka hrany čtverce,  
* $h$ – výška hranolu,  
* $d=\sqrt{41}\,\text{cm}$ – tělesová úhlopříčka,  
* $\varphi = 28^{\circ}$ – úhel mezi tělesovou úhlopříčkou a rovinou podstavy.

#### Geometrické vztahy

1. Pythagorova věta v kvádru  

   $$
   d^{2} \;=\; a^{2}+a^{2}+h^{2} \;=\; 2a^{2}+h^{2}.
   $$

2. Definice úhlu $\varphi$  

   $$
   \tan\varphi \;=\; \frac{h}{a\sqrt2}
   \quad\Longrightarrow\quad
   h \;=\; a\sqrt2\,\tan\varphi.
   $$

#### a) Výška hranolu

Dosadíme $h$ do rovnice pro $d$:

$$
d^{2}
  = 2a^{2}\bigl(1+\tan^{2}\varphi\bigr)
  = 2a^{2}\sec^{2}\varphi
  \;\Longrightarrow\;
  a^{2} = \frac{d^{2}}{2}\cos^{2}\varphi.
$$

$$
a = \frac{\sqrt{41}\,\cos28^{\circ}}{\sqrt2}
    \;\approx\; 4.00\;\text{cm},
\qquad
h = a\sqrt2\,\tan28^{\circ}
    \;\approx\; 3.01\;\text{cm}.
$$

$$
\boxed{h \;\approx\; 3.01\ \text{cm}}
$$

#### b) Povrch hranolu

$$
S
  = 2a^{2}+4ah
  = 2a^{2}+4a\bigl(a\sqrt2\,\tan\varphi\bigr)
  \;\approx\; 80.0\;\text{cm}^{2}.
$$

$$
\boxed{S \;\approx\; 80.0\ \text{cm}^{2}}
$$



---

### Úloha 3 – Vyvrtaný železný váleček

#### 1. Původní váleček  
Obvod podstavy:  

$$
2\pi R = 28\pi
\;\Longrightarrow\;
R = 14\ \text{cm}.
$$

Objem:  

$$
V_{0}= \pi R^{2}H = 196\pi H.
$$


#### 2. Otvor (vrtaný válec)  
Nechť poloměr otvoru je $r$. Zadání dává  

$$
2\pi r = H 
\quad\Longrightarrow\quad
H = 2\pi r.
$$

Objem odebraného materiálu:

$$
V_{\text{otvor}} = \pi r^{2}H = 2\pi^{2}r^{3}.
$$

#### 3. Rovnice pro úbytek objemu

Po odvrtání zůstalo $65\%$ původního objemu:

$$
V_{\text{otvor}} 
   = 0.35\,V_{0}
   \quad\Longrightarrow\quad
   2\pi^{2}r^{3}
     = 0.35\cdot 196\pi H.
$$

S využitím $H=2\pi r$:

$$
2\pi^{2}r^{3}
  = 0.35\cdot 196\pi (2\pi r)
  \;\Longrightarrow\;
  r^{2}=68.6
  \;\Longrightarrow\;
  r\approx 8.28\ \text{cm},\qquad
  H\approx 52.05\ \text{cm}.
$$

#### 4. Povrch výsledného tělesa

Součásti povrchu  

* **vnější plášť:** $2\pi R H$,  
* **dvě mezikruhové podstavy:** $2\pi(R^{2}-r^{2})$,  
* **vnitřní plášť otvoru:** $2\pi r H$.

Celkem:

$$
\begin{aligned}
S 
&= 2\pi R H + 2\pi r H + 2\pi\bigl(R^{2}-r^{2}\bigr) \\[2pt]
&\approx 8086\ \text{cm}^{2}.
\end{aligned}
$$

$$
\boxed{S \;\approx\; 8086\ \text{cm}^{2}}
$$



---

### Rychlý přehled výsledků

| Úloha | Hledaná veličina     | Výsledek                          |
| ----- | -------------------- | --------------------------------- |
| 1     | poloměr kužele \(r\) | \($\approx 10.28\ \text{cm}$\)    |
| 2     | výška hranolu \(h\)  | \($\approx 3.01\ \text{cm}$\)     |
|       | povrch hranolu \(S\) | \($\approx 80.0\ \text{cm}^{2}$\) |
| 3     | povrch výrobku \(S\) | \($\approx 8086\ \text{cm}^{2}$\) |













Odchylka přímky od roviny je odchylka od jejího pravúhlého průmětu této přímky s  přímkou p

Vzdálenost bodu od přímky 
