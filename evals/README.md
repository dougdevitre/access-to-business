# Evals

## eval-set.json

Test cases for verifying that the Access to Business skill triggers correctly on various user inputs.

```mermaid
flowchart LR
    A["Load Skill"] --> B["Send Trigger"]
    B --> C["Check Activation"]
    C --> D["Verify Route"]

    style A fill:#4a90d9,stroke:#2c5f8a,color:#fff
    style B fill:#f5a623,stroke:#c47d10,color:#fff
    style C fill:#e67e22,stroke:#b35e0a,color:#fff
    style D fill:#27ae60,stroke:#1a7a42,color:#fff
```

### What It Tests

The eval set covers trigger phrases across all skill capabilities:

- Stage detection (idea, pre-revenue, growth, scaling)
- Command recognition (`/start`, `/binder`, `/pitch`, etc.)
- Topic routing (fundraising, legal, compliance, metrics, etc.)
- Edge cases (ambiguous requests, multi-topic queries)

### How to Use

1. Load the skill into a Claude environment
2. Send each trigger phrase from `eval-set.json`
3. Verify the skill activates and routes to the correct mode/file
4. Check that the response follows the Task Response Format

### Format

Each test case includes:
- `input` -- the user message to send
- `expected_trigger` -- whether the skill should activate
- `expected_route` -- which file or mode should be loaded
