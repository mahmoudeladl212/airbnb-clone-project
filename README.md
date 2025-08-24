# airbnb-clone-project
Backend Developer – Implements server-side logic, API endpoints, and business rules.

Database Administrator (DBA) – Designs, optimizes, and maintains the relational database structure.

Frontend Developer – (Optional scope) Designs and develops the user interface for interacting with the backend.

DevOps Engineer – Manages CI/CD integration, Docker containerization, and deployment pipelines.

Security Engineer – Implements authentication, authorization, encryption, and threat protections.

Project Manager / Scrum Master – Ensures team collaboration, task organization, and timely delivery.
## Database Design
Users: id, name, email, role, password_hash.

Properties: id, owner_id (FK → Users), title, description, location, price.

Bookings: id, property_id (FK), user_id (FK), start_date, end_date, status.

Reviews: id, user_id (FK), property_id (FK), rating, comment, created_at.

Payments: id, booking_id (FK), amount, payment_status, timestamp.

Describe relationships:

A User can own multiple Properties.

A User can make multiple Bookings.

A Property can have many Reviews.

A Booking is linked to one Payment.
## Feature Breakdown
User Management: Sign-up, login, profile management, authorization.

Property Management: Host can list, edit, or delete their properties.

Booking System: Users can search, book properties, and manage reservations.

Reviews and Ratings: Guests can leave feedback on properties.

Payments: Secure system for booking payment confirmation.

Search & Filter: Browse properties by date, location, and price.
## API Security
Document measures:

Authentication: Secure login with JWT/OAuth2.

Authorization: Role-based access (e.g., host vs guest).

Data Encryption: HTTPS / SSL to protect sensitive info.

Rate Limiting: Prevent brute force and DDoS attacks.

Input Validation & Sanitization: Prevent SQL injection / XSS.


