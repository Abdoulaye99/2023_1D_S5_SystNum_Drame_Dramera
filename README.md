# 2023_1D_S5_SystNum_Drame_Dramera

    1. Quel est son rôle ?
Le MCP23S17 est un extenseur d’E/S 16 bits qui peut être utilisé pour ajouter des entrées/sorties à un microcontrôleur.

    2. Combien d'entrées/sorties (GPIO) peut-il gérer simultanéments ?
Jusqu'a 16 GPIO simultanément

    3.  Dans notre application, ces GPIO sont-ils configurés en entrée ou en sortie ?
Les GPIO peuvent être configurés en entrée ou en sortie en utilisant les registres IODIRA et IODIRB

    4.  A quelle fréquence maximale peut-on communiquer avec ce composant ?
  10 MHz
    5.  Listes les pin qui sont reliés au micro-controleur et expliciter leur rôle.
    
    6.  Etablir un tableau d'association entre les pins du composant et celle du micro-controleur.
    7.  A quoi servent les pins A0, A1 et A2 ? Qu'est ce que l'opcode ?
    
Les pins A0, A1 et A2 sont des broches d’adresse qui permettent de configurer l’adresse matérielle du composant.
L’opcode est un code d’opération qui est utilisé pour spécifier l’opération à effectuer sur le MCP23S17
    8.  A quoi servent les pins INTA et INTB ?
    
Les pins INTA et INTB sont des broches d’interruption qui sont utilisées pour signaler au microcontrôleur qu’un changement d’état s’est produit sur les GPIO
  
    9.  Quelle doit-être la valeur de sortie d'une pin pour allumer la led ?
    
Pour allumer une LED, la valeur de sortie de la broche doit être 1.

    10.  A quoi servent les résistances R501 à R516 ? Pourquoi ne sont-elles pas toutes de la même valeur ?
    
Les résistances R501 à R516 sont des résistances de pull-up qui sont utilisées pour garantir que les broches d’entrée sont à un niveau logique haut lorsqu’elles ne sont pas connectées à un signal. Les résistances ne sont pas toutes de la même valeur car elles sont dimensionnées pour les broches d’entrée qui ont des exigences de courant différentes
   
    11.  A quoi correspondent ces registres ?
    
Les registres IODIRA et IODIRB sont utilisés pour configurer les ports A et B comme entrées ou sorties. Les registres GPIOA et GPIOB sont utilisés pour lire ou écrire les valeurs des ports A et B.

    12.  Quels valeurs doivent-ils prendre pour que toutes les leds soient éteintes ?
    
il faut configurer les ports A et B en sortie et écrire des zéros dans les registres GPIOA et GPIOB.
    
    13.  Quels valeurs doivent ils prendre pour que toutes les leds soient allumées ?
    
il faut configurer les ports A et B en sortie et écrire des uns dans les registres GPIOA et GPIOB.
   
    14.  Pour que seule la led D508 soit allumée ?
    
Pour que seule la led D508 soit allumée, il faut configurer les ports A et B en sortie et écrire un zéro dans le bit 7 du registre GPIOA et des uns dans tous les autres bits de GPIOA et GPIOB.
