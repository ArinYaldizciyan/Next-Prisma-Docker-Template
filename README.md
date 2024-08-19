
## Getting Started
Install required modules with npm

```bash
npm i
```

Make sure to install Docker Desktop

Set up environment variables.
- Create a .env file with the following parameters
- DATABASE_URL="postgresql://postgres:{user_name}@db:5432/{db_name}?schema=public"
- POSTGRES_USER="user_name"
- POSTGRES_DB="db_name"
- POSTGRES_PASSWORD="postgres"
  #Do not change
- PGUSER="postgres"

## Development
Once you are ready to develop

```bash
docker-compose up --build
```

Then run

```bash
npm run migrate-dev
```
to set up initial migrations for prisma. 

Start modifying your code in your host environment and the mounts will automatically update your code in the container. No re-run is necessary. 

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.
