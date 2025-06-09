# Quantum Forge

A modern Node.js web application built with Express.js and EJS templating engine.

## 🚀 Features

- **Express.js** - Fast, unopinionated web framework for Node.js
- **EJS Templates** - Embedded JavaScript templating
- **Static File Serving** - Serve CSS, JavaScript, and image files
- **Environment Configuration** - Dotenv for environment variables
- **Development Hot Reload** - Nodemon for automatic server restarts
- **Modular Architecture** - Organized codebase with separate routing and app logic

## 📁 Project Structure

```
quantum-forge/
├── app/
│   └── app.js          # Main Express application setup
├── public/             # Static assets (CSS, JS, images)
├── router/             # Route definitions
├── views/              # EJS templates
├── .env                # Environment variables
├── .gitignore          # Git ignore rules
├── index.js            # Server entry point
├── package.json        # Project dependencies and scripts
└── README.md           # Project documentation
```

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/wilsb8/quantum-forge.git
   cd quantum-forge
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env` file in the root directory:
   ```env
   PORT=3000
   ```

## 🚀 Usage

### Development Mode
Run with automatic restarts on file changes:
```bash
npm run dev
```

### Production Mode
Run the application:
```bash
npm start
```

The server will start and listen on the port specified in your `.env` file (default: 3000).

Access the application at: `http://localhost:3000`

## 📋 Available Scripts

- `npm start` - Start the production server
- `npm run dev` - Start the development server with nodemon
- `npm test` - Run tests (currently not implemented)

## 🔧 Configuration

### Environment Variables

| Variable | Description | Default |
|----------|-------------|----------|
| `PORT` | Server port number | 3000 |

### View Engine

The application uses EJS as the templating engine. Templates are stored in the `views/` directory.

### Static Files

Static assets (CSS, JavaScript, images) are served from the `public/` directory.

## 🏗️ Architecture

### Application Setup (`app/app.js`)
- Configures Express application
- Sets up EJS as view engine
- Configures static file serving
- Sets up middleware for request parsing
- Integrates routing

### Server Entry Point (`index.js`)
- Loads environment configuration
- Creates HTTP server
- Starts listening on specified port

### Routing
- Routes are organized in the `router/` directory
- Modular approach for maintainable code

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- **Repository:** [https://github.com/wilsb8/quantum-forge](https://github.com/wilsb8/quantum-forge)
- **Issues:** [https://github.com/wilsb8/quantum-forge/issues](https://github.com/wilsb8/quantum-forge/issues)

## 📊 Dependencies

### Production Dependencies
- **express** (^5.1.0) - Web application framework
- **ejs** (^3.1.10) - Embedded JavaScript templates
- **dotenv** (^16.5.0) - Loads environment variables from .env file
- **path** (^0.12.7) - Utilities for working with file and directory paths

### Development Dependencies
- **nodemon** (^3.1.10) - Monitor for changes and automatically restart server

---

**Built with ❤️ using Node.js and Express.js**
