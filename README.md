
# Flight Management System

### Overview
* This project is a web-based system designed for the effective preparation and management of flight lists in an imaginary airline. It streamlines and optimizes the process of organizing flights and flight personnel, including flight information, pilot crew, cabin crew, and passengers. 

### Features

* **Flight Selection:** Users can select flights by unique flight number or filter through various criteria.
  
* **Information Gathering:** The system queries APIs to gather details about scheduled flights, crew, and passengers.

* **Multiple Views:** Information is presented through tabular, plane, and extended views.

* **Database Operations:** Supports generating, viewing, storing, and retrieving roster information with options for SQL or NoSQL databases.

* **Crew Selection:** Allows automatic or manual selection of flight and cabin crew based on constraints.

* **Passenger Management:** Manages passenger information, including seat assignments.

* **Authentication and Authorization:** Secure access with role-based permissions.


## System Requirements

### Functional Requirements
1. **Flight Selection:**
   * Users can select flights by entering flight numbers or applying filters.
   * Information is retrieved from Flight Information, Flight Crew, Cabin Crew, and Passenger APIs.

2. **Views:**
   * The system provides tabular, plane, and extended views for displaying information.

3. **Database Management:**
   * Supports SQL and NoSQL databases.
   * Allows exporting roster information in JSON format.

4. **Authentication/Authorization:**
   * Secure login and role-based access control.
  
## User Requirements
* **Ease of Use:** Intuitive interfaces for flight selection and information viewing.
* **Information Access:** Comprehensive details about flights, crew members, and passengers.
* **Database Management:** Efficient handling of roster information.
  
## User Roles and Use Cases
### Roles

1. Passenger:
    * Search flights, view seating plans, and flight information.
    * Log in with username and password.

2. Cabin Crew:
    * Search flights, view and update seating plans, flight information, and crew information.
    * Log in with username and password.
  
3. Flight Crew:
    * Search flights, view seating plans, flight information, and crew information.
    * Log in with username and password.

4. Admin:
    * Update or add flight and passenger information.
    * Log in with username and password.
  
## Use Cases
* **Admin:** Opens the application, logs in, searches for flights, updates flight crew information, and logs out.
  
* **Passenger:** Opens the application, logs in, searches for flights, views flight information in different views, and logs out.

* **Flight Crew:** Similar to the passenger but with additional options to view flight crew information.

* **Cabin Crew:** Similar to flight crew but with the ability to update seating plans.

## Architecture and Design 
### System Architecture
* Microservices Architecture: Each service (Main System, Flight Information, Flight Crew Information, Cabin Crew Information, Passenger Information) is developed, deployed, and scaled independently.
  
### Data Storage
* Polyglot Persistence: Uses SQL for structured data and NoSQL for unstructured data.

### API Design
* RESTful Principles: Ensures statelessness, cacheability, and a uniform interface.

### UI Design
* Responsive Web Design (RWD): Adapts to various device sizes and resolutions.

### Design Patterns
* Repository Pattern: For data access layers.
* Singleton Pattern: For database connection objects and configuration settings.

### Deployment
* Containerization with Docker: Ensures consistency across development, testing, and production environments.
  
### Diagrams
* ER Diagram
* Component Interface Diagrams
* UML Class and Interaction Diagrams
  
## Tech Stack
* **Frontend:** JavaScript, React.js, HTML/CSS.
* **Backend:** Python, Django.
* **Database:** MySQL, NoSQL.
* **DevOps:** Docker, CI/CD, Version Control.

  # Steps
  1. Clone the repository:
     * “` git clone https://github.com/yourusername/flight-management-system.git “`
     
  2. Navigate to the project directory:
    *  “` cd flight-management-system “`

  3. Set up and activate the virtual environment (optional but recommended):
     * “` python -m venv venv “`
     * “` source venv/bin/activate  # On Windows use `venv\Scripts\activate` “`
     
  4. Install backend dependencies:
     * “` pip install -r requirements.txt “`
     
  5. Install frontend dependencies:
     * “` npm install“`

  6. Set up the database:
     * “` python manage.py migrate “`
     
 # Usage
## Running the Application
1. Start the backend server:
 * “`python manage.py runserver“`

2. Start the frontend development server:
   * “`npm start“`

3.  Access the application at " http://localhost:3000 "


   ## Running with Docker
1. Build the Docker images:
   * “` docker-compose build “`

2. Run the Docker containers:
   * “` docker-compose up“`


##   Development

### Running Tests
* Backend:
  * “` python manage.py test “`

* Frontend:
  * “` npm test “`

  ## Deployment
* Build the Docker images:
* “` docker-compose build “`

* Run the Docker containers:
* “` docker-compose up “`


   ## Contributing

1. Fork the repository.
   
2. Create a new branch:
   * “` git checkout -b feature-name “`

3. Make your changes and commit them:
   * “` git commit -m "Add feature" “`

4. Push to the branch:
   * “` git push origin feature-name “`

5. Open a pull request.

## Team Members and Responsibilities
**Product Owner**
- Nur Deren Sakin

**Frontend Team**
- Nur Deren Sakin
- Ali Eren Şahin
- Kemal Efe Kolaylı
- Mert Genç
- Turhan Can Ada

**Backend Team**
- Ege Diriöz
- İsmail Aydın Karayılan
- Cem Görkem Baysal
- Alp Bartu Utar
- Alper Çamlı
