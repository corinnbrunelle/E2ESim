# E2ESim
E2ESim by CSIRO

pour le simulateur, ce n’est pas super user-friendly en ce moment à cause de l’histoire des instructions AVX-512 qui ne sont pas supportées. Il serait probablement mieux de faire un script simple en bash qui contient déjà les commandes, et qu’un usager pourrait simplement modifier selon le besoin. Par exemple, pour lancer la simulation pour le cas exemple (lac Heron) :
 
/home/shared/opt/sde-external-9.33.0-2024-01-07-lin/sde64 -future -- ./aqwafwdsim heron-simA.txt
 
La partie “/home/shared/opt/sde-external-9.33.0-2024-01-07-lin/sde64 -future” utilise Intel SDE pour émuler un processeur qui supporte AVX-512.
La partie « -- ./aqwafwdsim heron-simA.txt » est simplement la commande à émuler.

