# NextAI Frontend

A modern React application that provides an interactive interface for PDF document analysis and Q&A interactions. This frontend is part of the NextAI project, working in conjunction with a backend service to provide AI-powered document analysis capabilities.

## Features

- PDF document upload and processing
- Interactive chat interface for document Q&A
- Speech-to-text capabilities
- Text-to-speech responses
- Modern UI with Ant Design components
- Docker support for easy deployment

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Docker (optional, for containerized deployment)

## Local Development Setup

1. Clone the repository:
```bash
git clone https://github.com/Andrlulu/nextAI_frontend.git
cd nextAI_frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory:
```bash
REACT_APP_DOMAIN=http://localhost:5001
```

4. Start the development server:
```bash
npm start
```

The application will be available at `http://localhost:3000`

## Docker Setup

1. Build and run using docker-compose:
```bash
docker-compose up --build
```

2. Or build and run individually:
```bash
# Build the image
docker build -t nextai-frontend .

# Run the container
docker run -p 3000:3000 nextai-frontend
```

## Environment Variables

- `REACT_APP_DOMAIN`: The URL of the backend service (default: http://localhost:5001)

## Project Structure

```
nextai_frontend/
├── public/                 # Static files
├── src/
│   ├── components/        # React components
│   │   ├── ChatComponent.js
│   │   ├── PdfUploader.js
│   │   └── RenderQA.js
│   ├── App.js            # Main application component
│   └── index.js          # Application entry point
├── Dockerfile            # Docker configuration
├── docker-compose.yml    # Docker Compose configuration
└── package.json         # Project dependencies and scripts
```

## Available Scripts

- `npm start`: Runs the app in development mode
- `npm test`: Launches the test runner
- `npm run build`: Builds the app for production
- `npm run eject`: Ejects from Create React App

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
