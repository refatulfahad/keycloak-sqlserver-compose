# Keycloak with External SQL Server (Docker Compose)  

This **Docker Compose** setup runs **Keycloak** with an **external SQL Server** database.  

## Setup  

1. **Clone the repository**  
   - git clone https://github.com/refatulfahad/keycloak-sqlserver-compose.git
   - cd keycloak-sqlserver-compose

2. **Start Keycloak**  
   docker-compose up -d

3. **Ensure SQL Server is running**  
   - **Create the database** before starting Keycloak.  
   - **To connect via SSMS**, use:  
     - **Server Name:** `localhost,1434`  
     - **Authentication:** SQL Server  
     - **Username & Password:** Use `KC_DB_USERNAME` and `KC_DB_PASSWORD` from `docker-compose.yml`.
       
4. **Access Keycloak**  
   - Open: `http://localhost:8080`  
   - Admin Login:  
     - **Username:** `admin`  
     - **Password:** `admin`
