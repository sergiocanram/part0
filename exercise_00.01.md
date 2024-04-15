graph TD;
    A[Navegador] -->|1. Usuario escribe nota y hace clic en Save| B(Cliente);
    B -->|2. POST https://studies.cs.helsinki.fi/exampleapp/new_note| C[Servidor];
    C -->|3. La nota se guarda en la base de datos| D[Base de Datos];
    D -->|4. La base de datos confirma la operación| C;
    C -->|5. Respuesta 200 OK| B;
    B -->|6. La página se actualiza mostrando la nueva nota| A;
