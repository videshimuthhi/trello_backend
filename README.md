# Trello Backend

A backend service for a Trello-like task management application.

## Overview

This project provides the server-side implementation for a task management and collaboration tool inspired by Trello. It handles user authentication, board management, card organization, and real-time updates.

## Features

- User authentication and authorization
- Board creation and management
- Card and task management
- List organization
- Collaboration features
- Real-time updates

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager
- MongoDB or your configured database

### Installation

1. Clone the repository:
```bash
git clone https://github.com/videshimuthhi/trello_backend.git
cd trello_backend
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env` file in the root directory with the following variables:
```
PORT=5000
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
NODE_ENV=development
```

4. Start the development server:
```bash
npm run dev
```

## Project Structure

```
trello_backend/
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   └── utils/
├── tests/
├── .env
├── .gitignore
├── package.json
└── README.md
```

## API Endpoints

### Users
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/users/:id` - Get user profile

### Boards
- `GET /api/boards` - Get all boards
- `POST /api/boards` - Create a new board
- `GET /api/boards/:id` - Get board details
- `PUT /api/boards/:id` - Update board
- `DELETE /api/boards/:id` - Delete board

### Cards
- `GET /api/cards` - Get all cards
- `POST /api/cards` - Create a new card
- `PUT /api/cards/:id` - Update card
- `DELETE /api/cards/:id` - Delete card

## Development

### Running Tests

```bash
npm test
```

### Code Style

This project uses ESLint and Prettier for code formatting. Run:

```bash
npm run lint
npm run format
```

## Building for Production

```bash
npm run build
npm start
```

## Technologies Used

- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **JWT** - Authentication
- **Mongoose** - MongoDB ODM

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, email support@example.com or open an issue in the repository.

## Changelog

All notable changes to this project are documented in the [CHANGELOG.md](./CHANGELOG.md) file.
