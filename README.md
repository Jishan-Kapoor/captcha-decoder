# Decode CAPTCHA App

## Summary
The Decode CAPTCHA App is a static web application that decodes CAPTCHA images encoded in base64 format. It processes the PNG image data to extract and return the encapsulated text, using advanced image processing techniques. This lightweight application is hosted on GitHub Pages, ensuring accessibility and ease of deployment.

## Setup
To deploy this application on GitHub Pages, follow these steps:

1. **Fork the Repository**: Start by forking the repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using:
   ```bash
   git clone https://github.com/your-username/decode-captcha-app.git
   ```
3. **Navigate to Directory**: Change to the directory where you cloned the repository:
   ```bash
   cd decode-captcha-app
   ```
4. **Push Changes** (optional): Make any desired changes locally, then commit and push them back to your GitHub repository.
5. **Enable GitHub Pages**:
   - Go to the repository on GitHub.
   - Navigate to the "Settings" tab.
   - Scroll down to the "GitHub Pages" section.
   - Select the main branch as the source.
   - Save the settings. Your application is now published at `https://your-username.github.io/decode-captcha-app/`.

## Usage

### Accessing the Page
Visit the deployed GitHub Pages URL: `https://your-username.github.io/decode-captcha-app/`.

### Query Parameters and Configuration
- **Image Input**: The application accepts a base64-encoded PNG image data as input, which can be uploaded via the interface or input directly through a URL parameter.
- **Configuration Options**: The new feature includes automatic decoding of the CAPTCHA from the input base64 PNG image and returning the extracted text instantly.

### Key Features
- **User Interface**: A simple and intuitive interface for uploading images, and an option to input via URL.
- **Text Output**: Automatically outputs decoded text from the provided CAPTCHA.

## Code Explanation

### Technical Overview
The application is a combination of HTML for structure, CSS for styling, and JavaScript for functionality. It leverages a client-side scripting approach to accomplish CAPTCHA decoding.

### Key Libraries
- **Tesseract.js**: This OCR library is instrumental in processing and decoding text from images within the browser.

### Important Algorithms and Logic
- **Base64 Decoding**: Converts base64 strings back to binary data to create an image object.
- **Image Preprocessing**: Prepares the image for optimal OCR performance, including gray-scaling and thresholding where applicable.
- **OCR Process**: Utilizes the Tesseract.js library to interpret and extract text from the image.

## License
This project is licensed under the MIT License. For more information, see the [LICENSE](LICENSE) file.