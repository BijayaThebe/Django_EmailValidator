# Django_EmailValidator
Implement the email validation using Django Framework 

# Email Validation Flow



# Salesman Graphs
graph TD
    %% Level 1 - Start from A
    A[Start at A] -->|10| B1[B]
    A -->|15| C1[C]
    A -->|20| D1[D]
    A -->|25| E1[E]
    A -->|30| F1[F]

    %% Level 2 - Next cities from B
    B1 -->|35| C2[C]
    B1 -->|25| D2[D]
    B1 -->|17| E2[E]
    B1 -->|28| F2[F]

    %% Level 3 - Return to A (for illustration)
    C2 -->|15| A_end[A]
    D2 -->|20| A_end
    E2 -->|25| A_end
    F2 -->|30| A_end

    %% Level 2 - Next cities from C
    C1 -->|35| B2[B]
    C1 -->|30| D3[D]
    C1 -->|28| E3[E]
    C1 -->|40| F2b[F]

    %% Return to A
    B2 -->|10| A_end
    D3 -->|20| A_end
    E3 -->|25| A_end
    F2b -->|30| A_end

    %% Level 2 - Next cities from D
    D1 -->|25| B3[B]
    D1 -->|30| C3[C]
    D1 -->|22| E4[E]
    D1 -->|16| F3[F]

    %% Return to A
    B3 -->|10| A_end
    C3 -->|15| A_end
    E4 -->|25| A_end
    F3 -->|30| A_end

    %% Level 2 - Next cities from E
    E1 -->|17| B4[B]
    E1 -->|28| C4[C]
    E1 -->|22| D4[D]
    E1 -->|35| F4[F]

    %% Return to A
    B4 -->|10| A_end
    C4 -->|15| A_end
    D4 -->|20| A_end
    F4 -->|30| A_end

    %% Level 2 - Next cities from F
    F1 -->|28| B5[B]
    F1 -->|40| C5[C]
    F1 -->|16| D5[D]
    F1 -->|35| E5[E]

    %% Return to A
    B5 -->|10| A_end
    C5 -->|15| A_end
    D5 -->|20| A_end
    E5 -->|25| A_end



