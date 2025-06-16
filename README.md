# 🏠 Airbnb Clone Project

Welcome to the **Airbnb Clone Project**, a full-stack web development project inspired by the popular Airbnb platform. This project is developed as part of the ALX Software Engineering Program to reinforce essential skills in backend development, web frameworks, database management, security, and collaboration.

---

## 🎯 Project Goals

- Build a functional Airbnb-like platform from scratch.
- Implement clean, modular, and scalable backend services.
- Use a relational database to handle dynamic data.
- Design and deploy RESTful APIs.
- Collaborate using Git and GitHub.
- Learn and apply CI/CD and API security best practices.

---

## 👨‍💻 Team Roles

### Backend Developer
Responsible for implementing the application’s server-side logic, setting up API endpoints, and integrating with the database.

### Frontend Developer
Creates responsive user interfaces and ensures a smooth user experience using HTML, CSS, and JavaScript frameworks.

### Database Administrator (DBA)
Designs, manages, and optimizes the database schema and queries to ensure fast and secure data operations.

### DevOps Engineer
Handles deployment, CI/CD pipeline automation, server configurations, and monitoring of application performance.

### QA Engineer
Develops test plans and writes automated and manual tests to ensure software quality and reliability.

---

## 🧰 Technology Stack

| Technology      | Purpose |
|----------------|---------|
| **Python**     | Main programming language for backend logic. |
| **Flask**      | Lightweight web framework used to build RESTful APIs. |
| **MySQL**      | Relational database used to store and manage application data. |
| **HTML/CSS**   | Used to build and style frontend templates. |
| **Jinja2**     | Templating engine for rendering dynamic content in HTML. |
| **Git & GitHub** | Version control and collaboration. |
| **Docker**     | Containerization for development, testing, and deployment. |
| **GitHub Actions** | Automates testing, building, and deployment through CI/CD pipelines. |

---

## 🗃️ Database Design

### 🔑 Entities and Their Key Fields

1. **User**
   - `id` (primary key)
   - `username`
   - `email`
   - `password_hash`
   - `role` (host or guest)

2. **Property**
   - `id`
   - `user_id` (foreign key)
   - `title`
   - `description`
   - `location`

3. **Booking**
   - `id`
   - `user_id`
   - `property_id`
   - `start_date`
   - `end_date`

4. **Review**
   - `id`
   - `user_id`
   - `property_id`
   - `rating`
   - `comment`

5. **Payment**
   - `id`
   - `booking_id`
   - `amount`
   - `status`
   - `payment_date`

### 🧩 Relationships
- A **User** can own multiple **Properties**.
- A **Booking** is made by a **User** for a **Property**.
- A **Review** belongs to both a **User** and a **Property**.
- A **Payment** is linked to a **Booking**.

---

## 🔍 Feature Breakdown

### 1. User Management
Handles registration, login, authentication, and profile management for guests and hosts.

### 2. Property Management
Hosts can create, update, and delete property listings with details like images, descriptions, and availability.

### 3. Booking System
Users can search for properties and book available dates. The system checks for conflicts and stores bookings.

### 4. Review System
Guests can leave ratings and feedback after completing their stay, which helps maintain platform quality.

### 5. Payment Integration
Handles secure processing of payments for bookings, with payment status updates and receipt generation.

### 6. Admin Dashboard (Optional)
Admin users can monitor platform activity, manage users, and moderate content.

---

## 🔐 API Security

### Key Security Measures

- **Authentication**: Verifies user identity using JWT or session-based login systems.
- **Authorization**: Restricts access to specific endpoints based on user roles (guest/host/admin).
- **Input Validation**: Sanitizes all incoming data to prevent injection attacks.
- **Rate Limiting**: Protects endpoints from abuse by limiting the number of requests per user/IP.
- **HTTPS & Secure Headers**: Ensures encrypted communication and adds headers to guard against XSS/CSRF.

### Why Security Matters

- **User Data Protection**: Safeguards sensitive user information like passwords and personal details.
- **Booking & Payment Security**: Prevents unauthorized transactions or data breaches.
- **Platform Integrity**: Ensures only legitimate users and activities occur on the system.

---

## 🔁 CI/CD Pipeline

### What is CI/CD?

**CI/CD (Continuous Integration and Continuous Deployment)** automates the software delivery process. It ensures that changes to code are tested and deployed quickly, reliably, and safely.

### Why It's Important

- Automates testing and deployment.
- Reduces bugs by catching issues early.
- Speeds up delivery and feedback loops.

### Tools Used

- **GitHub Actions**: Automates testing and builds after every push.
- **Docker**: Provides consistent development and production environments.
- **Fabric**: Used for automated deployment scripts.

---

## 👥 Contributors

- Vision Chauke (Web Development, Backend Developer in training)

---

## 📜 License

This project is licensed for educational and development purposes only. Developed as part of the ALX Software Engineering Program.

