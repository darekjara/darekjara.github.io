---
layout: post
title: Hide and Seek
categories: [Anna a Elsa, Code.org]
excerpt: Z dnešního snu o Else a Anně se probudil s dobrou náladou. I Rapunzel ve snu radostně usmívala. Zvláštní. Jakoby je všechny zkoušela. Dnes si chtěla hrát na schovávanou.
---

Z dnešního snu o Else a Anně se probudil s dobrou náladou. I Rapunzel ve snu radostně usmívala. Zvláštní. Jakoby je všechny zkoušela. Dnes si chtěla hrát na schovávanou.
 
Nejdříve uviděl Annu a Elsu. Povídaly si o nějaké veselé situaci z předchozího dne. Objevila se Rapunzel a chtěla se přátelit. Elsa se rychle rozloučila a zmizela. Na chvíli. Přijala výzvu ke hře na schovávanou. Jak byla odvážná!

Kdo chytí Annu a Elsu? Ale pozor, na Rapunzel raději neklikej!

| ![](/images/EA-hide-seek.png) |
|:--:| 
| *Úvodní scéna* |

## Script
### Úvodní scéna
Animace úvodní scény je nezvykle dlouhá. Proč? Vytvořit epický děj, kde se postavy k sobě postupně přibližují, mluví spolu, vzdalují se, přichází někdo další, zapojuje se do rozhovoru a zase odchází, vyžaduje dlouhou sekvenci kroků s dobrým načasováním. Jedná se o obdobu scénáře k filmu nebo divadelního skriptu.

| [![](/images/EA-hide-seek-snippet-01.png)][picture1] |
|:--:|
| *Začátek kódu při spuštění* |

Pokračování úvodní scény. V momentě, kdy se postava Rapunzel pohne téměř na konci předchozího algoritmu na dolní okraj scény, začnou se současně hýbat Anna i Elsa. Každá svým směrem. Pokud by sekvence byla součástí předchozího algoritmu, holky by se mohly hýbat teprve jedna po druhé a výsledný dojem by postrádal na dynamičnosti.
Poslední algoritmus tvoří můstek do další části hry. Postavy Anny a Elsy mizí a místo nich se objevují... znovu Anna a Elsa. Ale které? A proč?

Pokračování úvodní scény. V momentě, kdy se postava Rapunzel pohne téměř na konci předchozího algoritmu na dolní okraj scény, začnou se současně hýbat Anna i Elsa. Každá svým směrem. Pokud by sekvence byla součástí úvodního algoritmu, postavy by se hýbaly jedna po druhé a výsledný dojem by postrádal na dynamičnosti.


Prostřednictvím samostatných bloků ``when actor 3 touches`` je zajištěn paralelní pohyb ostatních účinkujících. V tomto případě Anna (``actor1``) a Elsa (``actor2``).

Poslední algoritmus tvoří můstek do další části hry. Postavy Anny a Elsy mizí a místo nich se objevují... znovu Anna a Elsa. Ale které? A proč?

| [![](/images/EA-hide-seek-snippet-02.png)][picture2] |
|:--:|
| *Klíčová zápletka* |

### Pohyb postav
V úvodní scéně se objevují tři postavy. ``actor1`` Anna, ``actor2`` Elsa a ``actor3`` Rapunzel. Jejich pohyb je zakomponován do epického úvodu. Skrytě se ale na scéně objevují i postavy 4 a 5. Teprve když úvodní scéna končí a Anna 1 dojde k levému okraji hrací plochy a zmizí i s Elsou, změní se postavy 4 a 5 z neviditelných na viditelné Annu a Elsu.

Jejich pohyb je automatický, pravidelný a zajišťují jej tyto algoritmy.
Proč výměna postav? Block ``repeat forever do`` je samostatný a běží od začátku hry. Není možné jej vložit do spoštěcího bloku jako je např. ``when actor clicked``. Pokud je třeba, aby se Anna a Elsa hýbaly automaticky neustále dokola a zároveň vstoupily na scénu v jiný okamžik s jiným pohybem, rozdělení postav a střídání algoritmů je vhodná cesta. 

| [![](/images/EA-hide-seek-snippet-03.png)][picture3] |
|:--:|
| *Automatický pohyb postav* |



### Strategie hry: úspěch versus neúspěch
Hra je velmi jednoduchá. Jde o to, trefit se a kliknout na Annu nebo Elsu. Tím získáváš body. Pokud klikneš na Rapunzel, o 5 bodů přijdeš. Hra začíná znova. Dostupné programové bloky neumožňují vynulovat skóre, tedy nastavit jej znovu na 0. Postup s odebráním pěti bodů simuluje vymazání skóre a restart hry.

| [![](/images/EA-hide-seek-snippet-04.png)][picture4] |
|:--:|
| *Hra o skóre* |

## Hra
Hra je úmístěna na [code.org](https://studio.code.org/projects/infinity/rO6N2RFLczVvb1laxglJ-xDG_TnzszC4RnEo3z7kvyw){:target="_blank"}

<!-- Identifiers, in alphabetical order -->
[picture1]: /images/EA-hide-seek-snippet-01.png "Enlarge the picture"
[picture2]: /images/EA-hide-seek-snippet-02.png "Enlarge the picture"
[picture3]: /images/EA-hide-seek-snippet-03.png "Enlarge the picture"
[picture4]: /images/EA-hide-seek-snippet-04.png "Enlarge the picture"