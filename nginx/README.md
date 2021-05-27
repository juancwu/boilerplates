# Nginx Boilerplates

## Nginx Directories List

- **/etc/nginx** - the nginx configuration directory.
- **/etc/nginx/nginx.conf** - the main Nginx configuration file; this can be modifie to make changes to global configuration. (/usr/local/nginx/conf or /usr/local/etc/nginx are alternative directories for the main configuration file)
- **/etc/nginx/sites-available** - the directory where per-site "sever blocks" can be stored; Ngninx **will not use** the configuration files found in this directory unless they are linked to the sites-enabled directory. `ln -s /etc/nginx/sites-available/example.com /etc/nginx/sites-enabled/example.com` to make a symbolic link between sites-available and sites-enabled directories.
- **/etc/nginx/sites-enabled** - the directory where enabled per-site "server blocks" are stored.
- **/etc/nginx/snippets** - this directory contains repeatable configuration segments that can be use else where.
- **/var/log/nginx/access.log** - every request to the web server is recorded in this log file unless Nginx is configured otherwise.
- **/var/log/nginx/error.log** - any Nginx error will be recorded in this log file.
