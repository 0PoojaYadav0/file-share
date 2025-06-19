# file-share
A full-stack file management application using Node.js and Express.js, enabling users to securely store, organize, and access digital assets through an intuitive interface accessible across devices.
# File Share

File Share is a web application that allows users to create accounts, upload files, and organize them into folders. It provides a secure environment for storing and managing your files online.

## Features

- **User Authentication**
  - Secure signup and login system
  - Password encryption
  - Session management

- **File Management**
  - Upload files
  - Create folders for organization
  - Delete folders
  - Browse your files and folders

- **User Interface**
  - Clean and responsive design
  - Easy navigation
  - Mobile-friendly layout

## Technologies Used

- **Backend**
  - Node.js
  - Express.js
  - Passport.js (authentication)
  - Multer (file uploads)
  - bcryptjs (password hashing)

- **Frontend**
  - EJS (templating)
  - TailwindCSS
  - JavaScript

- **Database**
  - PostgreSQL
  - Prisma ORM

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/file-share.git
   cd file-share
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory with the following:
   ```
   DATABASE_URL="postgresql://username:password@localhost:5432/fileshare"
   SESSION_SECRET="your_session_secret"
   PORT=3000
   ```

4. **Set up the database**
   ```bash
   npx prisma migrate dev
   ```

5. **Generate Tailwind CSS**
   ```bash
   npx tailwindcss -i ./public/main.css -o ./public/output.css
   ```

6. **Start the server**
   ```bash
   node app.js
   ```

7. **Access the application**
   Open your browser and navigate to `http://localhost:3000`

## Usage

1. **Create an account**
   - Navigate to the signup page
   - Enter your first name, last name, username, and password
   - Click "Sign up"

2. **Login to your account**
   - Enter your username and password
   - Click "Login"

3. **Manage folders**
   - Create new folders from the dashboard
   - View your existing folders
   - Delete folders when needed

4. **Upload files**
   - Use the "New file upload" button to add files
   - Upload entire folders using "New folder upload"

## Project Structure

```
file-share/
├── controllers/       # Application controllers
├── prisma/            # Database schema and migrations
├── public/            # Static assets
├── routes/            # Express routes
├── views/             # EJS templates
│   └── partials/      # Reusable template components
├── app.js             # Main application entry point
└── package.json       # Project dependencies
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.