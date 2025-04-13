# Link Shortener API

A simple URL shortening service built with Node.js, Express, and MongoDB, similar to Bitly. It creates short URLs from long ones and redirects users to the original URL.

## Features
- **Shorten URLs**: Convert long URLs to short ones via POST `/api/url/shorten`.
- **Redirect**: Access short URLs to redirect to the original site.
- **MongoDB Storage**: Stores URLs in a MongoDB Atlas database.

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/S-anuse/Link-Shortner.git

## Install dependencies
npm install

## Run
npm start

## Usage
 POST to shorten : 
 ```bash curl -X POST -H "Content-Type: application/json" -d '{"longUrl":"https://www.amazon.com"}' http://localhost:5000/api/url/shorten

 GET to redirect
 Visit http://localhost:5000/xyz123

## Technologies: 
Node.js
Express
MongoDB (Atlas)
Mongoose
shortid (for URL codes)
valid-url (for URL validation)


## Notes
Warnings:
Ignored Git LF/CRLF warnings (Windows line endings, no functional impact).
Noted Mongoose circular dependency warnings (count, findOne) and Node.js [DEP0170] deprecation warning (MongoDB URI). Functionality unaffected.
Would upgrade Mongoose and dependencies in production.
Vulnerabilities:
 39 npm vulnerabilities (e.g., shortid) ignored for this prototype, as they didn’t affect testing.