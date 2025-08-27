


![Message consommé par le worker](img/img1.png)

Comportement asynchrone des messages ! La BDD va stocker jusqu'à ce que le worker prenne en charge les messages. ![](img/bus.png)

Au minimum 2 applications, une qui va stocker les messages, l'autre qui va les recevoir. Un adaptateur qui va stocker les message le temps qu'il y a ai un consommateur pour le consommer.



