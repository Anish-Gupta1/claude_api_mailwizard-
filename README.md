# Claude MailWizard Backend

## Overview
Claude MailWizard Backend is a server that facilitates email generation using Anthropic's Claude AI. This backend is required to run locally when using the **Anthropic API key** for generating email responses.

## Prerequisites
Ensure you have the following installed:
- **Node.js** (v16 or later recommended)
- **npm** or **yarn**
- **Anthropic API key** (store it securely)

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/claude-mailwizard-be.git
   cd claude-mailwizard-be
   ```

2. Install dependencies:
   ```sh
   npm install
   # or
   yarn install
   ```

## Running the Server
Start the backend server with:
```sh
npm start
# or
node index.js
```
If using nodemon for development:
```sh
npm run dev
```
The server will run on `http://localhost:3000` by default.

## API Endpoints
### Generate Email
**POST** `/api/generate`

#### Request Body:
```json
{
  "prompt": "Your input text here"
}
```

#### Response:
```json
{
  "generatedEmail": "Your AI-generated email content"
}
```

