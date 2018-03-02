# Bookstore API

Express and MongoDB REST API for managing books and genres.

## About

This is a compact CRUD service built with classic Express patterns. The server exposes book and genre endpoints backed by Mongoose models and is intended as a small portfolio sample for a Node.js API.

## Key Features

- CRUD endpoints for books and genres
- JSON request/response handling
- Mongoose-backed persistence
- Single-file Express bootstrap

## Architecture

- `app.js` wires Express, body parsing, Mongoose, and all routes
- `models/book` and `models/genre` are imported by the server entry point
- The API is served on port `3000`

## Tech Stack

- Node.js
- Express
- Mongoose
- body-parser

## Prerequisites

- Node.js
- MongoDB running locally

## Installation

1. Install dependencies in the repository root.
2. Start MongoDB locally.

## Configuration

- The current code connects to `mongodb://localhost/bookstore` directly in `app.js`

## How to Run

```bash
npm install
node app.js
```

## Example Usage

- `GET /api/books`
- `POST /api/books`
- `GET /api/genres`
- `POST /api/genres`

## Project Structure

- `app.js` - Express bootstrap and route definitions
- `package.json` - dependency manifest and metadata

## Current Status

Partially implemented. The server entry point references `./models/book` and `./models/genre`, but those files are not present in the workspace snapshot.

## Limitations

- No automated tests
- No environment variable support
- Missing model files make the repo incomplete as-is

## License

No explicit license file was found.
