###
# Linear Regression
## Inteligență Artificială - Tema 2

Testările au fost realizate pentru ambele seturi de date. Primul set de date simple prezintă puncte 
mai dezordonate, în timp ce setul de date complex prezintă date care fac trimitere la o
sinusoidă.

Pe cele două cazuri descrise, se pare că forma închisă liniară este mai performantă decât forma liniară
        polinomială. Pentru cea din urmă am ales gradul 7, inductiv iterând și găsind valoarea aparent cea
        mai potrivită. Diferența în modul dintre seturile de date de antrenare/testare se poate remarca la
        setul complex, aici forma închisă liniară dovedindu-și eficacitatea.
    
Pentru gradient descent, w tinde la valoarea lui ideala rapid pentru ambele seturi de date. 
    
In Stochastic Gradient Descent, unde batch-ul este de dimensiune 1, w ajunge aproape instant aproape de valoarea lui ideala, dar oscileaza in jurul varfului parabolei (descrise și în enunțul temei). 
    
Pentru Gradient descent cu batch de dimensiune 64, se observa cum w tinde foarte repede la valoarea lui ideala.

 Pentru learning rates mai mari, algoritmul gaseste mai repede un cost optim, dar nu e garantat ca va fi cel mai bun. In antiteza, Pentru learning rates mici (1e-5), algoritmul dureaza mai mult, dar are rezultate mai bune.

 Aceste seturi de date cel mai probabil pot fi considerate "mici", deoarece Gradient Descent aplicat pe exclusiv toate seturile
    de date, ajunge la o concluzie într-un timp relativ foarte rapid. Pe seturi de date mult mai mari, rentabilitatea acestuia scade
    și aici iese în lumină mult mai mult eficacitatea algoritmilor Mini-Batch Gradient Descent sau Stochastic Gradient Descent.
    
