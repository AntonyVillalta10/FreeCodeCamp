# Quality Assurance with Chai

## Overview
This is a Quality Assurance testing application using Chai, a popular JavaScript testing framework. The project is designed as a boilerplate for learning automated testing with Chai through FreeCodeCamp's Quality Assurance curriculum.

**Purpose:** Educational project for learning testing with Chai, Mocha, and automated testing practices  
**Type:** Full-stack web application with testing framework  
**Current State:** Successfully configured for Replit environment and ready to use

## Project Architecture

### Technology Stack
- **Backend:** Node.js with Express.js
- **Testing Frameworks:** 
  - Mocha (test runner)
  - Chai (assertion library)
  - Chai-HTTP (HTTP integration testing)
  - Zombie.js (headless browser testing)
- **Frontend:** Vanilla HTML, CSS, and JavaScript

### Project Structure
```
.
├── server.js           # Main Express server (entry point)
├── test-runner.js      # Mocha test runner configuration
├── assertion-analyser.js # Test assertion analyzer
├── tests/
│   ├── 1_unit-tests.js        # Unit test suite
│   └── 2_functional-tests.js  # Functional test suite
├── views/
│   └── index.html     # Frontend UI
├── public/
│   ├── client.js      # Client-side JavaScript
│   └── style.css      # Styles
└── package.json       # Dependencies
```

### Key Features
1. **Automated Test Runner:** Tests run automatically on server start
2. **API Endpoints:**
   - `GET /` - Main application UI
   - `GET /hello?name=<name>` - Simple greeting endpoint
   - `PUT /travellers` - Italian explorers lookup by surname
   - `GET /_api/get-tests` - Retrieve test results
3. **Interactive UI:** Form for testing the travellers API
4. **Test Suites:** 
   - Unit tests for Chai assertions
   - Functional tests with HTTP and browser automation

## Recent Changes (October 3, 2025)

### Replit Environment Setup
- ✅ Updated server to bind to `0.0.0.0:5000` for Replit compatibility
- ✅ Installed all npm dependencies (Express, Chai, Mocha, etc.)
- ✅ Configured workflow for automatic server startup
- ✅ Configured deployment settings (autoscale)
- ✅ Verified application functionality with screenshot testing

### Configuration Changes
- Modified `server.js` to use port 5000 (Replit requirement)
- Set server host to `0.0.0.0` for proper proxy routing
- Deployment configured for autoscale target

## How to Use

### Running the Application
The application runs automatically via the configured workflow. It will:
1. Start the Express server on port 5000
2. Automatically run the test suite
3. Display test results in the console

### Testing the Application
1. Open the application in the Replit preview
2. Use the "Famous Italian Explorers" form to test the API
3. Try surnames like: "Polo", "Colombo", "Vespucci", or "da Verrazzano"
4. View test results via the API endpoint: `/_api/get-tests`

### Expected Test Behavior
The test suite includes incomplete tests (marked with `assert.fail()`) as part of the learning curriculum. Users are expected to:
- Complete the unit test assertions in `tests/1_unit-tests.js`
- Complete the functional tests in `tests/2_functional-tests.js`
- Learn various Chai assertion methods through practice

## Development Notes

### Dependencies
All dependencies are managed via npm and defined in `package.json`:
- Express 4.17.1 (web server)
- Chai 4.3.4 (assertions)
- Mocha 9.0.3 (test runner)
- Chai-HTTP 4.3.0 (HTTP testing)
- Zombie 6.1.4 (headless browser)
- CORS 2.8.5 (cross-origin support)

### Port Configuration
- **Development:** Port 5000 (configured for Replit)
- **Deployment:** Uses PORT environment variable or defaults to 5000

### Deployment
The application is configured for Replit's autoscale deployment:
- **Target:** Autoscale (stateless web application)
- **Command:** `npm start`
- Suitable for educational/demo purposes

## User Preferences
No specific user preferences documented yet.

## Links
- FreeCodeCamp Course: https://www.freecodecamp.org/learn/quality-assurance/quality-assurance-and-testing-with-chai/
