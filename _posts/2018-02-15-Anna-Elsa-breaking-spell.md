---
layout: post
title: Anna a Elsa breaking the spell
categories: [Anna a Elsa, Code.org]
excerpt: Noc byla zase studená. Vsnil se do ledového království. Měl dojem, že Rapunzel mluví k němu mrazivě ledovým hlasem. Otřásl se strachem.
---

Noc byla zase studená. Vsnil se do ledového království. Měl dojem, že Rapunzel mluví k němu mrazivě ledovým hlasem. Otřásl se strachem. Zazněl smích. To se objevily veselá Anna a Elsa. Nebyl součástí scény, Rapunzel ho neviděla. Vyzývala Annu a Elsu k přátelství. Odmítly. Nevěřily jí. Stejně jako on. Rapunzel se rozčílila a pronesla zaklínadlo. Náhle se Anna a Elsa proměnily v Rapunzel. A přibyly další dvě. Co teď? Pochopil, že přece jenom je součástí snového dění. Jeho úkolem je osvobodit pravou Annu a Elsu.

Ale která to je? Dlouho je bedlivě pozoroval, až si všiml něčeho zvláštního v jejich pohybu. To musí být ony!

Nebo ne?


| ![](/images/EA-breaking-spell.png) |
|:--:| 
| *Prostředí hry* |

## Script
### Úvodní scéna
Začátek je opět lehce epický. Animací se představí hlavní aktérky. Proběhne krátký rozhovor, který vyústí v kouzlo Rapunzel. 


| [![](/images/EA-breaking-spell-snippet-01.png)][picture1] |
|:--:| 
| *Uvedení postav na scénu* |

Jakmile se Rapunzel dostane k dolnímu okraji scény, zmizí a objeví se čtyři nové postavy. Dvě jsou zakleté Anna a Elsa a ostatní dvě jsou pravé Rapunzel. Úkolem je poznat začarované holky Annu a Elsu.

| [![](/images/EA-breaking-spell-snippet-02.png)][picture2] |
|:--:| 
| *Proměna postav* |

### Pohyb postav
Postavy se hýbou po scéně automaticky. Anna a Elsa dostávají do svého pohybu trochu náhodnosti skrze paralelní kód. Ten vychýlí jejich pohyb náhodným směrem po náhodně zvoleném časovém okamžiku. Souběžně probíhá opakovaný pohyb doprava, doleva, nahoru, dolů.

Náhodný prvek v pohybu znesnadňuje odhadnutí, která postava je která. Zvláště když se změna pohybu odehraje v okamžiku, kdy postava není vidět. 

Kdy není postava vidět? Dočteš se níže ve strategii hry.

| [![](/images/EA-breaking-spell-snippet-03.png)][picture3] |
|:--:| 
| *Algoritmy pohybu postav* |

### Strategie hry: úspěch versus neúspěch
Kliknutí na pravou Annu a Elsu vede ke zvýšení skóre. Kliknutí na Rapunzel snižuje skóre.

Po kliknutí zmizí na náhodně zvolený okamžik postava, na kterou jsi klikl. Aby situace nebyla tak jednoduchá, po kliknutí na skutečnou Annu a Elsu se na náhodný okamžik skryje i jedna z Rapunzel. Jakmile se objeví, je těžší určit, která je Rapunzel a kdo je pravá Anna a Elsa.

Malou pomoc nabízí pohyb postav. Kód, který znáhodňuje pohyb Anny a Elsy zároveň slouží jako vodítko pro jejich rozpoznání. Pozoruj a všimni si trhaných změn pohybu u dvou postav Rapunzel.

>Tip: tento trik s pozorováním pohybu postav vznikl "objevem" až po vytvoření skriptu. Původně šlo o to, vnést do pohybu náhodnost a znesnadnit tak rozpoznání postav. Zajímavé je, jak se každý záměr může obrátit snadno ve svůj opak nebo jak může fungovat jinak, než byl zamýšlen. A takto je to se vším, nejenom s kódováním. Obojí funguje: pokud budeš dobře pozorovat okolí, odhalíš triky, které na tebe někdo nachystal a naopak můžeš díky tomu dostat do pasti svého protivníka. Dobře pozoruj.

## Hra
Hra je úmístěna na [code.org](https://studio.code.org/projects/infinity/wVPmu1A3P0H42361kpqMe6oms65Qq-yUOgXTzh1OcZo){:target="_blank"}

<!-- Identifiers, in alphabetical order -->
[picture1]: /images/EA-breaking-spell-snippet-01.png "Enlarge the picture"
[picture2]: /images/EA-breaking-spell-snippet-02.png "Enlarge the picture"
[picture3]: /images/EA-breaking-spell-snippet-03.png "Enlarge the picture"