# Switch_Conf
Configuration du switch hébergeant les différents VLANs


📄 Description
Ce dépôt contient la configuration complète d'un switch Cisco utilisée dans le cadre de la préparation à l'examen du BTS SIO option SISR. Ce fichier a pour but de documenter les paramétrages réseau mis en œuvre, notamment au niveau des VLANs, des interfaces, du mode trunk, etc.

🧰 Matériel utilisé
Modèle de switch : Cisco Catalyst WS-C2960X-24TD-L

Version IOS : 15.0

⚙️ Configuration réseau
🔐 Sécurité et services
Désactivation du service pad

Timestamps activés pour logs et débogages

HTTPS activé (ip http secure-server)

Pas de chiffrement des mots de passe (à activer en production)

🏷️ VLANs utilisés
VLAN	Description
1	VLAN par défaut
10	Réseau administratif
20	Réseau technique
30	Réseau utilisateurs

🔌 Interfaces configurées
Trunk
GigabitEthernet1/0/1 : trunk autorisant les VLANs 1,10,20,30

Access
Interface	VLAN assigné
Gig1/0/2 à 1/0/4	VLAN 20
Gig1/0/5 à 1/0/12	VLAN 10
Gig1/0/13 à 1/0/24	VLAN 30
