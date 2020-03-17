---
layout: post
title: Seeking the right Elsa
categories: [Anna a Elsa, Coding]
excerpt: Opět snil sen o Else a Anně. Elsa se objevila uprostřed louky. Byla v dobré náladě. Obrátila se na něj a pozdravila ho. Dnes jí to neobyčejně slušelo. Náhle se na kraji louky objevila zlá Rapunzel.
---
Opět snil sen o Else a Anně. Elsa se objevila uprostřed louky. Byla v dobré náladě. Obrátila se na něj a pozdravila ho. Dnes jí to neobyčejně slušelo. Náhle se na kraji louky objevila zlá Rapunzel. Projel jím záblesk obavy. I Elsa se poděsila. Rapunzel se k ní rychle přiblížila. Vyslovila nějaké kouzlo a kolem se rozletěly kusy ledu. Proměnila Elsu v Rapunzel. V ten moment se na zahradě objevily dvě další postavy Rapunzel. Celá zahrada se zatočila. Rapunzel změnily podobu na Elsu. Na zahradě stály čtyři Elsy. Ale která byla ta pravá?

Ještě štěstí, že v ten moment přišla na zahradu i Anna. Teď je na ní, poznat tu pravou. Cítí ve snu, že je to on, kdo má Annu vést. Rozbušilo se mu srdce. Cítil, že stačí jediná chyba, jediný krok špatným směrem a Elsa i Anna budou na věky ztraceny. 

![](/images/EA-seeking-Elsa.png)
## Script
### Úvodní scéna
Hra se skládá ze tří logických částí. 

První sada bloků vytváří animaci úvodní scény. V této části slouží kód k vytvoření příběhu.

Důvod rozdělení úvodní scény do samostatných bloků je kvůli načasování pohybu postav. Šlo by spojit bloky do jednoho nebo naopak rozložit do více. Cílem je vyvolat dojem až filmového ztvárnění. Postavy se pohybují a mění podobu současně. Čím více bude kód rozdělen, tím více se mohou postavy pohybovat současně. Kód je totiž v každém bloku vykonáván postupně od začátku do konce. Pokud chci, aby se nějaký kód odehrál současně, tedy paralelně, musím ho umístit do samostatného bloku.

| ![](/images/EA-seeking-Elsa-snippet-01.png) |
|:--:|
| *Úvodní scéna*|

### Ovládání Anny
Pro ovládání pohybu Anny slouží jednoduchý kód pohybu do všech stran pomocí kláves.

| ![](/images/EA-seeking-Elsa-snippet-02.png) |
|:--:| 
| *Ovládání Anny* |


### Úspěch vs neúspěch
Jen jedna postava Elsy je ta pravá. Je to ta, označená jako Actor 3. Pokud se k ní Anna přiblíží, spustí se vítězný kód. Ostatní tři možnosti obsahují stejný algoritmus.


| ![](/images/EA-seeking-Elsa-snippet-03.png) |
|:--:|
|*Bodovací script*|


## Hra
Hra je úmístěna na [code.org](https://studio.code.org/projects/infinity/6UH8xTUqiryUleUV58KA6LMebJVi_rApGhJ3RHLwSXM){:target="_blank"}