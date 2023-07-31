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
1. `id))I am a bang((`
1. `id)I am a cloud(`
1. 

## Flowchart example

- `flowchart` or use graph, 

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

## Gantt chart

```mermaid
gantt
    title A Gantt Diagram
    dateFormat YYYY-MM-DD
    tickInterval 5day
    section Main
        A task          :a1, 2014-01-01, 30d
        Another task    :after a1, 20d
    section Secondary
        Secondary       :2014-01-12, 12d
        another task    :24d
```

```mermaid
gantt
    dateFormat HH:mm
    %% This is a comment
    axisFormat %H:%M
    Initial milestone : milestone, m1, 17:49, 2m
    Task A : 10m
    Task B : 5m
    Final milestone : milestone, m2, 18:08, 4m
```

- dateFormat 
- axisFormat
- tickInterval: `/^([1-9][0-9]*)(minute|hour|day|week|month)$/;`
- weekday 
- `%%` = comment

## gitGraph example

```mermaid
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit type: HIGHLIGHT
   checkout main
   merge develop
   commit
   commit
```

- gitGraph
- where are the git hashes coming from?
- commit 
- id, tag, type - `commit id: "your_custom_id"` - `commit id: "Normal" tag: "v1.0.0"`
- branch
- checkout
- merge
- `%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'showBranches': false}} }%%`
- the page on this is really long...

## Journey diagram

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

- journey, title, section
- `Task name: <score>: <comma separated list of actors>`

## quadrantChart diagram

```mermaid
quadrantChart
    title Reach and engagement of campaigns
    x-axis Low Reach --> High Reach
    y-axis Low Engagement --> High Engagement
    quadrant-1 We should expand
    quadrant-2 Need to promote
    quadrant-3 Re-evaluate
    quadrant-4 May be improved
    Campaign A: [0.3, 0.6]
    Campaign B: [0.45, 0.23]
    Campaign C: [0.57, 0.69]
    Campaign D: [0.78, 0.34]
    Campaign E: [0.40, 0.34]
    Campaign F: [0.35, 0.78]
```

> This chart is not displaying on GitHub?!?

- title, 
- x-axis: `x-axis <text> --> <text>` or `x-axis <text>`
- y-axis: `y-axis <text> --> <text>` or `y-axis <text>`
- quadrant-1 - top right, moves counter-clockwise - `quadrant-1 <text>`
- quadrant-2, quadrant-3, quadrant-4
- `<text>: [x, y]` - x and y value is in the range 0 - 1

## Pie chart

```mermaid
pie
    title Pets adopted by volunteers
    "Dogs" : 386
    "Cats" : 185
    "Rabbits" : 85
```

- `%%{init: {"pie": {"textPosition": 0.5}, "themeVariables": {"pieOuterStrokeWidth": "5px"}} }%%`

## requirementDiagram

```mermaid
requirementDiagram

    requirement test_req {
    id: 1
    text: the test text.
    risk: high
    verifymethod: test
    }

    element test_entity {
    type: simulation
    }

    test_entity - satisfies -> test_req
```

- `{name of source} - <type> -> {name of destination}`

## C4Context

```mermaid
C4Context
      title System Context diagram for Internet Banking System
      Enterprise_Boundary(b0, "BankBoundary0") {
        Person(customerA, "Banking Customer A", "A customer of the bank, with personal bank accounts.")
        Person(customerB, "Banking Customer B")
        Person_Ext(customerC, "Banking Customer C", "desc")

        Person(customerD, "Banking Customer D", "A customer of the bank, <br/> with personal bank accounts.")

        System(SystemAA, "Internet Banking System", "Allows customers to view information about their bank accounts, and make payments.")

        Enterprise_Boundary(b1, "BankBoundary") {

          SystemDb_Ext(SystemE, "Mainframe Banking System", "Stores all of the core banking information about customers, accounts, transactions, etc.")

          System_Boundary(b2, "BankBoundary2") {
            System(SystemA, "Banking System A")
            System(SystemB, "Banking System B", "A system of the bank, with personal bank accounts. next line.")
          }

          System_Ext(SystemC, "E-mail system", "The internal Microsoft Exchange e-mail system.")
          SystemDb(SystemD, "Banking System D Database", "A system of the bank, with personal bank accounts.")

          Boundary(b3, "BankBoundary3", "boundary") {
            SystemQueue(SystemF, "Banking System F Queue", "A system of the bank.")
            SystemQueue_Ext(SystemG, "Banking System G Queue", "A system of the bank, with personal bank accounts.")
          }
        }
      }

      BiRel(customerA, SystemAA, "Uses")
      BiRel(SystemAA, SystemE, "Uses")
      Rel(SystemAA, SystemC, "Sends e-mails", "SMTP")
      Rel(SystemC, customerA, "Sends e-mails to")

      UpdateElementStyle(customerA, $fontColor="red", $bgColor="grey", $borderColor="red")
      UpdateRelStyle(customerA, SystemAA, $textColor="blue", $lineColor="blue", $offsetX="5")
      UpdateRelStyle(SystemAA, SystemE, $textColor="blue", $lineColor="blue", $offsetY="-10")
      UpdateRelStyle(SystemAA, SystemC, $textColor="blue", $lineColor="blue", $offsetY="-40", $offsetX="-50")
      UpdateRelStyle(SystemC, customerA, $textColor="red", $lineColor="red", $offsetX="-50", $offsetY="20")

      UpdateLayoutConfig($c4ShapeInRow="3", $c4BoundaryInRow="1")
```

5 types of C4 charts are supported.

1. System Context (C4Context)
2. Container diagram (C4Container)
3. Component diagram (C4Component)
4. Dynamic diagram (C4Dynamic)
5. Deployment diagram (C4Deployment)

## mindmap

```mermaid
mindmap
  root((mindmap))
    Origins
      Long history
      ::icon(fa fa-book)
      Popularisation
        British popular psychology author Tony Buzan
    Research
      On effectiveness<br/>and features
      On Automatic creation
        Uses
            Creative techniques
            Strategic planning
            Argument mapping
    Tools
      Pen and paper
      Mermaid
```

With icons:

```mermaid
mindmap
    Root
        A
        ::icon(fa fa-book)
        B(B)
        ::icon(mdi mdi-skull-outline)
```

syntax:

```
mindmap
    Root
        A
            B
            C
```

## timeline

```mermaid
timeline
    title History of Social Media Platform
    2002 : LinkedIn
    2004 : Facebook
         : Google
    2005 : Youtube
    2006 : Twitter
```

Syntax:

```
{time period} : {event}
<!-- or -->
{time period} : {event} : {event}
<!-- or -->
{time period} : {event}
              : {event}
              : {event}
```

## ZenUML

```mermaid
zenuml
    title Annotators
    @Actor Alice
    @Database Bob
    Alice->Bob: Hi Bob
    Bob->Alice: Hi Alice
```

> Not displaying in VS Code?!?

## State diagrams

```mermaid
stateDiagram
    [*] --> Still
    Still --> [*]

    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

> Not displaying in VS Code?!?

## Sankey diagram (beta)

```mermaid
sankey-beta

%% source,target,value
Electricity grid,Over generation / exports,104.453
Electricity grid,Heating and cooling - homes,113.726
Electricity grid,H2 conversion,27.14
```

> Not displaying in VS Code?!?
