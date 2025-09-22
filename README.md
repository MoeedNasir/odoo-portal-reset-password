# Odoo Portal Reset Password

A custom Odoo module that provides a **password reset flow for portal users**.  
This module extends Odoo’s authentication system to allow portal users to securely reset their password from the website.

##  Module Information
- **Name:** Portal Reset Password  
- **Version:** 1.0  
- **Author:** Tech Cog  
- **Category:** Website  
- **Depends on:** `base`, `website`, `auth_signup`  

##  Module Structure
portal_reset_password/
│
├── init.py
├── manifest.py
│
├── controllers/
│ ├── init.py
│ └── portal_reset_password.py
│
├── security/
│ └── ir.model.access.csv
│
└── views/
├── override_login.xml
└── reset_templates.xml

## Features
- Custom **reset password form** for portal users.  
- Secure flow integrated with Odoo’s authentication system.  
- Website views for password reset pages.  
- Override of default login to add "Forgot Password" option.  

## Installation
1. Copy the module folder `portal_reset_password` into your Odoo `addons` directory.  
2. Update the Odoo app list: 
or update from **Apps > Update Apps List** in the Odoo backend.  
3. Search for **Portal Reset Password** in Apps and install it.  

## Usage
1. Go to the **Website Login Page**.  
2. Click on **Forgot Password?**.  
3. Enter your registered email address.  
4. Receive reset link → Set new password → Log in again.  

## License
This module is licensed under the **LGPL-3.0 License** (same as Odoo Community).  

## Notes
- Designed for **portal users only** (customers, suppliers, etc.).  
- Can be extended for custom authentication flows.  
 
