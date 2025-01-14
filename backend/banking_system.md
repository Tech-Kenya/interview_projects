**Backend Technical Challenge: Banking System**

**Background**

The Banking System project is designed to assess your backend development skills and your ability to work with modern tools, frameworks, and best practices. This challenge simulates a simple banking API with a focus on clean architecture and modular design.

Most of our backend services are implemented with the following stack:

- REST APIs built with **Node.js** and **Express.js**.
- PostgreSQL is our preferred database for relational data storage.
- Deployment on containerized environments using **Docker** and orchestrated via **Kubernetes**.
- CI/CD pipelines using GitHub Actions or any modern CI/CD platform.
- Authentication and authorization mechanisms leveraging **JWT** or OpenID Connect.

The technical interview will be based on a coding assignment to evaluate your proficiency in:

- Developing RESTful APIs.
- Working with relational databases and writing optimized SQL queries.
- Designing modular and scalable architectures.
- Writing comprehensive unit tests with high code coverage.
- Integrating CI/CD pipelines.
- Deploying applications to a cloud-based platform (e.g., DigitalOcean, AWS, GCP).

We will focus on:

- API design and HTTP principles.
- Security best practices (e.g., input validation, secure authentication).
- Logical and efficient code flow.
- Database schema design.
- Version control practices.

---

**Screening Test**

Your task is to create a simple **Banking System API**. Follow the steps below:

1. **Set up the environment:**
   - Use **Node.js** with **Express.js** for the backend.
   - Use **PostgreSQL** as the database.
   - Write a `.env` file to manage environment variables for database credentials and JWT secrets.

2. **Design and implement the following database schema:**
   - **Employees:** Fields for ID, name, email, password (hashed), role, and timestamps.
   - **Customers:** Fields for ID, name, email, account balance, and timestamps.
   - **Transactions:** Fields for ID, customer_id, transaction_type (deposit/withdrawal), amount, and timestamps.

3. **Implement the following RESTful APIs:**
   - **Employee Management:**
     - Register an employee (`POST /api/employees/register`).
     - Login as an employee (`POST /api/employees/login`).
   - **Customer Management:**
     - Add a new customer (`POST /api/customers`).
     - Fetch a paginated list of customers (`GET /api/customers` with optional query params for sorting and filtering).
   - **Transaction Management:**
     - Deposit money to a customer account (`POST /api/transactions/deposit`).
     - Withdraw money from a customer account (`POST /api/transactions/withdraw`).

4. **Authentication & Authorization:**
   - Use **JWT** for securing routes.
   - Restrict certain actions to employees with specific roles (e.g., only admins can delete customers).

5. **Testing:**
   - Write **unit tests** and **integration tests** to achieve at least 80% code coverage.
   - Include tests for edge cases like invalid inputs and unauthorized access.

6. **CI/CD Pipeline:**
   - Set up GitHub Actions to:
     - Run the test suite on every push.
     - Lint the codebase using **ESLint**.
     - Deploy the application automatically to a PAAS/FAAS/IAAS of your choice (e.g., DigitalOcean, AWS).

7. **Deployment:**
   - Deploy the application using **Docker** and provide a `Dockerfile` and `docker-compose.yml` for local testing.
   - Host the application on a public platform and include the live link in your submission.

8. **Documentation:**
   - Write a clear and detailed `README.md` file explaining how to set up, test, and use the application.

---

**Submission Guidelines**

- Push your code to a **public GitHub repository**.
- Ensure your repository contains:
  - Well-organized folder structure.
  - `.env.example` file for environment variable references.
  - Test reports and CI/CD configuration.
- Include a live demo link (if deployed).
- Submit the repository link to us before the deadline.

---

**Evaluation Criteria**

We will assess the following:

1. **API Functionality:**
   - Correctness of endpoints.
   - Adherence to RESTful principles.
2. **Code Quality:**
   - Modular, clean, and well-documented code.
   - Use of modern JavaScript (ES6+).
3. **Testing:**
   - Coverage and quality of unit and integration tests.
4. **Database Design:**
   - Normalized schema and optimized queries.
5. **Security:**
   - Proper handling of sensitive data (e.g., hashing passwords).
   - Validation and sanitization of inputs.
6. **CI/CD:**
   - Automated testing, linting, and deployment.
7. **Documentation:**
   - Clear setup instructions and usage examples.

---