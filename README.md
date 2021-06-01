# My Blog Api Project

Ma première application serveur en RubyOnRails

## Présentation du projet

L’idée est de réaliser une application simple : un blog avec des articles. Tu pourras faire un CRUD complet pour les articles : création, index, lecture, edit, update, destroy. Le tout sera en API JSON.
## Base de données

La BDD **Postgresql** est composée de deux tables : Users, Articles
 * Un article possède forcément un user
 * Un user peut avoir plusieurs articles
## Versions utilisées 

* Ruby: 2.7.1
* Rails: 6.1.3

## Fonctionnalités

Ce que contient la **version finale** :

* Application Rails 6 en mode API 
* Base de données Postgresql
* Système d’authentification vie devise-jwt : 
  - création et édition d'un article accessible qu'aux utilisateurs connectés
  - fonctionnalités de destroy et d'edit/update accessibles qu'aux propriétaires des articles

## Lancement de l'app

```
git clone https://github.com/carolemny/my_blog_api.git
cd my_blog_api_ror
bundle install
```

**Database**

```
rails db:create
rails db:migrate
rails db:seed
```

**Lancer le serveur**

`rails server`

Puis aller sur : http://localhost:3000/

L'API pourra être testée par le biais d'Insomnia ou Postman. 

## L'équipe

* **Carole Meney** _alias_ [@carolemny](https://github.com/carolemny)