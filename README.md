# Moodle Email Templates Repository

Welcome to the **Moodle Email Templates** repository! This repository collects, shares, and contributes a variety of email templates for use within Moodle. These templates can be customized and used by Moodle administrators, developers, and educators to streamline communication in various Moodle notifications and events.

## Overview

Moodle provides a powerful notification system, but customizing the email templates can be a complex and time-consuming task. This repository aims to make this process easier by offering a collection of pre-made email templates for common Moodle events. These templates can be used, modified, and integrated into Moodle systems quickly.

## Repository Structure

The repository contains email templates categorized by their use in Moodle, such as:

- User Registration
- Course Enrollment
- Assignment Submissions
- Grade Notifications
- Course Completion
- Password Reset
- And more…

### Example Template Structure

```plaintext
templates/
├── user_registration/
│   ├── welcome_email.html
│   └── welcome_email_plain.txt
├── course_enrollment/
│   ├── enrollment_email.html
│   └── enrollment_email_plain.txt
├── assignment_submission/
│   ├── assignment_submission_notification.html
│   └── assignment_submission_notification_plain.txt
└── ...
```

Each folder contains:
- `*.html` - HTML-formatted version of the email template.
- `*.txt` - Plain-text version of the email template.

## How to Add a New HTML Email Template to Moodle

To add a new HTML email template to your Moodle installation, follow these steps:

1. **Download or Clone the Repository:**
   First, clone or download the repository to get the email templates.

2. **Identify the Template to Add:**
   Choose the relevant template from the repository. For example, if you want to add a "Welcome Email" template, navigate to `templates/user_registration/welcome_email.html`.

3. **Locate Moodle’s Email Template Directory:**
   In your Moodle installation, navigate to the directory where Moodle stores its language-specific email templates. For English, it’s typically located in the following path:

   ```
   moodle/lang/en/email/
   ```

4. **Add the New Template:**
   - Copy the `.html` version of the template to the `email/` directory.
   - Copy the `.txt` version if you want a plain text version of the template.
   - Ensure that the file names are descriptive, as they will be referenced by Moodle’s notification system. For example, you could name it `user_registration_welcome.html`.

5. **Modify the Template (if necessary):**
   - Open the copied HTML file and make any necessary adjustments (e.g., add dynamic content variables, customize the design, etc.).
   - The email templates in Moodle support placeholders for dynamic content, such as `{FIRSTNAME}`, `{LASTNAME}`, and `{COURSE}`. Make sure you use the correct placeholders according to Moodle's documentation.

6. **Configure Moodle to Use the New Template:**
   - Once you have placed the template in the `email/` directory, you may need to configure Moodle to use the new template for specific events.
   - Go to **Site administration > Language > Email** in Moodle.
   - Look for the specific event or notification that corresponds to your template (for example, "User account creation" or "Course enrollment").
   - Ensure the correct template is selected or edited in Moodle's settings.

7. **Test the Template:**
   - Test the new email template by triggering the corresponding event (e.g., registering a user or enrolling in a course) to verify that the template is used and the email is sent correctly.
   - Ensure that any dynamic content, like the user’s name or course details, appears as expected.

## Contributing

We welcome contributions from the community! If you have a new email template or improvements to existing ones, feel free to open a **Pull Request**.

To contribute:

1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a new branch for your changes.
4. Add your email template(s).
5. Commit your changes with a descriptive message.
6. Push to your fork and create a pull request.

## License

This repository is open source and available under the **MIT License**. You are free to use, modify, and distribute the templates.

## Acknowledgements

This repository is made possible by the Moodle community’s contributions. Special thanks to everyone who shares their knowledge and experience in customizing Moodle.

## Contact

For any questions or support related to the email templates, please open an issue in this repository or contact us at wailabualela@gmail.com.
