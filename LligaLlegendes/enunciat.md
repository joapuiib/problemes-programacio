### Exercici 11: LligaDeLesLlegendes
* Relitza aquest exercici en el subpackage extraordinaria.uf4.llegendes
Es vol realitzar un joc simple anomenat "Lliga de les Llegendes". Aquest joc conté 3 tipus de personatges.

Tots els personatges tenen les següents característiques:
- Vida: Punts de salut del nostre personatge. Aquests punts no poden ser inferiors a 0.
- Atac: Punts d'atac del nostre personatge. S'utilitzarà per inflingir danys al rival.
- Defensa: Punts de defensa del nostre personatge. S'utilitzarà per protegir-se d'atacs rivals.

A més tindran les següents accions:
- Attack getAttack(): Retornarà l'objecte Attack del nostre personantge. Cada Attack consisteix en:
  - danyBasic: Dany que rebrà el rival.
  - danyPercentual: Dany que rebrà el rival en relació a la vida restant. 
- recieveAttack(Attack): El personatge rebrà un atack i actualitzarà els punts de salut del personatge.

Per exemple, si un personatge amb 100 de vida i 10 de defensta reb un atack de 20 de dany bàsic i 0.1 de dany percentual, rebrà:
- dany = [ 20 (basic) + 0.1 (percentual) * 100 (vida) ] - 10 (defensa) = (20 + 10) - 10 = 30 - 10 = 20

El personatge quedarà amb 80 de punts de salut. Si la defensa és superior als danys causats, el personatge no rebrà danys.

Els personatges tenen les següents característiques:
- Tirador:
  - Attack: {basic=50 + el atac del personantge, percentual=0.2}
- Assasí:
  - Attack: {basic=100 + el atac del personantge, percentual=0}
- Tanque:
  - Attack: {basic=el atac del personantge, percentual=0}
