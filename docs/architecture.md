# Architecture

## System Overview

```mermaid
graph LR
    subgraph Input
        USER[User Message] --> SKILL[SKILL.md\nRouter + Core Logic]
    end

    subgraph Routing
        SKILL --> STAGE{Stage Detection}
        SKILL --> CMD{Command Parser}
        SKILL --> TOPIC{Topic Router}
    end

    subgraph Reference Files
        CMD --> COMMANDS[commands/]
        TOPIC --> PLAYBOOKS[playbooks/]
        TOPIC --> PITCH[pitch/]
        TOPIC --> TEMPLATES[templates/]
        TOPIC --> COMPLIANCE[compliance/]
        TOPIC --> CONTRACTS[contracts/]
        TOPIC --> ACCOUNTING[accounting/]
        TOPIC --> IP[ip/]
        STAGE --> REGIONAL[regional/]
    end

    subgraph Output
        COMMANDS --> RESPONSE[Task Response\nwith Steps]
        PLAYBOOKS --> RESPONSE
        PITCH --> RESPONSE
        TEMPLATES --> RESPONSE
        COMPLIANCE --> RESPONSE
        CONTRACTS --> RESPONSE
        ACCOUNTING --> RESPONSE
        IP --> RESPONSE
        REGIONAL --> RESPONSE
    end

    style USER fill:#2563eb,stroke:#1e40af,color:#fff
    style SKILL fill:#7c3aed,stroke:#6d28d9,color:#fff
    style RESPONSE fill:#22c55e,stroke:#16a34a,color:#fff
```

## Session Flow

```mermaid
sequenceDiagram
    participant U as User
    participant S as SKILL.md
    participant R as Reference File

    U->>S: Opens conversation
    S->>U: "Let's move. What are we building today?"
    U->>S: Describes need
    S->>S: Detect stage (0-4)
    S->>S: Identify mode (Focus/Sprint/Recovery/etc.)
    S->>R: Load relevant reference file
    R->>S: Reference content
    S->>U: Task Response (goal + time + steps)
    U->>S: Completes task or asks follow-up
    S->>U: Next task or session wrap
```

## Command Routing Flow

```mermaid
sequenceDiagram
    participant U as User
    participant S as SKILL.md
    participant SC as session-commands.md
    participant BC as binder-commands.md
    participant OC as ops-commands.md

    U->>S: Types /command
    alt Session command
        S->>SC: Load session-commands.md
        SC->>S: Command definition
    else Binder command
        S->>BC: Load binder-commands.md
        BC->>S: Command definition
    else Ops command
        S->>OC: Load ops-commands.md
        OC->>S: Command definition
    end
    S->>U: Execute command with Task Response Format
```

## Investor Binder Build Flow

```mermaid
graph TD
    START[/binder command] --> ASSESS{Current Stage?}

    ASSESS -->|Stage 0-1| SKELETON[Build Binder Skeleton\nSections 1-5 only]
    ASSESS -->|Stage 2| FULL[Full 17-Section Build]
    ASSESS -->|Stage 3-4| UPGRADE[Upgrade for Larger Rounds]

    FULL --> S1[1. Cover Page]
    FULL --> S2[2. Executive Summary]
    FULL --> S3[3. Problem]
    FULL --> S4[4. Solution]
    FULL --> S5[5. Market Size]
    FULL --> S6[6-17. Remaining Sections]

    S6 --> SCORE[/score - Rate Binder]
    SCORE --> GAPS[Identify Gaps]
    GAPS --> ITERATE[Iterate Until Ready]

    style START fill:#2563eb,stroke:#1e40af,color:#fff
    style ASSESS fill:#f59e0b,stroke:#d97706,color:#000
    style SCORE fill:#7c3aed,stroke:#6d28d9,color:#fff
    style ITERATE fill:#22c55e,stroke:#16a34a,color:#fff
```

## Progressive Disclosure

The skill uses progressive disclosure to manage complexity:

```mermaid
graph TD
    L1[Layer 1: SKILL.md\nAlways in context] --> L2[Layer 2: Commands\nLoaded on /command]
    L2 --> L3[Layer 3: Playbooks\nLoaded by topic]
    L3 --> L4[Layer 4: Templates\nLoaded on demand]
    L4 --> L5[Layer 5: Regional\nLoaded by state]

    style L1 fill:#ef4444,stroke:#dc2626,color:#fff
    style L2 fill:#f59e0b,stroke:#d97706,color:#000
    style L3 fill:#3b82f6,stroke:#2563eb,color:#fff
    style L4 fill:#8b5cf6,stroke:#7c3aed,color:#fff
    style L5 fill:#22c55e,stroke:#16a34a,color:#fff
```

**Rule:** Never load all reference files at once. Load only what the current task requires.
