# <span style="vertical-align: sub"><img src="src/main/resources/taxi-icon.png"></span> Taxi-Service Application <span style="vertical-align: sub"><img src="src/main/resources/taxi-icon.png"></span>

### <span style="vertical-align: sub"><img src="src/main/resources/description.png"></span> Project description:

`Simple Web-application that supports registration, authentication and other CRUD operations`

### <span style="vertical-align: sub"><img src="src/main/resources/features.png"></span> Features:

- registration of driver
- authentication of driver
- create/update/remove of driver
- create/update/remove of car manufacturer
- create/update/remove of car 
- display list of all drivers
- display list of all driver's cars
- display list of all manufacturers
- display list of all cars

### <span style="vertical-align: sub"><img src="src/main/resources/structure.png"></span> Structure:

1. `main.java` package folders:

   - `controller` - contains presentation layer classes
   - `dao` - contains DAO layer interfaces and classes
   - `exception` - contains custom exceptions
   - `lib` - contains injector and custom annotations
   - `model` - contains models for car/manufacturer/driver
   - `service` - contains business logic layer interfaces and classes
   - `util` - contains class to create connection to DB
   - `web.filter` - contains authentication filter

2. `resources` package:
   - script for database to create required schema and tables

3. `webapp` package:
    - `WEB-INF` folder: contains all JSP pages for application
    - `web.xml` - settings for web application

### <span style="vertical-align: sub"><img src="src/main/resources/technologies.png"></span> Technologies:

- `Maven`
- `JSP`
- `JDBC API`
- `JSTL`
- `Servlet API`
- `MySQL`
- `Tomcat`

### <span style="vertical-align: sub"><img src="src/main/resources/run.png"></span> Instructions to run the project

- Install IDE to your PC
- Clone the project to your IDE (e.g. IntelliJ IDEA)
- Install MySQL to your PC and new create MySQL connection
- Copy script from `init_db.sql` in `resources` folder
- Execute script in your MySQL connection
- Change parameters: `USERNAME`, `PASSWORD` in `ConnectionUtil` class for yours (they should match `username` and `password` from your MySQL connection)
- Download Tomcat and add configuration in your IDE (for this project `v9.0.50` was used)
- Run project with Tomcat
