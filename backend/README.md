# User Management System Backend

A robust backend system for managing users, employees, departments, and workflows. This system provides a RESTful API with comprehensive features for user authentication, employee management, department organization, and workflow automation.

## Project Overview

The User Management System is a comprehensive solution designed to streamline organizational operations through efficient user and resource management. This backend system serves as the core engine that powers various administrative and operational functions.

### Key Components

1. **User Management**
   - Secure authentication and authorization system
   - Role-based access control
   - User profile management
   - Session handling and security

2. **Employee Management**
   - Complete employee lifecycle management
   - Employee profile tracking
   - Performance monitoring
   - Department assignment and role management

3. **Department Management**
   - Hierarchical department structure
   - Department resource allocation
   - Inter-department communication channels
   - Department performance metrics

4. **Workflow Automation**
   - Customizable workflow templates
   - Automated approval processes
   - Task assignment and tracking
   - Status monitoring and notifications

5. **Request Processing**
   - Streamlined request submission
   - Multi-level approval workflows
   - Request tracking and history
   - Automated notifications

### System Architecture

The system is built using a modern tech stack that ensures scalability, security, and maintainability:

- **API Layer**: RESTful API architecture with comprehensive documentation
- **Authentication**: JWT-based secure authentication system
- **Database**: Flexible database support (PostgreSQL/MySQL) with Sequelize ORM
- **Real-time Features**: Socket.IO integration for live updates
- **Documentation**: Swagger UI for interactive API documentation
- **Security**: Multiple layers of security including input validation and error handling

### Integration Capabilities

The system is designed to be easily integrated with:
- Frontend applications
- Third-party services
- External authentication providers
- Email notification systems
- Reporting and analytics tools

## Features

- User Authentication and Authorization
- Employee Management
- Department Management
- Workflow Management
- Request Processing
- API Documentation with Swagger
- Real-time Updates with Socket.IO
- Email Notifications
- Database Integration with Sequelize ORM

## Tech Stack

- Node.js
- Express.js
- Sequelize ORM
- PostgreSQL
- MySQL
- Socket.IO
- JWT Authentication
- Swagger UI
- Nodemailer

## Prerequisites

- Node.js (v12 or higher)
- PostgreSQL or MySQL database
- npm or yarn package manager

## Installation

1. Clone the repository:
```bash
git clone: https://github.com/PolandDiosana/user-management-system/tree/Nabua-frontend-signup-auth
cd user-management-system/backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
# Development mode
npm run dev

# Production mode
npm start
```

## API Documentation

The API documentation is available at `/api-docs` when the server is running. It provides detailed information about all available endpoints, request/response formats, and authentication requirements.

## Project Structure

```
├── accounts/           # User account management
├── employees/          # Employee management
├── departments/        # Department management
├── workflows/          # Workflow management
├── requests/           # Request processing
├── _middleware/        # Middleware functions
├── _helpers/           # Helper utilities
├── config.json         # Configuration file
├── server.js          # Main application file
└── swagger.yaml       # API documentation
```

## API Endpoints

### Authentication
- POST /accounts/authenticate
- POST /accounts/register
- GET /accounts/current
- PUT /accounts/current
- GET /accounts/:id

### Employees
- GET /employees
- POST /employees
- GET /employees/:id
- PUT /employees/:id
- DELETE /employees/:id

### Departments
- GET /departments
- POST /departments
- GET /departments/:id
- PUT /departments/:id
- DELETE /departments/:id

### Workflows
- GET /workflows
- POST /workflows
- GET /workflows/:id
- PUT /workflows/:id
- DELETE /workflows/:id

### Requests
- GET /requests
- POST /requests
- GET /requests/:id
- PUT /requests/:id
- DELETE /requests/:id

## Security

- JWT-based authentication
- Password hashing with bcrypt
- CORS enabled
- Input validation with Joi
- Error handling middleware

## Development

The project uses nodemon for development, which automatically restarts the server when changes are detected. To start the development server:

```bash
npm run dev
```

## Production

For production deployment:

1. Set NODE_ENV to production
2. Configure appropriate environment variables
3. Start the server using:
```bash
npm start
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License. 