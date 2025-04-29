# Live Streaming Platform

A modern live streaming platform built with a microservice architecture, enabling users to create, manage, and watch live streams.

## Project Overview

This application consists of three main components:

1. **REST API Server**: A JSON-based API for stream management
2. **RTMP Server**: Handles real-time multimedia protocol for live video streaming
3. **Client Application**: Frontend interface for users to interact with the platform (currently in development)

## Tech Stack

### API Server

- Node.js
- JSON Server for RESTful API endpoints
- Stores stream metadata including titles, descriptions, and user IDs

### RTMP Server

- Node.js
- Node Media Server for handling RTMP protocol
- Configured for optimal streaming performance with properly tuned chunk sizes and caching

## Features

- **Stream Management**: Create, read, update, and delete stream information
- **Live Video Streaming**: Real-time video broadcasting via RTMP protocol
- **RESTful API**: Clean API design for integrating with frontend applications

## Architecture

The application follows a microservice architecture pattern:

- The API server runs on port 3001 and manages stream metadata
- The RTMP server operates on port 1935 (RTMP) and 8000 (HTTP) for video streaming
- Services are decoupled for better maintainability and scalability

## Getting Started

### Prerequisites

- Node.js (v12+)
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies for each service:

```bash
# API Server
cd api
npm install

# RTMP Server
cd ../rtmpserver
npm install
```

### Running the Services

1. Start the API server:

```bash
cd api
npm start
```

2. Start the RTMP server:

```bash
cd rtmpserver
npm start
```

## Future Development

- Complete frontend client implementation with React
- Add user authentication and authorization
- Implement chat functionality for live streams
- Add stream analytics and monitoring

## License

ISC
