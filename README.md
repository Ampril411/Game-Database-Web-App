This is a JSP + Servlet-based web application. It connects to a MySQL database and allows users to view, search, and update game-related data.

## 📦 Project Structure

- `src/java/` – Java source files:
  - `model/` – Java classes for database tables
  - `dal/` – DAO classes for database access
  - `servlet/` – Servlets handling web requests
- `src/webapp/` – JSP pages and frontend files
  - `WEB-INF/` – `web.xml` deployment descriptor
  - `lib/` – required libraries (MySQL driver, JSTL)
- `Driver.java` – Java class to create tables and insert sample data

## 🚀 How to Run Locally

1. **Install MySQL** and create your schema.
2. **Edit `ConnectionManager.java`** to update your DB credentials.
3. Run `Driver.java` once to populate the database with sample data.
4. **Deploy project to Tomcat:**
   - Use IntelliJ IDEA or Eclipse
   - Or export `.war` file and place it in `tomcat/webapps/`
5. Access the app in browser at:
   ```
   http://localhost:8080/yourAppName/
   ```

## 💡 Features Implemented

- Filterable list-based report with partial match
- Detail report using joins across 3+ tables
- Update functionality on at least one table
- PreparedStatements for SQL injection protection

## 📚 Technologies Used

- Java (JSP & Servlets)
- MySQL
- Apache Tomcat
- JSTL + JDBC
