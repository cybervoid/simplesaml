Small example of **SAML 2.0** implementation with IdP on **MYSQL** and **SimpleSAMLPHP**

Features:
- User Management CRUD (thanks: https://github.com/ajayrandhawa/User-Management-PHP-MYSQL)
- Apache
- MySQL
- SimpleSAMLPHP 
 
_(This is only for learning purposes, do not use for production)_

- Create a symlink on /var/simplesamlphp so we can keep the default path and any changes made to the repo

`sudo ln -s /var/www/html/simplesaml/simplesamlphp/ /var/simplesamlphp`

- create a vhost pointing to the identity provider directory
- check if user management is working:
    -username: admin
    -password: 963852741
    -http://www.yourdomain.com/admin/
- create a new user
- log to simplesaml interface:
    - http://www.yourdomain.com/simplesaml
    - username: admin
    - password: cornell_2018
- if everything is working, check authentication for the new user under **_example-sql_**
