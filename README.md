# Design Patterns en Java

Ce projet met en pratique plusieurs modèles de conception classiques en Java. Ces design patterns permettent d'améliorer la flexibilité, la maintenabilité et la lisibilité du code.

## Modèles de Conception Implémentés

- Adapter Pattern
- Composite Pattern
- Decorator Pattern
- Observer Pattern
- Proxy Pattern
- Strategy Pattern

---

## Introduction

L'objectif de ce projet est d'explorer et de démontrer l'utilisation des design patterns les plus courants. Chaque pattern répond à une problématique spécifique en termes de création, de structure ou de comportement des objets.

---

## Détails des Patterns

### Adapter Pattern

Permet de rendre compatibles des interfaces incompatibles.

**Principales classes :**
- `MediaPlayer` (Interface cible)
- `AdvancedMediaPlayer` (Interface existante)
- `MediaAdapter` (Adaptateur)
- `AudioPlayer` (Client)

### Composite Pattern

Permet de composer des objets sous forme d'une structure arborescente.

**Principales classes :**
- `Employee` (Interface commune)
- `Developer` & `Manager` (Employés individuels)
- `CompanyDirectory` (Composite)

### Decorator Pattern

Ajoute dynamiquement des fonctionnalités à un objet sans modifier sa structure.

**Principales classes :**
- `Coffee` (Interface de base)
- `SimpleCoffee` (Composant concret)
- `CoffeeDecorator` (Classe abstraite)
- `MilkDecorator`, `SugarDecorator`, `ChocolateDecorator` (Décorateurs concrets)

### Observer Pattern

Met en place une relation un-à-plusieurs entre objets pour notification d'événements.

**Principales classes :**
- `Subject` (Interface sujet)
- `Observer` (Interface observateur)
- `NewsPublisher` (Sujet concret)
- `User` (Observateur concret)

### Proxy Pattern

Fournit un substitut à un objet pour en contrôler l'accès.

**Principales classes :**
- `Image` (Interface)
- `RealImage` (Image réelle)
- `ProxyImage` (Proxy)

### Strategy Pattern

Définit une famille d'algorithmes interchangeables dynamiquement.

**Principales classes :**
- `PaymentStrategy` (Interface stratégie)
- `CreditCardPayment`, `PayPalPayment`, `BitcoinPayment` (Implémentations concrètes)
- `ShoppingCart` (Contexte)

---

## Utilisation

Chaque pattern dispose d'une classe de démonstration permettant de visualiser son fonctionnement :

- `AdapterPatternDemo`
- `CompositePatternDemo`
- `DecoratorPatternDemo`
- `ObserverPatternDemo`
- `ProxyPatternDemo`
- `StrategyPatternDemo`

Lancez simplement ces classes pour observer le comportement des modèles implémentés.

---

## Conclusion

Les design patterns présentés dans ce projet offrent des solutions robustes à des problèmes récurrents en conception logicielle. Leur utilisation contribue à rendre le code plus souple, réutilisable et facile à faire évoluer.

