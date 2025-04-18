# Email Automation

A Streamlit-based email automation tool that allows users to send emails with customizable templates, file attachments, and a user-friendly interface.

## Features

- 📧 Send emails using Gmail SMTP
- 📝 Pre-defined email templates
- 📎 Support for multiple file attachments
- 🎨 Light/Dark theme selection
- 🔒 Secure password handling
- 📱 Responsive user interface

## Prerequisites

- Python 3.x
- Gmail account with App Password enabled
- 2-Step Verification enabled for your Google Account

## Getting Started

### Clone the Repository

You can clone this repository using either HTTPS or SSH method:

#### HTTPS Method
```bash
git clone https://github.com/yourusername/Email_Automation.git
cd Email_Automation
```

#### SSH Method (if you have SSH keys configured)
```bash
git clone git@github.com:yourusername/Email_Automation.git
cd Email_Automation
```

### Installation

1. Create and activate a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Unix/macOS
# OR
venv\Scripts\activate  # On Windows
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the project root with the following variables:
```
SENDER_EMAIL=your-email@gmail.com
RECEIVER_EMAIL=default-receiver@example.com
EMAIL_PASSWORD=your-gmail-app-password
```

## Usage

1. Start the application:
```bash
streamlit run streamlit_app.py
```

2. Access the web interface at `http://localhost:8501`

3. Fill in the email form:
   - Select an email template
   - Verify/modify sender and receiver emails
   - Customize subject and message
   - Add attachments (optional)
   - Enter your Gmail App Password

4. Click "Send Email" to send your message

## Gmail App Password Setup

1. Go to your Google Account settings
2. Enable 2-Step Verification if not already enabled
3. Navigate to Security > App Passwords
4. Generate a new app password
5. Use this password in the application

## Technical Details

### Dependencies

- streamlit>=1.28.0
- python-dotenv>=1.0.0
- email-validator>=2.1.0

### Features

- Maximum attachment size: 25MB
- Supports multiple file attachments
- Real-time email preview
- Progress tracking for email sending
- Secure password handling

## Security Notes

- Never share your Gmail App Password
- Store sensitive information in the `.env` file
- The `.env` file should never be committed to version control
- Check spam folder if emails are not received

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
