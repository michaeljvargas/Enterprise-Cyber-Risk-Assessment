flowchart TB
  %% Threat scenarios and attack paths linked to risk IDs

  subgraph T1["R-01: Credential Stuffing → Account Takeover"]
    A1[Attacker] --> L1[Login Page]
    L1 --> Auth1[Authentication Service]
    Auth1 --> Acc1[Customer Account Access]
    Acc1 --> Impact1[Impact: Fraud loss / Customer harm]
  end

  subgraph T2["R-03: Phishing → Privileged Access Misuse"]
    P2[Phishing Email] --> E2[Employee]
    E2 --> Admin2[Admin Tools]
    Admin2 --> Data2[Customer Data / Config Changes]
    Data2 --> Impact2[Impact: Data exposure / Unauthorized actions]
  end

  subgraph T3["R-04: Cloud Misconfiguration → Data Exposure"]
    Net3[Public Internet] --> Mis3[Misconfigured Storage / Public Resource]
    Mis3 --> Leak3[Customer PII + Financial Data]
    Leak3 --> Impact3[Impact: Breach / Regulatory + reputational risk]
  end

