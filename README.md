# Software-A2
Secure Blog Assignment

DATABASE CALLED: epiz_21653868_blog

CREATE TABLE IF NOT EXISTS users (
userid int(11) NOT NULL AUTO_INCREMENT,
username varchar (30) NOT NULL,
email varchar(300) NOT NULL UNIQUE,
password varchar(300) NOT NULL,
activation varchar(300) NOT NULL UNIQUE,
status enum('0','1') NOT NULL DEFAULT '0',
PRIMARY KEY (uid)
); 

CREATE TABLE IF NOT EXISTS blog (
postid int(11) NOT NULL AUTO_INCREMENT,
title varchar (30) NOT NULL,
description varchar(300) NOT NULL UNIQUE,
content varchar(300) NOT NULL,
userid  int(11) NOT NULL,
PRIMARY KEY (postid),
FOREIGN KEY (userid)
); 

HTML5: https://www.styleshout.com/category-template/blog/

http://software-developer.epizy.com/

https://daveismyname.blog/creating-a-blog-from-scratch-with-php

https://www.phpclasses.org/blog/package/10087/post/1-secure-login-and-registration-system.html#class

http://codingcyber.org/simple-login-script-php-and-mysql-64/

https://www.tutorialrepublic.com/php-tutorial/php-mysql-login-system.php

https://blog.synapsefi.com/updates/security-blog-php

https://clevertechie.com/php/19/php-user-registration-form-mysql

http://mysqltutorial.org/php-mysql/php-mysql-blob/

http://www.codingcage.com/2016/02/upload-insert-update-delete-image-using.html

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
  - Blog table
    - PostID
    - UserID
    - PostTitle
    - PostDesc
    - PostCont
 
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
