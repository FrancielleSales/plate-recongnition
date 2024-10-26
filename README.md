# PLATE RECOGNITION
Tool for automatic recognition and detection of Brazilian license plates in images

## Creating the development environment

### Requirements

- Django
- Node.js
- Postgresql
- Máquina com qualquer distribuição Linux (pode estar também em VM ou WSL)

### Database

**With PostgreSQL installed, access it:**
```sh
psql -U postgres
```
**Create a user to manage the database:**
```sh
CREATE USER dbpr WITH PASSWORD '321';
```
**Create the database:**
```sh
CREATE DATABASE db_pr;
```
**Grant permissions to the user:**
```sh
GRANT ALL PRIVILEGES ON DATABASE db_pr TO dbpr;
```
To exit the shell, use: \q

**To create the database tables and add users for testing:**
```sh
cd /database
python3 config.py
```
**To run database check:**
```sh
cd database/maintenance
python3 verify_database.py
```
**To create a backup:**
```sh
cd /database/backups
python3 backup_database.py
```

### Backend

### Frontend
