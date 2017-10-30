# Super Fast, Secure WordPress Setup for Ubuntu 16.04 LTS on DigitalOcean with NGINX, PHP7, and MariaDB

This is a shell script to automate setting up [the WordPress server setup described in this blog post](http://www.morphatic.com/2016/05/21/super-fast-secure-wordpress-install-on-digitalocean-with-nginx-php7-and-ubuntu-16-04-lts/). To use it:

1. Create a droplet at DigitalOcean--use the Ubuntu 16.04 LTS image on the smallest size droplet
2. Set up your domain over at [Mailgun](https://mailgun.com)
3. Set up your DNS at DigitalOcean
4. Log into your new droplet via SSH, i.e. `ssh root@[your-droplet's-IP-address]`
5. Import this script<br>`curl -s https://raw.githubusercontent.com/morphatic/fast_secure_wp_server_setup/master/fast_secure_wp_server_setup -o server_setup`
6. Make it executable: `chmod +x server_setup`
7. Run it: `sudo ./server_setup`
8. Follow all of the instructions and be very careful filling out the prompts

**NOTE: This ONLY works for new domain setups where your domain name is NOT pointed at another server somewhere.** In the future, I'd like to update the script so that it can handle setting up a temporary site while you are migrating a site from another location to DigitalOcean.
