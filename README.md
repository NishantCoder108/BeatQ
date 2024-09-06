1. Run by Docker

-   create dockerfile where all configuration things are written

-   ```js
     docker build -t BeatQ .

    ```

-   ```
     docker run BeatQ -p 3000:3000
    ```

## Note

1. For running prisma , we must ensure migrate dev and then we can run db.
2. For running postgres , we must to see his password , username and localhost

    ```bash
    docker run --name postgres -e POSTGRES_PASSWORD=mysecretpassword -e POSTGRES_DB=muzerdb -p 5432:5432 -d postgres
    ```

3. Put in .env file

    ```bash

    DATABASE_URL=postgres://postgres:mysecretpassword@localhost:5432/db

    ```
