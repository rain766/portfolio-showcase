SplitSnap

A modern Flask web application for secure file uploads with a beautiful drag-and-drop interface.

## Demo[TBD]

[Live Demo]()

## Screenshots

![SplitSnap screenshot 1](https://github.com/rain766/portfolio-assets/blob/main/SplitSnap2025/SplitSnap2025_1.png?raw=true)  
![SplitSnap screenshot 2](https://github.com/rain766/portfolio-assets/blob/main/SplitSnap2025/SplitSnap2025_2.png?raw=true)  
![SplitSnap screenshot 3](https://github.com/rain766/portfolio-assets/blob/main/SplitSnap2025/SplitSnap2025_3.png?raw=true)  
![SplitSnap screenshot 4](https://github.com/rain766/portfolio-assets/blob/main/SplitSnap2025/SplitSnap2025_4.png?raw=true)

## Features

- Modern, responsive UI with drag-and-drop functionality
- Support for multiple file types (txt, pdf, png, jpg, jpeg, gif, doc, docx)
- Secure file handling with filename sanitization
- Real-time upload progress tracking
- RESTful API endpoints

## API Endpoints

### GET `/`

- **Description**: Home page with upload form
- **Response**: HTML page with drag-and-drop interface

### GET `/upload`

- **Description**: Upload page
- **Response**: HTML page for file uploads

### POST `/upload`

- **Description**: Handle file upload
- **Request**: Multipart form data with file
- **Response**: JSON response with upload status

#### Request Format:

```
Content-Type: multipart/form-data
Body: file=<file_data>
```

#### Response Format:

```json
{
  "message": "File uploaded successfully",
  "filename": "example.pdf",
  "filepath": "uploads/example.pdf"
}
```

## Configuration

The application can be configured by modifying the following settings in `app.py`:

- `UPLOAD_FOLDER`: Directory where uploaded files are stored (default: 'uploads')
- `MAX_CONTENT_LENGTH`: Maximum file size in bytes (default: 16MB)
- `ALLOWED_EXTENSIONS`: Set of allowed file extensions

## File Types Supported

- Text files: `.txt`
- PDF documents: `.pdf`
- Images: `.png`, `.jpg`, `.jpeg`, `.gif`
- Documents: `.doc`, `.docx`

## Security Features

- File type validation
- Filename sanitization using `secure_filename`
- File size limits
- Secure file storage in dedicated uploads directory

## Development

To run the application in development mode with auto-reload:

```bash
python app.py
```

The application will run on `http://localhost:5000` with debug mode enabled.

## Project Structure

```
SplitSnap/
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── README.md          # Project documentation
├── templates/         # HTML templates
│   └── index.html     # Main upload page
└── uploads/           # Uploaded files directory (created automatically)
```

## Notes

This repository is for project overview and demo access only. Source code is not included.
