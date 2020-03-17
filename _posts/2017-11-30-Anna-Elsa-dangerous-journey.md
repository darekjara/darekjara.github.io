---
layout: post
title: Dangerous journey
categories: [Anna a Elsa, Coding]
excerpt: V pokoji bylo chladno. Přetáhl si deku k bradě. Usnul. Vstoupil do snění o Else a Anně. Byl Annou. Všude kolem led a chlad. Nebyl zde sám. Byla zde i Rapunzel. Slídila po něm. Ne jedna. Rovnou dvě. Mizely a zase se objevovaly. Tušil, že tam někde na druhém konci té ledové plochy na něj čeká Elsa.
---
V pokoji bylo chladno. Přetáhl si deku k bradě. Usnul. Vstoupil do snění o Else a Anně. Byl Annou. Všude kolem led a chlad. Nebyl zde sám. Byla zde i Rapunzel. Slídila po něm. Ne jedna. Rovnou dvě. Mizely a zase se objevovaly. Tušil, že tam někde na druhém konci té ledové plochy na něj čeká Elsa. Potřebuje otevřít bránu. Ukázat cestu přes ledovou pláň. Věděl, že se musí vyhnout zlé Rapunzel a přivést Elsu do bezpečí. Podaří se mu to?
![](/images/EA-dangerous-journey.png)
## Script
### Úvodní scéna
Na dolním okraji scény se objeví Anna. Rapunzel v horní a střední části.

![](/images/EA-dangerous-journey-snippet-01.png)
### Ovládání postav
Kód pro pohyb a mizení obou postav Rapunzel má stejnou podobu. Rozdíl způsobuje náhodná doba mezi jejich pohybem tam a zpět a jejich mizením a opětovným objevením. Tato náhodnost vnáší do hry prvek nepředvídatelnosti. 


![](/images/EA-dangerous-journey-snippet-02.png)

*Pohyb a mizení Rapunzel*

![](/images/EA-dangerous-journey-snippet-03.png)

*Ovládání Anny*

### Úspěch versus neúspěch
Pokud Anna dojde k hornímu okraji, objeví se Elsa a putuje dolů. Poté se navýší skóre a Elsa se skrytě vrací zpátky k hornímu okraji. Dokud neproběhne celá sekvence kódu, nelze Elsu znovu přivolat. Nestačí tedy nechat Annu u horního okraje a čekat na navyšování skóre. Navíc se zvyšuje riziko, že se objeví Rapunzel... Anna se tedy musí hýbat.

![](/images/EA-dangerous-journey-snippet-04.png)

Jakmile se Rapunzel přiblíží k Anně, skóre se snižuje. Jediné bezpečné místo je pro Annu spodní okraj hrací plochy.

![](/images/EA-dangerous-journey-snippet-05.png)
