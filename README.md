# File Metadata Microservice

This project is a simple file metadata microservice built with Node.js and Express. It allows users to upload a file and then returns a JSON response with the file's metadata, including its name, type, and size.

## Features

- File upload functionality using `multer` with memory storage, meaning files are not stored on the server's disk.
- Returns file metadata as JSON.

## How to Use

1. Clone this repository to your local machine.
2. Install dependencies by running `npm install`.
3. Start the server with `npm start`. The server will listen on the port specified in your `.env` file or default to port 3000.
4. Access the application through `http://localhost:3000` in your web browser.
5. Use the form to upload a file. Upon submission, the server will respond with the file's metadata.

## Endpoints

- `GET /`: Displays a simple file upload form.
- `POST /api/fileanalyse`: Endpoint to which the file is uploaded. Returns the file's metadata as JSON.

## Technologies Used

- Node.js
- Express
- Multer for handling `multipart/form-data`.

## Environment Variables

To run this project, you will need to add the following environment variable to your `.env` file:

- `PORT` (optional) - The port number on which the server will listen.