# Apps

## intake-app.html

A self-contained React intake assessment app that helps founders identify their startup stage and priorities.

Built as a single HTML file with no external dependencies -- open it in any browser to use.

```mermaid
flowchart LR
    A["Open App"] --> B["Answer Questions"]
    B --> C["Get Stage 0-4"]
    C --> D["Start /start Session"]

    style A fill:#4a90d9,stroke:#2c5f8a,color:#fff
    style B fill:#f5a623,stroke:#c47d10,color:#fff
    style C fill:#7b68ee,stroke:#5a4abf,color:#fff
    style D fill:#27ae60,stroke:#1a7a42,color:#fff
```

### How It Works

1. Open `intake-app.html` in a browser
2. Answer the assessment questions
3. Get your startup stage (0-4) and recommended focus areas
4. Use the results to guide your first `/start` session

### Technical Details

- Self-contained: React is bundled inline, no CDN or npm required
- Single file: Everything (HTML, CSS, JS) in one `.html` file
- Offline-capable: Works without an internet connection
