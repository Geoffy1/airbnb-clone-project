# airbnb-clone-project
# Airbnb Clone Project (Back-End)

## 🚀 Project Overview
This project simulates the backend infrastructure of a real-world Airbnb-style booking platform. It handles user authentication, property listings, bookings, payments, and reviews.

## 🏆 Project Goals
- **User Management:** Secure registration, login, and profile management.
- **Property Management:** CRUD for property listings.
- **Booking System:** Reservation and booking management.
- **Payment Processing:** Secure and traceable transactions.
- **Review System:** Allow users to leave property reviews.
- **Data Optimization:** Indexing and caching for performance.

## ⚙️ Technology Stack
- Django
- Django REST Framework
- PostgreSQL
- GraphQL
- Celery
- Redis
- Docker
- GitHub Actions (CI/CD)

## 👥 Team Roles

- **Backend Developer:** Implements API endpoints, models, and business logic.
- **Database Administrator (DBA):** Designs and maintains efficient database schemas.
- **DevOps Engineer:** Automates deployment, manages environments, and monitors uptime.
- **QA Engineer:** Tests APIs, ensures features meet requirements, and reports bugs.

## 🛠️ Technology Stack

- **Django:** Main web framework for backend logic.
- **Django REST Framework:** Toolset for creating RESTful APIs.
- **PostgreSQL:** Relational DB for storing app data.
- **GraphQL:** Flexible data querying language.
- **Celery:** Handles async tasks like sending notifications.
- **Redis:** In-memory store used for caching and Celery broker.
- **Docker:** Containerization for consistent development environments.
- **GitHub Actions:** Automates testing and deployment workflows.

## 🗃️ Database Design

### Entities:
1. **Users**
   - id, username, email, password_hash, is_host
2. **Properties**
   - id, owner_id, name, location, price, description
3. **Bookings**
   - id, user_id, property_id, start_date, end_date
4. **Payments**
   - id, booking_id, amount, status, payment_date
5. **Reviews**
   - id, user_id, property_id, rating, comment

### Relationships:
- A **User** can have many **Properties**.
- A **Booking** belongs to both a **User** and a **Property**.
- A **Payment** is linked to a **Booking**.
- A **Review** is left by a **User** for a **Property**.

## ✨ Feature Breakdown

### User Management
Users can register, log in, and manage their profile securely.

### Property Management
Hosts can create, update, and delete property listings.

### Booking System
Users can view availability and make property reservations.

### Payment Processing
Payments are securely processed and linked to bookings.

### Review System
Users can leave and manage feedback for properties they’ve booked.
