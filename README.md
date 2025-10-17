# Captcha Solver Frontend Application

This project provides a simple, single-file responsive web application for solving captchas, built with HTML, JavaScript, and Tailwind CSS. It's designed to demonstrate a basic frontend interaction for displaying a captcha image and validating user input.

## Features

-   **Responsive Design**: Utilizes Tailwind CSS for a modern, mobile-first, and responsive user interface.
-   **Dynamic Image Loading**: Loads captcha images from a URL query parameter (`?url=...`) or defaults to a local `sample.png`.
-   **Client-Side Validation**: Basic client-side validation for user input against a hardcoded captcha solution.

## How to Use

1.  **Open `index.html`**: Simply open the `index.html` file in your web browser.
2.  **Default Captcha**: The application will initially display `sample.png` as the captcha image.
3.  **Custom Captcha (via URL)**: You can provide a custom captcha image URL by appending a `?url=` query parameter to the `index.html` file in your browser's address bar.
    *   Example: `file:///path/to/your/project/index.html?url=https://example.com/some-captcha-image.png`
    *   Or, if hosted: `https://yourdomain.com/index.html?url=https://example.com/some-captcha-image.png`
4.  **Enter Solution**: Type the characters displayed in the captcha image into the input field.
5.  **Submit**: Click the "Submit" button or press Enter to check your answer.

## Captcha Solution

For the `sample.png` image provided, the expected solution is `ADoR3`. The current implementation performs a case-sensitive comparison. For a real-world application, an OCR (Optical Character Recognition) backend would be integrated to dynamically read the captcha text.

## Technologies Used

-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: Utility-first CSS framework for styling and responsiveness.
-   **JavaScript**: Client-side logic for image loading, input handling, and validation.

## Development

This application is designed as a standalone `index.html` file, making it easy to deploy or use as a starting point. No build tools are required beyond a web browser.