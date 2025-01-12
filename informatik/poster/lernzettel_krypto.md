---
title: 'Lernzettel - Kryptographie'
institute: 'Gymnasium Lüneburger Heide'
author: Niklas von Hirschfeld
date: 2024-10-01
toc: true
publish: false
---

```{=context}
\definestartstop
  [exdent]
  [before={\startnarrower[left]\setupindenting[-\leftskip,yes]},
   after=\stopnarrower]
```

<!--
- Begriffe
    - Mono
    - Poly
    - Sub
    - Trans
- Verfahren
    - RSA
    - Ceaser
    - Vigener
-->

# Begriffe

```{=context}
\startexdent
```

**Kodierung** beschreibt den Prozess der Umwandlung von Daten in ein anderes
Format, welches zur Datenübertragung, Datenkompression und Fehlererkennung
verwendet werden kann.

**Kryptographie** beschreibt hingegen die Verschlüsselung von Daten. Ihre
Hauptziele sind Vertraulichkeit, Integrität und Authentizität. Dies bedeutet, dass
Informationen so verschlüsselt werden, dass sie nur von berechtigten Personen
gelesen werden können, ihre Unversehrtheit garantiert wird oder die Identität des
Absenders bestätigt werden kann.

**Substitution** (von lat. *substituere = „ersetzen“*) bezeichnet in der
Kryptographie eine der beiden grundlegenden Ideen der Verschlüsselung. Dabei
werden die Zeichen nach einen System **ersetzt**.

**Transposition** (von lat. *transponere = „versetzen“*) beschreibt das andere
grundelegende Verfahren. Dabei werden die Zeichen lediglich **umsortiert**.
Nach der Transposition bleiben *alle* Zeichen erhalten.

**Monoalphabetische** Substitution bezeichnet ein Verfahren in dem jedes
Zeichen durch ein einzigartiges, ersetzt wird. Es wird also zum Beispiel
**nur** jedes Zeichen $A$ durch das Zeichen $B$ ersetzt und kein anderes.

**Polyalphabetisch** Substitution kann, im gegensatz zu dem *monoalphabetischen
Substitutionsverfahren*, ein Zeichen $A$ durch mehrer andere Zeichen ersetzen.

**Symmetrische Verfahren** solche Verfahren verwenden zum ver- wie auch
entschlüsseln den *selben Schlüssel*.

**Assymmetrische Verfahren** solche Verfahren nutzen *unterschiedliche
Schlüssel* für die ver- und entschlüsselung.

```{=context}
\stopexdent
```

\column

# Verfahren

## Caesar

Der **Caesercode** (auch Caeser-Verschlüsselung oder -Verschiebung) ist ein
*symmetrisches* Verschlüsselungsverfahren, welches nach Julius Caesar
benannt ist. Dieser habe es für die Kommunikation mit seinen militärischen
Verbündeten genutzt. Nachrichten mussten über lange Distanzen transportiert
werden. Dabei passierte es nicht selten, dass solche Nachrichten abgefangen
wurden. Damit dabei keine vertraulichen Informationen an den *Gegner* gerieten,
wurde die Caeser-Verschlüsselung genutzt.

## Vigener

Das **Vigenère-Verfahren** ist ein *symmetrisches* Verschlüsselungsverfahren,
das im 16. Jahrhundert von Blaise de Vigenère entwickelt wurde. Es gilt als
eine Weiterentwicklung der einfachen Caesar-Verschlüsselung und wurde über
Jahrhunderte als eine der sichersten Methoden zur Verschlüsselung von Texten
angesehen. Anders als beim Caesar-Code wird hier ein **Schlüsselwort**
verwendet, um den Text zu verschlüsseln.

## RSA
