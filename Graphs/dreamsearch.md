~~~mermaid
flowchart TD
    classDef core fill:#1976d2,color:#fff,stroke:#1976d2
    classDef component fill:#7986cb,color:#fff,stroke:#7986cb
    classDef interface fill:#81c784,color:#000,stroke:#81c784
    
    subgraph Core["Core Processing"]
        direction TB
        CS[Cognitive Simulator]:::core
        SN[Social Network Analyzer]:::core
        PM[Predictive Model]:::core
    end
    
    subgraph Components["Key Components"]
        direction TB
        PSY[Psychological Pattern Recognition]:::component
        DM[Dream State Processor]:::component
        UC[Unconscious Connection Mapper]:::component
        PA[Pattern Analyzer]:::component
    end
    
    subgraph Interfaces["Data Interfaces"]
        direction TB
        DI[Dream Input]:::interface
        PI[Prisoner Data]:::interface
        CI[Cult Follower Data]:::interface
        GI[Government Agent Data]:::interface
    end
    
    DI --> DM
    PI --> PSY
    CI --> SN
    GI --> PM
    
    DM --> UC
    PSY --> PA
    UC --> PA
    SN --> PA
    PA --> PM
    
    PM --> CS
    CS --> SN
    
    subgraph Legend["Legend"]
        direction LR
        L1[Core Processing]:::core
        L2[Components]:::component
        L3[Interfaces]:::interface
    end
~~~
