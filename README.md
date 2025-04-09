# SANTANDER API

## DIAGRAM CLASS 


```mermaid
classDiagram
  class User {
    +String name
    +Account account
    +Card card
    +Feature[] features
    +News[] news
  }

  class Account {
    +String number
    +String agency
    +String balance
    +String limit
  }

  class Card {
    +String number
    +String limit
  }

  class Feature {
    +String icon
    +String description
  }

  class News {
    +String icon
    +String description
  }

  User --> Account
  User --> Card
  User --> Feature
  User --> News
