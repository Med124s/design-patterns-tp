Modèles de Conception en Java
Ce projet illustre l'application de plusieurs design patterns classiques en Java. Les modèles couverts sont les suivants :

Adapter Pattern

Composite Pattern

Decorator Pattern

Observer Pattern

Proxy Pattern

Strategy Pattern

Table des matières
Introduction

Modèles de conception implémentés

Adapter Pattern

Composite Pattern

Decorator Pattern

Observer Pattern

Proxy Pattern

Strategy Pattern

Utilisation

Conclusion

Introduction
L’objectif de ce projet est de présenter l’implémentation pratique de plusieurs modèles de conception largement utilisés en génie logiciel. Ces patterns permettent de répondre à des problématiques courantes en matière de création, de structuration et de comportement des objets dans une application. Les modèles suivants sont implémentés :

Adapter Pattern : Facilite la compatibilité entre des interfaces qui ne sont pas conçues pour fonctionner ensemble.

Composite Pattern : Permet de traiter de manière uniforme des objets individuels et des compositions d'objets.

Decorator Pattern : Ajoute dynamiquement des fonctionnalités à un objet sans altérer sa structure d’origine.

Observer Pattern : Met en place un mécanisme de notification entre un sujet et plusieurs observateurs en cas de changement d’état.

Proxy Pattern : Fournit un substitut à un objet afin de contrôler son accès.

Strategy Pattern : Définit plusieurs algorithmes interchangeables selon les besoins.

Modèles de conception implémentés
Adapter Pattern
Ce pattern permet à des interfaces incompatibles de collaborer. Ici, la classe AudioPlayer est capable de lire différents formats de fichiers (MP3, MP4, VLC) grâce à un adaptateur.

Principales classes :

MediaPlayer (Interface cible)

AdvancedMediaPlayer (Classe existante avec une interface différente)

MediaAdapter (Adaptateur reliant les interfaces)

AudioPlayer (Client utilisant l’adaptateur)

Composite Pattern
Le Composite Pattern est utilisé pour structurer des objets sous forme d'arbres hiérarchiques, permettant de traiter de façon uniforme objets simples et composites. Dans cet exemple, CompanyDirectory regroupe différents types d’employés.

Principales classes :

Employee (Interface commune)

Developer et Manager (Employés individuels)

CompanyDirectory (Classe composite)

Decorator Pattern
Ce pattern permet d’enrichir un objet en y ajoutant de nouvelles responsabilités de manière dynamique. L’exemple utilisé consiste à personnaliser un café en y ajoutant du lait, du sucre ou du chocolat.

Principales classes :

Coffee (Interface de base)

SimpleCoffee (Composant concret)

CoffeeDecorator (Classe abstraite pour les décorateurs)

MilkDecorator, SugarDecorator, ChocolateDecorator (Décorateurs concrets)

Observer Pattern
Le Observer Pattern établit une relation de type un-à-plusieurs où un objet sujet informe ses observateurs de tout changement d’état. Ici, un éditeur de nouvelles notifie ses utilisateurs.

Principales classes :

Subject (Interface du sujet observé)

Observer (Interface des observateurs)

NewsPublisher (Sujet concret)

User (Observateur concret)

Proxy Pattern
Ce modèle fournit un objet proxy pour contrôler l'accès à un autre objet. Dans notre cas, ProxyImage gère l’accès à une image réelle, en retardant son chargement jusqu'à ce qu'il soit nécessaire.

Principales classes :

Image (Interface pour l'affichage)

RealImage (Classe concrète pour l'image réelle)

ProxyImage (Proxy contrôlant l'accès)

Strategy Pattern
Le Strategy Pattern permet de définir une famille d’algorithmes et de les rendre interchangeables selon le contexte. L’exemple présenté utilise différentes méthodes de paiement dans un panier d’achat.

Principales classes :

PaymentStrategy (Interface pour les stratégies de paiement)

CreditCardPayment, PayPalPayment, BitcoinPayment (Implémentations concrètes)

ShoppingCart (Contexte utilisant une stratégie)

Utilisation
Pour tester les différents patterns, il suffit d'exécuter la classe de démonstration correspondante :

AdapterPatternDemo : Utilisation d'un lecteur audio avec plusieurs formats.

CompositePatternDemo : Organisation hiérarchique des employés.

DecoratorPatternDemo : Ajout dynamique d’ingrédients à un café.

ObserverPatternDemo : Notifications des utilisateurs par un éditeur de nouvelles.

ProxyPatternDemo : Gestion différée du chargement d’une image.

StrategyPatternDemo : Paiement flexible via différentes stratégies.

Conclusion
Ce projet met en évidence la puissance des design patterns pour structurer et améliorer la qualité du code. Leur utilisation permet de rendre le logiciel plus flexible, modulaire et facile à maintenir, tout en offrant des solutions éprouvées à des problèmes récurrents en développement logiciel.