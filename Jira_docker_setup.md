
# Jira Docker Setup with PostgreSQL

This guide will help you set up Jira with PostgreSQL in Docker, including an Admin login configuration. We will create the necessary `docker-compose.yml` 
## Prerequisites

- Docker installed on your machine
- Docker Compose installed
- Basic knowledge of Docker and Docker Compose

---

## Directory Structure

```
/your-directory
├── docker-compose.yml

```


## docker-compose.yml

Here is the `docker-compose.yml` to set up Jira and PostgreSQL services.

```yaml
version: '3.8'

services:
  jira:
    build: .
    container_name: jira
    ports:
      - "8080:8080"
    environment:
      - ATL_JDBC_URL=jdbc:postgresql://db:5432/jiradb
      - ATL_JDBC_USER=jirauser
      - ATL_JDBC_PASSWORD=jirapassword
      - ATL_DB_DRIVER=org.postgresql.Driver
    depends_on:
      - db
    volumes:
      - jira_data:/var/atlassian/application-data/jira
    restart: unless-stopped

  db:
    image: postgres:13
    container_name: jira_db
    environment:
      POSTGRES_USER: jirauser
      POSTGRES_PASSWORD: jirapassword
      POSTGRES_DB: jiradb
    volumes:
      - postgres_data:/var/lib/postgresql/data
    restart: unless-stopped

volumes:
  jira_data:
  postgres_data:
```

---

## Steps to Set Up

### 1. **Create the Files:**

- Create a new directory for your setup.
- Save the `docker-compose.yml` in this directory.

### 2. **Build and Start the Containers:**

- Open a terminal and navigate to your project directory.
- Run the following command to build the Docker images and start the services:

```bash
docker-compose up -d
```

### 3. **Access Jira:**

- Open your web browser and go to `http://localhost:8080`.
- Jira will prompt you to complete the setup wizard.

### 4. **Complete the Setup Wizard:**

- During the setup, select **PostgreSQL** as the database type.
- Provide the following database connection details:
  - **Hostname**: `db`
  - **Database**: `jiradb`
  - **Username**: `jirauser`
  - **Password**: `jirapassword`
- Jira will automatically connect to the PostgreSQL database.

### 5. **Create Admin Account:**

- As part of the setup wizard, you'll create an admin account for Jira.
- Set the username and password for the admin user.

---

## Admin Login

- After completing the setup wizard, Jira will be ready to use.
- Open your browser and go to `http://localhost:8080` to log in with the admin credentials you created.

---


