# Faleproxy
[![Faleproxy CI](https://github.com/hileamlakB/faleproxy/actions/workflows/ci.yml/badge.svg)](https://github.com/hileamlakB/faleproxy/actions/workflows/ci.yml)

A Node.js web application that fetches a URL, replaces every instance of "Yale" with "Fale" in the document, and displays the modified content.

## Features

- Simple and intuitive user interface
- Fetches web content from any URL
- Replaces all instances of "Yale" with "Fale" (case-insensitive)
- Displays the modified content in an iframe
- Shows original URL and page title in an info bar

## Installation

1. Clone this repository
2. Navigate to the project directory
3. Install dependencies:

```bash
npm install
```

## Usage

1. Start the server:

```bash
npm start
```

2. Open a browser and go to `http://localhost:3001`
3. Enter a URL in the input field (e.g., https://www.yale.edu)
4. Click "Fetch & Replace" to see the modified content

## Development

To run with auto-restart on file changes:

```bash
npm run dev
```

## Testing

The application includes a comprehensive test suite:

- **Unit tests**: Test the Yale-to-Fale replacement logic
- **API tests**: Test the application endpoints
- **Integration tests**: Test the entire application workflow

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode during development
npm run test:watch

# Run tests with coverage for CI/CD
npm run test:ci
```

## CI/CD Setup

This project uses GitHub Actions for continuous integration and deployment:

- Tests run on both Node.js 18.x and 20.x
- Preview deployments are created for pull requests
- Production deployments happen automatically when tests pass on the main branch

The deployment is handled by Vercel.

## Technologies Used

- Node.js
- Express - Web server framework
- Axios - HTTP client for fetching web pages
- Cheerio - HTML parsing and manipulation
- Vanilla JavaScript for frontend functionality
- Jest, Supertest, and Nock for testing
