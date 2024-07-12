# Salon Management System

###### Technologies:
<p align="center">
<img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/postgresql-colored.svg" width="75" height="75" alt="PostgreSQL" style="margin: 10px 15px 0 15px;" />
<img src="https://img.icons8.com/color/75/000000/console.png" width="75" height="75" alt="Bash" style="margin: 10px 15px 0 15px;" />
</p>

- **Bash:** Used for scripting to interact with PostgreSQL for database management.
- **PostgreSQL:** Relational database used to store and manage customer, service, and appointment data.

## Description

This project is a management system designed for small businesses, specifically tailored for a beauty salon. It includes functionalities for managing customers, services, and appointments through a PostgreSQL database and a Bash script interface.

## Project Structure

### Database Structure and Initialization

The `salon.sql` file contains the database schema definition and initial data insertion. Key tables include:

- `customers`: Stores customer information including name and phone number.
- `services`: Lists available salon services like cut, color, and perm.
- `appointments`: Tracks scheduled appointments with service details and times.

### Bash Shell Script

The `salon.sh` script serves as the command-line interface to interact with the database. Key functionalities include:

- Viewing available services and selecting service options.
- Creating new customer records and managing customer appointments.
- Inserting and querying appointment details based on customer preferences.

### Authentication and Security

The system includes basic authentication via Bash script for accessing management features. Passwords are hashed using secure methods to ensure data integrity and user privacy.

#### Benefits of Using Bash and PostgreSQL

- **Ease of Use:** Utilizes familiar command-line interfaces for quick database interactions.
- **Reliability:** PostgreSQL ensures robust data management and relational capabilities.
- **Security:** Implements secure password hashing and basic authentication for controlled access.

## How to Use

### Setting Up the Database

1. **Ensure PostgreSQL is installed**: Install PostgreSQL on your system if not already available.

2. **Create the Database**: Run the SQL script to create the necessary tables and initial data:
   ```bash
   psql -U <username> -f salon.sql
   ```

### Running the Bash Script

1. **Grant Execution Permission**: Ensure the script has executable permissions:
   ```bash
   chmod +x salon.sh
   ```

2. **Execute the Script**: Start the salon management system by running:
   ```bash
   ./salon.sh
   ```

### Navigation within the Script

- **Main Menu**:
  - Allows selecting options to manage customers, services, and appointments.
  
- **Customer and Appointment Management**:
  - Create new customer records, view available services, and schedule appointments.

## Technologies Used

- **PostgreSQL**: Reliable and efficient database management.
- **Bash Scripting**: Command-line interface for easy database interactions.

---
#### This is a FreeCodeCamp Challenge for Relational Database Projects Certification
<p align="center">
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg" width="250" height="75" alt="freeCodeCamp" style="margin: 0 15px; opacity: 0.6" />
</p>
