Groupe :

BERARD Lucas
DE MASFRAND Guillaume
DUFRENE Mélic
GILG Thibault
PUISSANT Fabien

Nous fait une application web gérant des cartes.
Une architecture full Rest à été adoptée (voir image CardMarket). Ceci nous permet de séparer les services gérant
les utilisateurs et les cartes pour des raisons de maintenabilité et clareté. 

Nous avons donc deux entités : User et Card ainsi qu'un modèle CardFactory qui va permettre de creer de nouvelles cartes
User et Card sont liés à leur repository et service respectifs

Nous avons aussi 3 RestControllers, un gérant les utilisateurs, l'autre les cartes et enfin le troisième va gérer le marché
des cartes car il va utiliser à la fois le service User et le service Card.

Une fois l'application lancée, il faut se creer un compte utilisateur via la page de d'inscription puis une fois ceci fait, 
5 cartes aléatoires sont créées pour l'utilisateur. Il peut maintenant se connecter pour acceder au marché.
Une fois connecté, l'utilisateur est redirigé vers la page principale où il peut acheter ou vendre ses cartes.
Nous avons ajouté une fonctionnalité qui permet de creer des cartes aléatoire contre de l'argent.
Un soin particulié à été porté à l'expérience utilisateur notamment via l'utilisation de toast (messages popup informatifs) et 
de la fluidité de l'application : rechargement de la carte selectionnée lorqu'on la vend ou achète sans rechargement de page.
Toutes les fonctionnalités sont terminées et il manque simplement un systeme de lazy load des cartes afin que toutes les cartes 
ne soient pas afficher d'un seul coup. En effet il faudrait les faire apparaître au fur et à mesure du scroll de la page.


Page de d'inscription : /addUser.html
Page de connexion : /login.html
Page principale : /card.html ("impossible" d'y acceder sans se connecter)


Source du projet : https://github.com/fabienpuissant/ASI_Atelier2

