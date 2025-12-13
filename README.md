# Projet — Mécanique Orbitale (ENS / M2)

Ce repo contient :
- le rapport (`Rapport détaillé.pdf`)
- les scripts Matlab (`Exercice I.mlx`, `exercice_II.mlx`)
- une page GitHub Pages (`index.html`) pour afficher les équations avec **KaTeX**.

## 1) Orbite elliptique — équations utilisées

Rayon orbital :
$
r(\nu)=\frac{a(1-e^2)}{1+e\cos\nu}.
$

Excentricité (à partir de deux points) :
$
e=\frac{r_2-r_1}{r_1\cos\nu_1-r_2\cos\nu_2}.
$

Vis-viva :
$
v=\sqrt{\mu\left(\frac{2}{r}-\frac{1}{a}\right)}.
$

Période :
$
T=2\pi\sqrt{\frac{a^3}{\mu}}.
$

## 2) Perturbation J2 — dérives séculaires

Avec $p=a(1-e^2)$ et $n=\sqrt{\mu/a^3}$ :
$
\dot{\Omega}=-\frac{3}{2}nJ_2\left(\frac{R_T}{p}\right)^2\cos i,
$
$
\dot{\omega}=\frac{3}{4}nJ_2\left(\frac{R_T}{p}\right)^2(4-5\sin^2 i).
$

Inclinaison critique (gel de $\omega$) :
$$
4-5\sin^2 i=0 \Rightarrow \sin^2 i=\frac{4}{5}.
$$

## 3) Transfert de Hohmann (rendez-vous)

Demi-grand axe de l’ellipse de transfert :
$$
a_T=\frac{r_1+r_2}{2}.
$$

Vitesses sur l’ellipse (périgée / apogée) :
$
v_{p,T}=\sqrt{\mu\left(\frac{2}{r_1}-\frac{1}{a_T}\right)},\quad
v_{a,T}=\sqrt{\mu\left(\frac{2}{r_2}-\frac{1}{a_T}\right)}.
$

Impulsions :
$
\Delta v_1=v_{p,T}-v_1,\quad \Delta v_2=v_2-v_{a,T},\quad \Delta v_{tot}=\Delta v_1+\Delta v_2.
$

Temps de vol (demi-période) :
$
T_{trans}=\pi\sqrt{\frac{a_T^3}{\mu}}.
$

Phasage (rendez-vous) :
$$
\varphi_0+n_2t_t=\pi \Rightarrow \varphi_0=\pi-n_2t_t.
$$

## 4) Masse d’ergols (Tsiolkovski)

$$
\Delta V=I_{sp}g_0\ln\left(\frac{m_0}{m_f}\right),
\quad
m_f=m_0\exp\left(-\frac{\Delta V}{I_{sp}g_0}\right),
\quad
m_{erg}=m_0-m_f.
$$
