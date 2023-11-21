# Restful Booker API Testing with Postman & Newman

This repository hosts automated API tests for the Restful Booker API, leveraging Postman collections and Newman for test execution. It also integrates Jenkins for continuous integration and continuous delivery (CI/CD) to automate the testing process. The Restful Booker API serves as a sample API for both testing and learning purposes. The test suite encompasses various endpoints, ensuring the API's functionality and reliability.

## Table of Contents

- [Technologies Used](#technologies-used)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Test Tasks](#test-tasks)
- [Generating HTML Reports](#generating-html-reports)
- [Contact](#contact)

## Technologies Used
- Postman
- Newman

## Features
- Detailed and organized API test suites.
- Comprehensive test cases covering various endpoints, HTTP methods, and scenarios, utilizing Google Sheets.
- Exported Postman collection for manual testing.
- Automation of API testing via command-line execution.
- Jenkins integration for CI/CD automation.

## Prerequisites
Before getting started, ensure you have:

- **Postman**: Download it from [Postman Downloads](https://www.postman.com/downloads/).
- **Newman**: Install via Node.js using `npm install -g newman`.
- **Jenkins**: Set up a Jenkins server for CI/CD automation.

## Installation
Follow these steps to set up the project:

  1. Clone this repository to your local machine:
  2. Navigate to the project directory:
     cd Restful-Booker-APIS
  3. Install project dependencies:
    - Install Postman.
    - Install Newman.
    - Install Newman-reporter-htmlextra.
## Usage
### Running Tests in Postman
1. Open Postman.
2. Import the Postman collection.
3. Configure environment variables using the provided Postman environment directory.
4. Run the API tests using Postman's collection runner.

### Running Tests via Command Line (Newman)
Execute tests via the command line using Newman:
  Newman runs BookingAPIS.json -e Bookingenvironment.json -r htmlextra     

## Test Tasks
The tests are organized into collections within Postman, each focusing on specific API tasks:
- CREATE Token
- GET ALL Booking ID
- CREATE Booking
- GET Details For Booking ID
- UPDATE Booking
- UPDATE Booking Partially
- DELETE Booking
- Ping - HealthCheck

For detailed test scenarios and requests, refer to the [Google Sheets](https://docs.google.com/spreadsheets/d/1saJHUvAjCNjZ-i4enfGtgWL8LNLOINWHmw2tIsTTdyg/edit?usp=sharing).

## Generating HTML Reports
Newman supports various reporters, including htmlextra, which generates detailed HTML reports for API test runs. To generate HTML reports, use `-r htmlextra` option when running Newman.

HTML reports will be available in the reports directory of this repository.

## Contact
For questions, suggestions, or issues related to this project, please feel free to contact us:

- Email: mahmoudkhallaf288@gmail.com  

      
   
