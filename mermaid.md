# Mermaid Markdown Diagrams

- [Mermaid on GitHub](https://github.com/mermaid-js/mermaid#readme) 
- [Mermaid docs page](https://mermaid.js.org/intro/)

> _To preview the charts in VS Code you need the extension Markdown Preview Mermaid Support_

## Syntax and examples

Use `mermaid` as the code block language

    ```mermaid
    <!-- code here -->
    ```

Keywords and syntax

1. `TD`, `LR`
1. `%%{``}%%` - for comments
1. `-->`
1. `->>`
1. `-->>`
1. `:`
1. `()`
1. `[]`
1. `{}`
1. `[*]`
1. Diagram Types: graph, gantt, classDiagram, gitGraph, erDiagram, journey, quadrantChart, sequenceDiagram, stateDiagram-v2, pie, requirementDiagram, C4Context, mindmap, timeline, zenuml, sankey-beta, 
1. `end`, participant, loop, Note, right of, dateFormat, title, section, state, as, excludes, click, style, fill, subgraph, class, autonumber, activate, deactivate, 
1. `}|..|{`, `||--o{`, `||--|{`, `[(Database)]`, `((This is the text in the circle))`
1. node-name(Your Text Here)
1. `click` nodename "href"

## Flowchart example

```mermaid
flowchart

    subgraph Nodes
        node-one(Label 1)

        node-two((Label 2))
        node-three([Label 3])
        node-four{Label 4}
        node-five{{Label 5}}
        style node-five fill:green

        node-one-->node-two
        node-two-->node-three
        node-three-->|No|node-four
        node-three-->|Yes|node-five
    end

    subgraph Fruit
        grape[Grapes]
        apple(Apples)

        grape-->apple
    end

    Nodes-->Fruit

```

- `-->` - used to connect 2 nodes
- `[]` - square corners (default)
- `()` - rectangle node with rounded corners
- `(())` - circle node
- `([])` - pill shaped node
- `{}` - diamond shaped node
- `{{}}` - 6 sided node
- `|Line Label|` - add a label to an arrow line 
- `LR` - chart goes left to right, `TD` chart gors top down, `BT` for bottom to top, nothing is default

## Sequence diagram example

```mermaid
sequenceDiagram
    autonumber
    participant Client
    participant OAuthProvider
    participant Server
    Client->>OAuthProvider: Request access
    activate OAuthProvider
    OAuthProvider->>Client: Access token
    deactivate OAuthProvider
    Client->>Server: Request resource
    activate Server
    Server->>OAuthProvider: Validate token
    activate OAuthProvider
    OAuthProvider->>Server: Token valid
    deactivate OAuthProvider
    Server->>Client: Send resource
    deactivate Server
```

- `autonumber` to number each sequence
- `->>` - used in sequence diagrams to connect nodes
- activate, deactivate

## Class diagram example

```mermaid
classDiagram
    class Order {
        +OrderStatus status
    }
    class OrderStatus {
        <<enumeration>>
        FAILED
        PENDING
        PAID
    }
    class PaymentProcessor {
        <<interface>>
        -String apiKey
        #connect(String url, JSON header)
        +processPayment(Order order) OrderStatus
    }
    class Customer {
        +String name
    }
    Customer <|-- PrivateCustomer
    Customer <|-- BusinessCustomer
    PaymentProcessor <|-- StripeProcessor
    PaymentProcessor <|-- PayPalProcessor
    Order o-- Customer
```

- `<<enumeration>>`
- `<<interface>>`
- `-` indicates private
- `+` indicates public 
- `#` indicates protected
- inheritance, composition, and aggregation relationships
- inheritance: class and sub-class relationship - use `<|--`
- composition vs aggregation: special cases of associations 
- use `o--` for aggregation
- use `*--` for composition

## Entity Relationship Diagram example

This is more generic than a class diagram

```mermaid
erDiagram
    Customer ||--o{ Order: places
    Order ||--o{ LineItem: contains
    Customer {
        String id
        String name
    }
    Order {
        String id
        OrderStats status
    }
    LineItem {
        String item-number
        String description
        int quantity
        int price
    }
```

- use `||--o{`, no
- `|o` means 0 or 1
- `||` exactly 1
- `o{` 0 or more
- `|{` 1 or more
- attributes: 