# Django_EmailValidator
Implement the email validation using Django Framework 
# Email Validation Flow

```mermaid
flowchart TD
    A[Input Email List] --> B[For Each Email: Extract Domain]
    B --> C[1️⃣ Format Check]
    C -->|Valid| D[2️⃣ DNS MX Lookup]
    C -->|Invalid| Z[Mark as Invalid & Stop Checks]
    D --> E[3️⃣ SMTP Handshake Check]
    E --> F[4️⃣ SPF Check (DNS TXT)]
    F --> G[5️⃣ DKIM Check (DNS TXT)]
    G --> H[6️⃣ DMARC Check (DNS TXT)]
    H --> I[Aggregate Results]
    I --> J[Return JSON Response]

    style Z fill:#f88,stroke:#000,stroke-width:1px
    style I fill:#8f8,stroke:#000,stroke-width:1px
