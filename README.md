# Orbital Mechanics Project — Summary

This project studies basic orbital mechanics and mission analysis, including
Keplerian orbits, J2 perturbations, Hohmann transfers, rendez-vous phasing,
and propellant mass estimation. Numerical simulations are implemented in MATLAB
and compared with analytical results.

---

## Keplerian orbit

Orbital radius as a function of true anomaly:

$$
r(\nu)=\frac{a(1-e^2)}{1+e\cos\nu}
$$

Orbital velocity (vis-viva equation):

$$
v=\sqrt{\mu\left(\frac{2}{r}-\frac{1}{a}\right)}
$$

Orbital period:

$$
T=2\pi\sqrt{\frac{a^3}{\mu}}
$$

---

## J2 perturbation (secular effects)

Definitions:

$$
p=a(1-e^2)
$$

$$
n=\sqrt{\frac{\mu}{a^3}}
$$

RAAN drift:

$$
\dot{\Omega}=-\frac{3}{2}nJ_2\left(\frac{R_T}{p}\right)^2\cos i
$$

Argument of perigee drift:

$$
\dot{\omega}=\frac{3}{4}nJ_2\left(\frac{R_T}{p}\right)^2(4-5\sin^2 i)
$$

---

## Hohmann transfer

Transfer orbit semi-major axis:

$$
a_T=\frac{r_1+r_2}{2}
$$

Velocity increments:

$$
\Delta v_1=\sqrt{\mu\left(\frac{2}{r_1}-\frac{1}{a_T}\right)}-\sqrt{\frac{\mu}{r_1}}
$$

$$
\Delta v_2=\sqrt{\frac{\mu}{r_2}}-\sqrt{\mu\left(\frac{2}{r_2}-\frac{1}{a_T}\right)}
$$

Total transfer cost:

$$
\Delta v_{tot}=\Delta v_1+\Delta v_2
$$

Transfer time:

$$
T_{trans}=\pi\sqrt{\frac{a_T^3}{\mu}}
$$

---

## Rendez-vous phasing

Initial phase condition:

$$
\varphi_0=\pi-n_2T_{trans}
$$

---

## Propellant mass (Tsiolkovsky)

$$
\Delta V=I_{sp}g_0\ln\left(\frac{m_0}{m_f}\right)
$$

$$
m_f=m_0\exp\left(-\frac{\Delta V}{I_{sp}g_0}\right)
$$

$$
m_{erg}=m_0-m_f
$$
