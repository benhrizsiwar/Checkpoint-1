# question 1 : 
**cat /etc/passwd**
# question 2
**chmod 744 myfile** *propriétaire a la permission de lecture ecriture et exécution et le groupe et les autres ont juste le droit de lecture*
# question 3
*Les variables locales de script bash ne sont pas accessibles dans les autres (même les shell fils)* 
*les variables d'environnements peuvent étre copiées dans chaque shell fils* 
### utiliser une variable : 
**echo** $variable
### pour rendre une variable permanente :
**export** variable="variable"
# question 4 
#!/bin/bash

read -p "Donner un nombre : " nombre 


**if [ "$nombre" -gt 10 ]; then**

  echo "Le nombre est bien supérieur à 10"

  else 

  echo "Le nombre n'est pas exact"

**fi**

--- *on va vérifier si le nombre donné est supérieur à 10*
# question 5
#!/bin/bash

- **echo** "Malgré le prix élevé de 100$, il a dit"

- **echo** '"Bonjour !" au vendeur'

- **echo** "\"Bonjour, est-ce que ce clavier fonctionne bien ?\""

- **echo** '"Évidemment ! On peut tout écrire avec'

- **echo** 'que ce soit des pipe | ou bien des backslash \\!"'

- **echo** '"Même des tildes ~?"'

- **echo** '"Évidemment"'

# question 6
**fg %1**
# question 7
Couche 3: Réseau (PDU: paquet)
Couche 2: Liaison (PDU: trame)
# question 8
| Commande Unix | Équivalent PowerShell               |
|---------------|-------------------------------------|
| cp            | Copy-Item                           |
| cd            | Set-Location                        |
| mkdir         | New-Item -ItemType Directory        |
| ls            | Get-ChildItem                       |

# question 9
**PAYLOAD** est la charge utile qui est envoyée dans la trame, elle contient les données telsque la fréquence, le timestamp ,...
# question 10
Pour simplifier l’écriture des masques de sous réseau, on écrit simplement le nombre de bits à 1 précédé d’un /. 
Le rangement des adresses IP en classe A, B, C, ... est historique. De nos jours, cette classification n'a plus lieu d'être mais la notification CIDR doit être celle à utiliser.
