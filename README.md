QR Code Generator
This simple Node.js application allows you to generate a QR code from a URL provided by the user. The application prompts the user for a URL, generates a QR code image, and saves both the QR code image and the URL to a file.

How It Works
Prompt the User for a URL:

The application uses the inquirer package to prompt the user to input a URL.
Generate the QR Code:

Once the URL is provided, the qr-image package generates a QR code image from the URL.
Save the QR Code and URL:

The QR code is saved as a PNG image (qrr_img.png).
The URL is also saved in a text file (Url.txt).
Prerequisites
To run this application, you'll need to have Node.js installed on your machine.

You’ll also need to install the following npm packages:

inquirer - A collection of common interactive command-line user interfaces.
qr-image - A module for generating QR codes.
fs - A Node.js built-in module to interact with the file system.
Installation
Clone this repository to your local machine.

Navigate to the project directory.

Install the required npm packages:

bash
Copy code
npm install inquirer qr-image
Usage
To run the application, execute the following command:

bash
Copy code
node index.js
You will be prompted to enter a URL. Once you enter the URL:

A QR code will be generated and saved as qrr_img.png in the current directory.
The entered URL will be saved to a file named Url.txt.
Example
Here’s what happens when you run the program:

bash
Copy code
? Type in your Url: https://www.example.com
After entering the URL, the QR code image (qrr_img.png) and the text file containing the URL (Url.txt) will be created in the project directory.

Error Handling
The application includes basic error handling:

If the prompt cannot be rendered in the current environment, a message is logged.
If there's an issue saving the file, the error is thrown.
