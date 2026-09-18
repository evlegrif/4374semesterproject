```mermaid
graph LR
    Root[Smart Parking Platform]

    %% Level 2 Teams
    Root --> B[1.1 Backend/API]
    Root --> P[1.2 Payment Integration]
    Root --> M[1.3 Mapping & Location]
    Root --> W[1.4 Web Application]
    Root --> Mo[1.5 Mobile App]
    Root --> QA[1.6 QA & Testing]

    %% Level 3 Backend
    B --> B1[1.1.1 Setup user registration]
    B --> B2[1.1.2 Integrate ALPR software]
    B --> B3[1.1.3 Build 3rd party architecture]
    B --> B4[1.1.4 Configure pricing engine]
    B --> B5[1.1.5 Milestone: Infrastructure Deployed]

    %% Level 3 Payment
    P --> P1[1.2.1 Integrate payment APIs]
    P --> P2[1.2.2 Start receipt database]
    P --> P3[1.2.3 Milestone: Payment Gateway Live]

    %% Level 3 Mapping
    M --> M1[1.3.1 Build interactive map]
    M --> M2[1.3.2 Integrate navigation handoff]
    M --> M3[1.3.3 Milestone: Location Services Connected]

    %% Level 3 Web App
    W --> W1[1.4.1 Build operator admin UI]
    W --> W2[1.4.2 Create occupancy views]
    W --> W3[1.4.3 Milestone: Web Portal Live]

    %% Level 3 Mobile App
    Mo --> Mo1[1.5.1 Build driver profiles]
    Mo --> Mo2[1.5.2 Create reservation logic]
    Mo --> Mo3[1.5.3 Build current activity UI]
    Mo --> Mo4[1.5.4 Sync push notifications]
    Mo --> Mo5[1.5.5 Milestone: Mobile App Ready]

    %% Level 3 QA
    QA --> QA1[1.6.1 Audit city law compliance]
    QA --> QA2[1.6.2 Test app end-to-end]
    QA --> QA3[[1.6.3 Goal: Project Deployed]]

    %% Styling
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:1px;
    classDef root fill:white,stroke:#003d59,stroke-width:2px,color:black;
    classDef milestone fill:#d4edda,stroke:#28a745,stroke-width:2px;
    
    class Root root;
    class B5,P3,M3,W3,Mo5,QA3 milestone;
