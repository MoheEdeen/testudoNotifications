# testudoNotifications

## Overview
`testudoNotifications` is a Python script designed to notify you via email when a specific class opens up for registration on the University of Maryland's Testudo system. The original code was adapted from [matthewnau's repository](https://github.com/matthewnau/testudo/commits?author=matthewnau).

## Features
- Monitors class availability for a specified term and course.
- Sends email notifications when the class becomes available.

## Prerequisites
- Python 3.x installed on your machine.
- Internet connection for accessing Testudo and sending email notifications.
- Access to Testudo's term and class IDs.

## Important Notes

- **Not a Web Scraper:** This script does not scrape the website for data. It directly checks the "Schedule of Classes" section on Testudo, which is publicly accessible.
- **No Special Benefits:** This script does not provide any special privileges or allow you to register for classes before others. It only notifies you when a class becomes available, based on the data provided by Testudo.
- **Notification Only:** The script sends you an email notification when a class opens up. It does not automate the registration process.

## Installation

1. **Clone the Repository:**

   Download the code from the repository using the following command:

   `git clone https://github.com/yourusername/testudoNotifications.git`

2. **Navigate to the Project Directory:**

   `cd testudoNotifications`

3. **Install Required Packages:**

   Ensure you have the necessary Python packages installed. If not, install them using `pip`:

   `pip install requests smtplib`

## Configuration
Before running the script, you need to update a few placeholders in the code:

1. **Term ID:**

   - Search for `PUT_TERM_ID_HERE` in the code.
   - Replace it with the term ID you are interested in which is found here:
   - <img width="718" alt="image" src="https://github.com/user-attachments/assets/eb209758-46d7-4529-b584-f53ed93ff03d">
   - <img width="964" alt="image" src="https://github.com/user-attachments/assets/c531ac90-f9ce-4f17-837a-8c2c2326ba2f">
   - <img width="958" alt="image" src="https://github.com/user-attachments/assets/96c5f6f9-851d-4685-af26-936a138cdd47">

2. **Class Name:**

   - Search for `CLASSNAME` in the code.
   - Replace it with the course code you want to monitor (e.g., CMSC250).

3. **Email Address:**

   - Search for `EMAILHERE` in the code.
   - Replace it with the email address where you want to receive notifications.

## Usage
Once the configuration is complete, run the script using the following command:

`python testudoNoti.py`

The script will continuously monitor the specified class's availability on Testudo and send an email notification to the provided email address when the class opens up.

## Troubleshooting
- **No Notifications Received:** Ensure that your email credentials are correctly configured in the script, and that the email server settings are accurate.
- **Script Fails to Run:** Check that all dependencies are installed, and that the term ID and class name are correctly specified.

## Contributions
This project is based on original code by [Matthew Nau](https://github.com/matthewnau/testudo/commits?author=matthewnau). Contributions to further improve or customize this script are welcome. Feel free to submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
