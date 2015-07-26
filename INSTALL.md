## Install the Burrow Server

### Requirements
 - SSH access tor your server with permission to `sudo`.
 - A supported version of [Nginx](http://nginx.org/) on that server.
 - A supported version of [PHP](http://www.php.net/supported-versions.php) on that server.
 
### Procedure
1. Copy the files to your server.
2. Import the Database.
3. Modify the database variables in `settings.database.php`
4. Modify the hostname in `nginx.conf`
5. Run `sudo ln -s /path/to/burrow/_burrow/nginx.conf /etc/nginx/sites-enabled/burrow.conf`
6. Run `sudo service nginx restart`
7. If Burrow is set to public (the default), you can see it by going to your IP address or domain.

## Add an Agent

### Requirements
 - A monitoring server with [Burrow](https://github.com/eustasy/burrow) already installed.
 - A server with SSH access.
 - A supported version of [PHP](http://www.php.net/supported-versions.php) on that server.

### Procedure
1. Copy the files for the [Weasel Agent](https://github.com/eustasy/weasel) onto your server.
2. Generate Secret
3. Copy the Secret to Burrow
4. Set up Cron job
