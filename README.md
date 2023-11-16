# Connexion entre le logiciel TouchDesigner et le projecteur suspendu au plafond

## Comment faire ?
Brancher le câble (HDMI) lié au projecteur dans l'ordinateur. Ne pas oublier de s'assurer que le projecteur est associé à un port pour permettre sa connexion avec l'ordinateur. Sile projecteur est déjà suspendu au plafond, on ne peut recréer le fameux parcours qui mène à l'adresse IP du projecteur se trouvant dans le menu Réseau. Dans ce cas-là, on peut avoir recours à un outil de suivi des adresses IP, par exemple, *Angry IP Scanner*. 

![image](https://github.com/projet-final-2024/prototypage-camelie/assets/93718179/03b86597-d497-4d9e-84c4-f83fdcf284cd)
> Image provenant du site de *[Angry IP Scanner](https://angryip.org/screenshots/)*

Il s'agit d'essaie-erreur pour trouver l'adresse IP du projecteur souhaité et pour cela il faut transcrire l'adresse IP dans le navigateur web en rentrant dans le message déclenché, le nom d'utilisateur (EPSONWEB) et le mot de passe (admin) par défaut. Ensuite, on va arriver sur une page qui nous présente les différentes sources et choisir celle qui présente l'ordinateur et ainsi observer si un signal est transmis entre les deux ou non. Si c'est le cas, le résultat va ressembler à cela : 

![MicrosoftTeams-image (23)](https://github.com/projet-final-2024/prototypage-camelie/assets/93718179/c0fcd4fe-3bcd-465a-84ef-7a71189d250b)

En poursuivant, on ouvre le fichier que l'on veut projeter dans le logiciel de TouchDesigner et ajoute un composant qui se nomme Window s'il n'est pas déjà présent. Ce dernier inclut le contrôle de nombreux paramètres dont la résolution, le centrage et le(s) moniteur(s) sur lesquels la fenêtre sera affichée. La différence avec le composant Fenêtre et */perform* est que : 

> *Le composant Window vous permet de créer et de maintenir une fenêtre flottante ou fixe distincte affichant le contenu de n'importe quelPanneauou n'importe quelVisionneuse de nœuds*

> Phrase tirée du site de *[TouchDesigner](https://derivative.ca/UserGuide/Window_COMP)*

![image](https://github.com/projet-final-2024/prototypage-camelie/assets/93718179/f3b09f07-43f5-4700-8025-fa3f6cefd126)

La kinect a également été utilisée pour ajouter la détection de présence au visuel réalisé dans TouchDesigner. Elle a été connectée dans l'ordinateur au moyen de son câble (USB). 

## Résulat, est-ce que ça marche ou pas ? 
Ça marche ! 

https://github.com/projet-final-2024/prototypage-camelie/assets/93718179/73b1ab75-5e33-4eb5-89d3-84619d5bf75a
