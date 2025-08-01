# Asiimwe Edson - Software Engineer Portfolio

A modern, responsive portfolio website built with HTML, Tailwind CSS, and PHP for email functionality.

## Features

- ✅ Responsive design
- ✅ Dark mode toggle
- ✅ Smooth scrolling navigation
- ✅ Contact form with email functionality
- ✅ CV download functionality
- ✅ Back to top button
- ✅ Modern UI with Tailwind CSS

## Email Setup Instructions

### 1. Install Dependencies

First, install PHPMailer using Composer:

```bash
composer install
```

### 2. Configure Email Settings

Edit `send_email.php` and update the following settings:

```php
$mail->Host = 'smtp.gmail.com'; // Your SMTP host
$mail->Username = 'your-email@gmail.com'; // Your email
$mail->Password = 'your-app-password'; // Your app password
```

### 3. Gmail Setup (if using Gmail)

1. Enable 2-Factor Authentication on your Gmail account
2. Generate an App Password:
   - Go to Google Account settings
   - Security → 2-Step Verification → App passwords
   - Generate a password for "Mail"
3. Use this app password in the PHP file

### 4. Server Requirements

- PHP 7.4 or higher
- Composer
- SMTP access (Gmail, Outlook, etc.)

## File Structure

```
Profile_website/
├── index.html          # Main portfolio page
├── send_email.php      # Email handling script
├── composer.json       # PHP dependencies
├── assets/
│   └── cv-john-doe.txt # CV file
└── README.md          # This file
```

## Customization

### Update Personal Information

Edit `index.html` to update:
- Name and title
- Contact information
- Skills and experience
- Projects
- Social media links

### Update CV

Replace `assets/cv-john-doe.txt` with your actual CV file.

### Email Configuration

The contact form will send emails to `eddieas2012@gmail.com`. Update this in `send_email.php` if needed.

## Testing

1. Start a local PHP server:
```bash
php -S localhost:8000
```

2. Open `http://localhost:8000` in your browser

3. Test the contact form by filling it out and submitting

## Deployment

### Shared Hosting
1. Upload all files to your web server
2. Run `composer install` on the server
3. Configure email settings in `send_email.php`

### VPS/Dedicated Server
1. Install PHP and Composer
2. Upload files
3. Run `composer install`
4. Configure email settings

## Security Notes

- Remove debug information in production
- Use environment variables for sensitive data
- Enable HTTPS in production
- Validate and sanitize all input

## Support

For issues or questions, please contact eddieas2012@gmail.com 