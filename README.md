# solidity-smart-contract
Caussanel Vallet
Charge à vous, de définir le jeton/token que vous souhaitez implémenter.
- Quelle sera sa valeur ? 
- Qui l'émettra ? En quelle quantité ? Sera-t-il possible d'un créer de nouveaux ? D'en détruire ?

 Les token modélisent des points de fidélité, un facteur est donc renseigné par le magasin dans un sens pour donner le nombre de points à attribuer en fonction du prix(fonction AddPoints),dans un autre pour calculer la remise obtenue en fonction du nombre de Points que le client souhaite utiliser (fonction UsePoints). C'est le commerçant qui génère les token et peut les detruire, dans une quantité adaptée aux nombres de clients évidemment et de leurs achats,ainsi que du facteur choisi pour l'attribution.Lorsque les points sont utilisés ils retournent dans le wallet du magasin et le cycle recommence.

 Faudra-t-il être authentifié pour en posséder ? pour en transmettre ? Si oui, par qui ?
 
 Les fonctions transfer et transferfrom du standard erc20 qui permettent l'échange de points entre clients si l'opération est validée par le magasin et qui sont utilisées dans les fonctions add et use points qui ne sont accessibles que par le commerçant.
