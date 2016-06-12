# create-site
A Bash script to create an Nginx 'virtual host' with per-user PHP-FPM pools for increase security. This script has only been used on Debian 8 Jessie/Ubuntu 14.04.

## Installation

In order to use this script, you have already installed Nginx and php-fpm. At the time of writing for Debian Jessie this can be done by installing the packages with apt-get:

`apt-get install nginx php5-fpm`

## Usage

Download this repository:
```
git clone https://github.com/Sam-R/create-site.git
```

Go into the repository
```
cd create-site
```

Create a site by calling the script using elevated privileges (sudo or root user) and with a valid domain name:
```
./create-site example.com
```

Follow the on-screen instructions to create a site host in Nginx, user account and PHP-FPM pool.
