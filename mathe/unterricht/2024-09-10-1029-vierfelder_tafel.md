---
title: 'Vierfeldertafel'
subtitle: 'subtitle'
author: Niklas von Hirschfeld
date: 2024-09-10
toc: true
bib: false
chapter: false
publish: false
environments: []
---

::: leftbar
S. 248
:::

--- 

**Beispiel am Urnenmodell**

In einer Urne sind **10** Kugeln, **5** davon sind Markiert (Ereignis $M$).
Also $P(M)=\frac{5}{10}=50\%$. Es gibt allerding **drei** von **vier** roten Kugeln, welche
Markiert sind und und **zwei** von **sechs** nicht rote Kugeln. Wenn man nun beim ziehen
vorher schon weiß, welche Farbe die Kugel hat, bevor man die Markierung sieht,
verändert sich die Wahrscheinlichkeit auf $\frac{3}{4}=75\%$.

Man bezeichnet die Wahrscheinlichkeit für eine Markierung ($M$) unter der
Bedingung rot ($R$) als **bedingte Wahrscheinlichkeit** und schreibt.

::: inmargin
Das bedingende Ereignis $R$ wird als Index notiert. Man liest $P_R(M)$:
"Wahrscheinlichkeit von $M$ unter der Bedingung $R$"
:::

$$
P_R(M)=\frac{3}{4}=75%
$$


::: block
**Satz:** $P_E(F)$ ist die **bedingte Wahrscheinlichkeit**
:::

# Aufgaben

Eine Münze wird dreimal geworfen. Berechnen Sie $P_E(F)$ und $P_F(E)$.
Beschreiben Sie die gesuchten Wahrscheinlichkeiten in Worten.

::: leftbar
a) E: "Beim zweiten Wurf lag 'Zahl' oben."    F: "Es lag dreimal 'Zahl' oben"
:::

$P_E(F)$ verändert sich zu "Es lag zwei mal Zahl oben", da der Zweite Wurf
bereits Zahl hat. Also ergibt sich die Wahrscheinlichkeit
$P_E(F)=\frac{1}{4}$ anstatt $P(F)=\frac{1}{6}$

$P_F(E)$ da dreimal 'Zahl' oben liegt, dann liegt auch beim zweiten Wurf
'Zahl' oben. Also eine Wahrscheinlichkeit von $P_F(E)=1$

::: leftbar
b) E: "Beim ersten Wurf lag 'Zahl' oben"    F: "Es lag genau einam 'Zahl' oben"
:::

$P_E(F) = \frac{1}{3}$: Möglichkeiten: $100,110,111$ (1: Zahl, 0: nicht Zahl)

$P_F(E) = \frac{1}{3}$: Möglichkeiten: $100,010,001$

::: leftbar
**Was wir wissen müssen**

- Vierfeldertafeln aus und in sachzusammenhänge
- Baumdiagramme hin und her
- Was bedeutet bedingte Wahrscheinlichkeit
- Fachsprache
- Formeln kennen
:::

