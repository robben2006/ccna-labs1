# ccna-labs1
Identification des adresses MAC et IP

# Packet Tracer - Identification des adresses MAC et IP

## Objectifs
- Comprendre le fonctionnement des PDU en communication locale et distante
- Observer le comportement des adresses MAC et IP à travers les différents équipements (PC, Switch, Hub, Routeur, Access Point)
- Analyser le rôle de chaque équipement dans le traitement des trames

## Topologie
![Topologie](screenshotstopologie.png)

## Partie 1 – Communication réseau local (172.16.31.5 → 172.16.31.2)

### Tableau des PDU

 Sur le périphérique  Dest. MAC        MAC src          IPv4 src       IPv4 dest     
-------------------------------------------------------------------------------------
 172.16.31.5          000C85CC1DA7   00D0D311C788   172.16.31.5    172.16.31.2   
 Commutateur 1        000C85CC1DA7   00D0D311C788   SO            SO           
 Concentrateur        SO              SO              SO            SO           
 172.16.31.2          00D0D311C788   000C85CC1DA7   172.16.31.2    172.16.31.5   

## Partie 2 – Communication réseau distant (172.16.31.5 → 10.10.10.2)

### Tableau des PDU

 Sur le périphérique  Dest. MAC        MAC src          IPv4 src       IPv4 dest     
-------------------------------------------------------------------------------------
 172.16.31.5          00D0BA8E741A   00D0D311C788   172.16.31.5    10.10.10.2    
 Commutateur 1        00D0BA8E741A   00D0D311C788   SO            SO           
 Routeur              00602F844AB6   00D0588C2401   172.16.31.5    10.10.10.2    
 ...                  ...              ...              ...            ...           

## Questions de réflexion (réponses)

1. ...
2. ...
...
(ajoute tes réponses ici)

## Ce que j’ai appris
- Les adresses MAC changent à chaque saut de couche 2 (notamment au niveau du routeur)
- Le concentrateur et le point d’accès n’utilisent pas les adresses MAC de la même façon
- Le routeur est le point où les adresses MAC sourcedestination sont modifiées lors d’une communication inter-réseaux

