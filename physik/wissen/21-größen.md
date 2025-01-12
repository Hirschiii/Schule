---
title: 'Größen zur Beschreibung einer Welle'
subtitle: 'subtitle'
author: Niklas von Hirschfeld
date: 2024-09-13
toc: true
bib: false
chapter: false
publish: false
environments: []
---

- Zentrale Größen zur Beschreibung einer Welle sind ihre Amplitude $\hat{y}$, ihre Schwingungsdauer $T$, ihre Frequenz $f$ und ihre Phasen- bzw. Ausbreitungsgeschwindigkeit $c$.



::: {.buffer title="Größen anhand der sinus 'Welle'" reference="fig:wellen_beschriftet" }
\startMPpage

u := 1cm;

drawarrow (((-1 * pi) - 1) * u,0)--(((2 * pi) + 1) *u,0);

drawarrow (0,-1.5 * u)--(0,1.5 * u);

draw function (1, "x", "sin(x)", (-1 * pi) - 1, (2 * pi) + 1, .01) scaled u;

label.rt(btex $y$ etex, (0, 1.5 * u));
label.top(btex $x$ etex, (((2 * pi) + 1) * u, 0));

draw (-0.1 * u, 1 * u)--(0.1 * u, 1 * u);
draw (-0.1 * u, -1 * u)--(0.1 * u, -1 * u);

label.rt(btex $1$ etex, (0, 1 * u));
label.rt(btex $-1$ etex, (0, -1 * u));

draw (pi * u,0.1 * u)--(pi * u, -0.1 * u);
draw (2pi * u,0.1 * u)--(2pi * u, -0.1 * u);
draw (-1 * pi * u,0.1 * u)--(-1 * pi * u, -0.1 * u);

label.bot(btex $\pi$ etex, (pi * u, 0));
label.bot(btex $2\pi$ etex, (2 * pi * u, 0));
label.bot(btex $-\pi$ etex, (-1 * pi * u, 0));

% ---------- Groessen ---------- %

% ------------ Wellenlaenge ------------ %

% lambda_left := (0, 0.5 * u);
% lambda_right := (2 * pi * u, 0.5 * u);

draw (0, 0.5 * u)--(2 * pi * u, 0.5 * u) withcolor blue;
draw (0, 0.7 * u)--(0, 0.3 * u) withcolor blue;
draw (2 * pi * u, 0.7 * u)--(2 * pi * u, 0.3 * u) withcolor blue;

label.top(btex $\lambda$ etex, (pi * u, 0.5 * u));

% ------------ Amplitude ------------ %

draw (-0.5 * u, 0)--(-0.5 * u,1 * u) withcolor red;
draw (-0.7 * u, 0)--(-0.3 * u, 0) withcolor red;
draw (-0.7 * u, 1 * u)--(-0.3 * u, 1 * u) withcolor red;

label.lft(btex $\hat{y}$ etex, (-0.5 * u, 0.5 * u));

\stopMPpage
:::

> *Hinweis:* Alle folgenden Definitionen für die Größen von Wellen stammen von Leifi[@LeifiGroesseWellen] 

::: {.definition title="Wellenlänge"} :::
$\lambda$ ist der  x-Abstand eines Teilchens zum nächsten Teilchen im gleichen Schwingungszustand (d.h. die beiden Teilchen müssen die gleiche Auslenkung und die gleiche Geschwindigkeit haben).

**Anmerkung:** Zu Teilchen mit gleichem Schwingungszustand sagt man auch gleichphasig schwingende Teilchen.

::: {.math title="Zusammenhang Größen von Wellen" reference="wellen:groessen" }
\lambda = c \cdot T = \frac{c}{f}
:::

:::::::::::::::::::::::::::::::::::::::::

::: {.definition title="Amplitude"} 
$\hat{y}$ ist die Maximale Auslenkung der
schwingenden Teilchen einer Welle aus ihrer Ruhelage Ruhelage
Gleichgewichtslage. Wir gehen dabei davon aus, dass die Welle ungedämpft ist,
d.h dass alle schwingenden Teilchen die gleiche Amplitude wie das erregende
Teilchen besitzen. 
:::

::: {.definition title="Schwingungsdauer"}
$T$ beschreibt die Zeit, die jedes einzelne Teilchen der harmonischen Welle für
eine volle Schwingung benötigt. Wir gehen dabei davon aus, dass alle
schwingenden Teilchen die gleiche Schwingungsdauer wie das erregende Teilchen
besitzen.
:::

::: {.definition title="Frequenz"}
$f$ stellt die Anzahl der Schwingungsperioden jedes einzelnen Teilchens pro Zeiteinheit dar. Wir gehen dabei davon aus, dass alle schwingenden Teilchen die gleiche Frequenz wie das erregende Teilchen besitzen. Es gilt:
$$
f=\frac{1}{T}
$$
:::

::: {.definition title="Kreisfrequenz"}
$\omega$ ist der Überstrichener Winkel (im Bogenmaß) jedes einzelne Teilchens pro Zeiteinheit. Wir gehen dabei davon aus, dass alle schwingenden Teilchen die gleiche Kreisfrequenz wie das erregende Teilchen besitzen. Es gilt:

$$
\omega = 2 \cdot \pi \cdot f = \frac{2 \cdot \pi}{T}
$$
:::


::: {.definition title="Phasen- oder Ausbreitungsgeschwindigkeit der Welle"}
$c$ beschreibt die Geschwindigkeit, mit der sich die Störung über den Wellenträger ausbreitet. Leicht zu bestimmen ist \(c\), wenn man einen ausgezeichneten Punkt (z.B. den Wellenberg) beobachtet.

**Achtung:** Die Phasengeschwindigkeit ist nicht mit der Geschwindigkeit der von der Welle erfassten Teilchen zu verwechseln.
:::



