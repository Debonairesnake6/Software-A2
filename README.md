# Software-A2
Secure Blog Assignment

http://software-developer.epizy.com/

https://daveismyname.blog/creating-a-blog-from-scratch-with-php

https://www.phpclasses.org/blog/package/10087/post/1-secure-login-and-registration-system.html#class

http://codingcyber.org/simple-login-script-php-and-mysql-64/

https://www.tutorialrepublic.com/php-tutorial/php-mysql-login-system.php

https://blog.synapsefi.com/updates/security-blog-php

Languages:
  - php
  - mysql
  - html
  - css
  
  Framework:
    - code igniter
 
 Ryan:
  - Create new blog
    - Edit existing blog
    - Published to main blog
    - Contain the following
      - Images
      - Hyperlinks
      - Videos
      - Formatting options
        - Headings
        - Lists
        - etc.
    - User can write in HTML or markup
  - Manage blogs
    - Create, edit, delete posts
  - Main blog page
    - Visitors can view summary
    - Click post for detailed view
    - Show author and avatar
 
 Mike:
  - User registration
    - Unique username
    - Valid email
    - Valid password
    - Activation link (Only need to log)
    - Need admin aproval
  - User login
    - Send to blog management page
    - Forgot my password
  - User profile page
    - Only valid user can visit/edit
    - Upload avatar
    - Change basic details
    - Re-authentication to change password
  - Admin page
    - Create, edit, approve, delete users

Security:
  - SSL encryption (all pages)
  - All forms validated
  - Passwords salted/hashed
  - Avatar uploads (img only)
    - Strip metadata
  - Protect against:
    - SQL injection
    - XSS
    - CSRF
    - Open redirects
  - Account lock after 5 failed attempts
  - Encrypt using strong algorithms
  - Logs

Bonuses:
  - Implement 2FA
    - Using an app/Email
  - Look professional
    - HTML5 and CSS3 compliant
  - Host live server and add DoS protection
  - Email can
    - Activate account
    - Reset password
    - Unlock account
  - Daily offsite backups
    - Demonstrate recovery
