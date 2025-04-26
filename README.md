# Build Night #1

## Participant Information
- Name: Gabriel Andres Faundez Soto
- GitHub: https://github.com/FarDust
- LinkedIn: https://www.linkedin.com/in/gnfaundez/

Welcome to Build Night #1! This repository has been created for you to work on your project.

## 🚀 Project Overview

This project combines two powerful tools for astronomical anomaly detection:

1. **Anomaly Reaper**: A Python-based backend for detecting anomalies in astronomical images using PCA
2. **Void Scanner**: A Next.js web application that provides an intuitive interface for reviewing detected anomalies

Together, they form a complete system for processing, analyzing, and reviewing astronomical image data to discover unusual patterns or phenomena.

## 🌌 Anomaly Reaper

Anomaly Reaper is a specialized tool for detecting unusual patterns and anomalies in astronomical imagery data, particularly from TESS (Transiting Exoplanet Survey Satellite).

### Key Features

- 🖼️ Process FITS astronomical image files from TESS missions
- 🔄 Generate embeddings from image data using Google Vertex AI
- 📊 Reduce dimensionality with PCA and detect outliers
- 🚀 API interface for uploading and processing new images
- 📊 Interactive visualization of detected anomalies

### Technology Stack

- **Backend:** Python, FastAPI, SQLAlchemy
- **Machine Learning:** Google Vertex AI embeddings, scikit-learn
- **Image Processing:** Astropy, scikit-image, PIL

### Quick Start

```bash
# Navigate to the anomaly-reaper directory
cd anomaly-reaper

# Install dependencies with UV
uv --group dev --group test sync

# Run the application
anomaly-reaper-api --port 8080
```

The API will be available at http://localhost:8080.

## 🔭 Void Scanner

Void Scanner is a modern web application designed to help astronomers and researchers analyze and classify astronomical images with an intuitive interface.

### Key Features

- 🔭 **Anomaly Detection**: Automatic identification of unusual patterns in astronomical images
- 🌌 **Tinder-style Interface**: Quick and intuitive image review and classification
- 🧠 **User Feedback Collection**: Aggregates expert insights to improve machine learning models
- 📊 **Statistics Dashboard**: Track system performance and anomaly distributions
- 🎮 **Demo Mode**: Practice with sample anomalies before working with real data

### Technology Stack

- **Next.js**: React framework with server-side rendering and routing
- **TypeScript**: For type safety and better developer experience
- **Tailwind CSS**: For responsive and customizable UI components

### Quick Start

```bash
# Navigate to the void-scanner directory
cd void-scanner

# Install dependencies
npm install

# Start the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 🔄 System Integration

To use both components together:

1. Start the Anomaly Reaper backend first
2. Configure Void Scanner to connect to the Anomaly Reaper API
3. Use Void Scanner's interface to review and classify anomalies detected by Anomaly Reaper

## 📋 Project Structure

```
.
├── README.md
├── anomaly-reaper/        # Python-based anomaly detection backend
│   ├── data/              # Sample data and models
│   ├── migrations/        # Database migration scripts
│   ├── models/            # Trained machine learning models
│   ├── src/               # Source code
│   └── tests/             # Unit and integration tests
└── void-scanner/          # Next.js web application frontend
    ├── public/            # Static assets
    └── src/               # Source code
        ├── app/           # Next.js app directory
        ├── components/    # React components
        └── services/      # API service layer
```

## 📄 License

Both projects are licensed under the MIT License.

---

*Building tools for astronomical discovery and anomaly detection*
