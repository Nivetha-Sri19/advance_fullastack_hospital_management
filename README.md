# Advanced Hospital Management System 

A backend-focused Hospital Management System developed using **FastAPI** with advanced backend engineering concepts including JWT Authentication, Role-Based Access Control (RBAC), Appointment Management, Background Tasks, File Handling, Pagination, Search & Filtering, and Unit Testing.

---

# 🚀 Tech Stack

- Python
- FastAPI
- SQLAlchemy
- SQLite
- JWT Authentication
- Passlib (bcrypt)
- Pydantic
- Pytest
- Uvicorn

---

# 📁 Project Structure

```bash
backend/
│
├── models/
├── routers/
├── schemas/
├── services/
├── tests/
├── uploads/
├── utils/
│
├── config.py
├── database.py
├── hospital.db
├── hospital.log
├── main.py
├── requirements.txt

Features Implemented
🔐 Authentication System


JWT Authentication


Secure Login & Registration


Password Hashing using bcrypt


Token Validation


Forgot Password Functionality



👥 Role-Based Access Control (RBAC)
Supported Roles:


Admin


Doctor


Patient


Access Control


Admin can manage all users and appointments


Doctor can manage assigned appointments


Patient can book and view appointments



📅 Appointment Management
Features


Appointment Booking


Appointment Approval/Rejection


Appointment Completion


Status Handling:


Pending


Approved


Rejected


Completed




Validations


Prevent Double Booking


Validate Appointment Slots


Doctor Availability Checking



🔍 Search & Filtering
Doctor Search


Search by Name


Search by Specialization


Appointment Filtering


Filter by:


Date


Status


User





📄 Pagination & Sorting
Implemented for listing APIs:


Page Number


Limit


Sorting


Ascending / Descending order


Example:
GET /doctors?page=1&limit=10&sort_by=name

⚙️ Service Layer Architecture
The application follows clean architecture principles by separating:


Routers


Models


Schemas


Services


Utilities


Business logic is handled inside the service layer for better maintainability and scalability.

📁 File Handling
Implemented:


File Upload Support


File Type Validation


File Size Validation


File Metadata Storage



⚡ Background Tasks
Implemented using FastAPI BackgroundTasks.
Examples:


Notification handling


Logging operations


Async processing



📦 API Response Standardization
Example Success Response:
{  "success": true,  "message": "Operation successful",  "data": {}}
Example Error Response:
{  "success": false,  "message": "Validation failed",  "error": {}}

❌ Global Exception Handling
Implemented centralized exception handling for:


Authentication Errors


Validation Errors


Database Errors


File Upload Errors



🧪 Unit Testing
Basic API testing implemented using pytest.
Covered Modules:


Authentication APIs


Appointment APIs


Validation Testing


Run Tests:
pytest

⚙️ Installation & Setup
1️⃣ Clone Repository
git clone <repository-url>

2️⃣ Navigate to Backend
cd backend

3️⃣ Create Virtual Environment
Windows
python -m venv venvvenv\Scripts\activate
Linux / Mac
python3 -m venv venvsource venv/bin/activate

4️⃣ Install Dependencies
pip install -r requirements.txt

5️⃣ Run Application
uvicorn main:app --reload
Application will run on:
http://127.0.0.1:8000

📘 API Documentation
Swagger UI:
http://127.0.0.1:8000/docs
ReDoc:
http://127.0.0.1:8000/redoc

🔑 Main API Endpoints
Authentication
MethodEndpointDescriptionPOST/auth/registerRegister UserPOST/auth/loginLoginPOST/auth/forgot-passwordForgot Password

Doctors
MethodEndpointGET/doctorsPOST/doctors

Appointments
MethodEndpointPOST/appointmentsGET/appointmentsPUT/appointments/{id}

🔒 Security Features


JWT Authentication


Password Hashing


Protected APIs


Role-Based Authorization


Input Validation


File Validation



🎯 Assignment Objectives Covered
✅ Advanced Authentication
✅ RBAC
✅ Appointment Management
✅ Search & Filtering
✅ Pagination & Sorting
✅ Service Layer Architecture
✅ File Handling
✅ Background Tasks
✅ API Standardization
✅ Exception Handling
✅ Unit Testing

For accessing access with username: Nivetha and password:Nivetha@123


















