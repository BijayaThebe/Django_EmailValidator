# Django_EmailValidator
Implement the email validation using Django Framework 


# Email Validation Flow
flowchart TD
    A[Input Email List] --> B[For Each Email Extract Domain]
    B --> C[Format Check]
    C -->|Valid| D[DNS MX Lookup]
    C -->|Invalid| Z[Mark as Invalid and Stop Checks]
    D --> E[SMTP Handshake Check]
    E --> F[SPF Check DNS TXT]
    F --> G[DKIM Check DNS TXT]
    G --> H[DMARC Check DNS TXT]
    H --> I[Aggregate Results]
    I --> J[Return JSON Response]

    style Z fill:#f88,stroke:#000,stroke-width:1px
    style I fill:#8f8,stroke:#000,stroke-width:1px

