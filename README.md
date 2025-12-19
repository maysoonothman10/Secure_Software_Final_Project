# Secure_Software_Final_Project

This repository contains a deliberately vulnerable Node.js + Express application for security testing.

---

## Installation
Clone the repository:
git clone https://github.com/SirAppSec/vuln-node.js-express.js-app.git

cd vuln-node.js-express.js-app

Install dependencies:
npm install (need nvm version 16 or 18)

Start the app:
npm run dev

The app will run at:
http://localhost:5000

Running ZAP
Open OWASP ZAP.

Set the target URL to:
http://localhost:5000
Import the OpenAPI specification if needed:

http://localhost:5000/v1/api-docs/
Run Passive Scan or Active Scan.

Review alerts for vulnerabilities.

Running Semgrep
Base Rules
semgrep --config "p/javascript" --config "p/nodejs" --error

Custom Rules
Custom rules are located in the semgrep-rules/ directory:
semgrep --config semgrep-rules/ --error
