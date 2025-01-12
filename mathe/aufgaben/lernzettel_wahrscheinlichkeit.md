---
title: 'Lernzettel - Stochastic'
subtitle: 'subtitle'
author: Niklas von Hirschfeld
date: 2024-10-02
toc: false
bib: false
chapter: false
publish: false
titlepage: ""
environments: []
---

```{=context}
\setuppagenumbering[location=]

\setuplayout[
   topspace=0.5cm, % Top margin
   header=0.5cm, % Header size
]

\setuphead[chapter]
          [
            before={},
            after={},
          ]

\definestartstop
[exdent]
[before={\startnarrower[left]\setupindenting[-\leftskip,yes]},
after=\stopnarrower]
```

# Lernzettel - Stochastic


## Wahrscheinlichkeiten


```{=context}
\startexdent
```

::: inmargin
*Zuffalsexperiments:* Ziehen, mit Zurücklegen, von zwei Kugeln aus einer Urne mit fünf roten und drei blauen Kugeln.

*Ergebnismenge:* $S=\{rr; rb; br; bb\}$.

Das *Ereignis* $E = \{rr; rb; br\}$ bedeutet, dass mindestens eine Kugel rot ist. Das *Gegenereignis* von $E$ ist $\overline{E}$
:::


Die **Wahrscheinlichkeiten** aller Ergebnisse eines Zuffalsexperiments sind
Zahlen im interval $\[0; 1\]$ mit Summe $1$. Sie bilden die
*Wahrscheinlichkeitsverteilung*. Die Ergebnisse fässt man in der
**Ergebnismenge** zusammen, eine *Teilmenge* davon ist ein **Ergebnis**.

::: inmargin
Als **fair** bezeichnet man ein Spiel, bei dem der Erwartungswert für den Gewinn
null ist. Gewinn = Auszahlung - Einsatz
:::

```{=context}
\stopexdent
```

::: block
**Definition:** Wenn jedem Ergebnis eines Zufallsexperiments ein Zahlenwert
zugeordnet wird, spricht man von einer **Zufallsgröße**. Die
**Wahrscheinlichkeitsverteilung** ener Zufallsrgöße $X$ ist eine Tabelle, bei
der jedem Wert $k$ von $X$ die Wahrscheinlichkeit $P(X=k)$ zugeordnet ist. Für
eine Zufallsgröße $X$ mit den Werten $x_1,x_2, ..., x_n$ heißt $\mu = x_1 \cdot
P(X=x_1) + x_2 \cdot P(X = x_2)... + x_n \cdot P(X = x_n)$ **Erwartungswert**
von $X$. Er gibt an, welchen Mittelwert man bei ausreichend großer
Versuchsanzahl auf lange Sicht erwartet.
:::

## Zufallsgrößen

| Begriff            | Zeichen / Formel                                                            | Beschreibung                                           |
| ---                | ---                                                                         | ---                                                    |
| Varianz            | $V=(x_1-\mu)^2\cdot P(X=x_1)+... +(x_n-\mu)^2\cdot P(X=x_n)$                | Ein Maß für die Streuung                               |
| Standardabweichung | $\sigma = \sqrt{V}$                                                         | Abweichung der Werte von dem eigenen Durchschnittswert |
| Erwartungswert     | $\mu = x_1 \cdot P(X=x_1) + x_2 \cdot P(X = x_2)... + x_n \cdot P(X = x_n)$ |                                                        |

## Bedingte Wahrscheinlichkeiten

**Beispiel am Urnenmodell**

In einer Urne sind **10** Kugeln, **5** davon sind Markiert (Ereignis $M$).
Also $P(M)=\frac{5}{10}=50\%$. Es gibt allerding **drei** von **vier** roten Kugeln, welche
Markiert sind und und **zwei** von **sechs** nicht rote Kugeln. Wenn man nun beim ziehen
vorher schon weiß, welche Farbe die Kugel hat, bevor man die Markierung sieht,
verändert sich die Wahrscheinlichkeit auf $\frac{3}{4}=75\%$.

::: inmargin
Das bedingende Ereignis $R$ wird als Index notiert. Man liest $P_R(M)$:
"Wahrscheinlichkeit von $M$ unter der Bedingung $R$"
:::

Man bezeichnet die Wahrscheinlichkeit für eine Markierung ($M$) unter der
Bedingung rot ($R$) als **bedingte Wahrscheinlichkeit** und schreibt.

