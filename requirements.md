# AirBnB Clone - Technical Requirements Specification

## 1. User Authentication System

### Functional Requirements
- Users can register with email/password
- Users can log in and receive JWT tokens
- Password reset functionality
- Role-based access control (guest/host/admin)

### API Endpoints
| Method | Endpoint           | Description                     |
|--------|--------------------|---------------------------------|
| POST   | /api/auth/register | Register new user               |
| POST   | /api/auth/login    | Authenticate user               |
| POST   | /api/auth/forgot   | Initiate password reset         |

### Request/Response Examples
**Registration Request:**
```json
{
  "email": "user@example.com",
  "password": "SecurePass123!",
  "role": "host"
}
