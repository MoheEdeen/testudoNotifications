testudoNotifications
Overview
testudoNotifications is a Python script designed to notify you via email when a specific class opens up for registration on the University of Maryland's Testudo system. The original code was adapted from matthewnau's repository.

Features
Monitors class availability for a specified term and course.
Sends email notifications when the class becomes available.
Prerequisites
Python 3.x installed on your machine.
Internet connection for accessing Testudo and sending email notifications.
Access to Testudo's term and class IDs.
Installation
Clone the Repository:

Download the code from the repository using the following command:

bash
Copy code
git clone https://github.com/yourusername/testudoNotifications.git
Navigate to the Project Directory:

bash
Copy code
cd testudoNotifications
Install Required Packages:

Ensure you have the necessary Python packages installed. If not, install them using pip:

bash
Copy code
pip install requests smtplib
Configuration
Before running the script, you need to update a few placeholders in the code:

Term ID:

Search for PUT_TERM_ID_HERE in the code.
Replace it with the term ID you are interested in (e.g., Fall 2024, Spring 2025).
Class Name:

Search for CLASSNAME in the code.
Replace it with the course code you want to monitor (e.g., CMSC250).
Email Address:

Search for EMAILHERE in the code.
Replace it with the email address where you want to receive notifications.
Usage
Once the configuration is complete, run the script using the following command:

bash
Copy code
python testudoNoti.py
The script will continuously monitor the specified class's availability on Testudo and send an email notification to the provided email address when the class opens up.

Troubleshooting
No Notifications Received: Ensure that your email credentials are correctly configured in the script, and that the email server settings are accurate.
Script Fails to Run: Check that all dependencies are installed, and that the term ID and class name are correctly specified.
Contributions
This project is based on original code by Matthew Nau. Contributions to further improve or customize this script are welcome. Feel free to submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
