# MovieTime

Avant de commencer, lancer :

```bash
composer install
```

## Base de Données

La base de donnée se fait en local avec mySql en utilisant MAMP PRO (libre à vous de choisir l'outil que vous souhaitez)

Elle est composée de 4 tables principales :

- Address
- Category
- Product
- User

ainsi que de 'Doctrine_migration_version'

La connexion à la base se fait dans le '.env' en décommentant la partie nécessaire et en y connectant les infos de la BDD

ici la route principale est locale -> http://127.0.0.1:8000/

Depuis cette route principale on retrouve ensuite :

http://127.0.0.1:8000/connexion

http://127.0.0.1:8000/inscription

qui vont renvoyer vers :

http://127.0.0.1:8000/compte

-> http://127.0.0.1:8000/compte/modifier-mon-mot-de-passe
-> http://127.0.0.1:8000/compte/adresses
-> http://127.0.0.1:8000/compte/ajouter-une-adresse

La page principale est la page des produits :

http://127.0.0.1:8000/nos-produits
Cette page va permettre de retrouver l'ensemble des produits, de pouvoir faire des recherches par filtre et par mot-clé
On peut cliquer sur un produit qui nous renvoi sur sa page ( http://127.0.0.1:8000/produit/id )

Depuis le produit, on peut l'ajouter au panier http://127.0.0.1:8000/mon-panier
-> ajouter une quantité http://127.0.0.1:8000/cart/add/{id}
-> retirer une quantité http://127.0.0.1:8000/cart/remove
-> supprimer le produit http://127.0.0.1:8000/cart/delete/{id}

Easy Admin
Pour une gestion simplifiée on utilise Easy Admin -> http://127.0.0.1:8000/admin
On peut y gérer les utilisateurs, les catégories et les produits
![Capture](https://user-images.githubusercontent.com/37074836/151331728-32a77f44-141d-41ac-bc80-321169849bf5.PNG)
