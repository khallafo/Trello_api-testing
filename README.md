Restful trello API Testing with Postman, Newman
This repository contains automated API tests for the Restful Booker API, utilizing Postman collections and Newman for test execution. Additionally, it incorporates Jenkins for continuous integration and continuous delivery (CI/CD) to automate the testing process. The Restful Booker API is a sample API for testing and learning purposes. The test Modules covers a variety of endpoints and tests to ensure the API's functionality and reliability.

Table of Contents
Technologies Used
Features
Prerequisites
Installation
Usage
Test Tasks
Generating HTML Reports
Contact
Technologies Used
POSTMAN - Newman

Features
Detailed and organized API test suites.
Test cases covering various endpoints, HTTP methods, and scenarios using Google sheets.
Exported Postman collection for manual testing 
Automation of API testing through cmd 
Prerequisites
Before you begin, ensure you have met the following requirements:

Postman: You need to have Postman installed. If you don't have it, you can download it from Postman Downloads.

Newman: You can install Newman using Node.js. Make sure you have Node.js installed, and then run the following command:

npm install -g newman
Jenkins: You will need a Jenkins server set up for CI/CD automation. You can install Jenkins following the instructions on the Jenkins website.

Installation
Clone this repository to your local machine:

git clone (https://github.com/khallafo/Trello_api-testing)
Navigate to the project directory:

cd Restful-Booker-APIS
Install the project dependencies:

Install Postman
Install Newman
Install Newman-reporter-htmlextra
Usage
Running Tests in Postman

Open Postman.
Import the Postman collection.
Configure the environment variables using the Postman environment "Bookingenvironment" directory or create your own environment file.
Run the API tests using Postman's collection runner.
Running Tests via the Command Line using the Newman

You can also run the tests via the command line using Newman. Use the following command to run a specific test suite, specifying the environment:

newman run BookingAPIS.json -e Bookingenvironment.json -r htmlextra
Test Tasks
The tests are organized into collections within Postman, each focusing on specific API tasks:

- CREATE Token: Test Task for creating an authentication token.

- GET ALL Booking ID: Test Task for retrieving all booking IDs.

- CREATE Booking: Test Task for creating a new booking.

- GET Details For Booking ID: Test Task for retrieving details of a specific booking ID.

- UPDATE Booking: Test Task for updating an existing booking.

- UPDATE Booking Partially: Test Task for partially updating an existing booking.

- DELETE Booking: Test Task for deleting a booking.

- Ping - HealthCheck: Test Task for checking the API's health status.

For more details on the test scenarios, expected outcomes, and specific requests you will find them in the Google Sheets (https://docs.google.com/spreadsheets/d/1saJHUvAjCNjZ-i4enfGtgWL8LNLOINWHmw2tIsTTdyg/edit?usp=sharing))
Generating HTML Reports
Newman supports multiple reporters, including htmlextra, which generates detailed HTML reports for your API test runs. To generate HTML reports, simply specify the -r htmlextra option when running Newman, as shown in the example above.

The HTML reports will be available in the reports directory of this repository.

Contact
If you have any questions, suggestions, or issues related to this project, please feel free to contact us. We welcome your feedback and contributions.

Email: mahmoudkhallaf288@gmail.com
