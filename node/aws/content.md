## Warning

Amazon Web Services has no cap on charges, so if a site you are hosting on AWS has a sudden surge in popularity then you could be hit with a large bill.  Similarly, if you leave a server running which you meant to terminate you will still be charged.

Finally you need to be **extra, extra careful** to keep your AWS keys secret and out of your Git repository.  If you suspect that you may have exposed your key you should revoke it immediately, and check that there are no servers running which you cannot account for.  If you aren't careful, you could [find yourself making a $3,493 mistake](http://vertis.io/2013/12/16/unauthorised-litecoin-mining.html).

## Build

[As you predicted](https://projects.thinkful.com/deployment-on-heroku-153/) your [Lorum Hodor app](https://gist.github.com/oampo/63f9f4d7f066d67a8d67) has become the hottest property on the web since [that thing which that guy from Twitter did](https://vine.co/).  To give you more control over your server setup, and allow you to scale your infrastructure even more quickly, you have decided to migrate from Heroku to [Amazon Web Services (AWS)](https://aws.amazon.com/).

## Milestones

### Milestone 1: Launch an instance

To complete this milestone you should sign up for AWS, then use the management console to launch a new EC2 instance.  The instance should be a `t2.micro` server running Ubuntu.  As well as the default security rule allowing SSH access to the server you should add a rule which makes HTTP over port 80 available anywhere.

You will be prompted to create a new key pair which will allow you to connect to the instance.  Download your private key, and keep it somewhere secure.  Then use SSH to connect to the machine by clicking the connect button, and following the instructions.

### Milestone 2: Set up Node & NPM

Use `apt-get` to synchronize the package index and install Node.js and NPM.  [Then fix the permissions for NPM](https://docs.npmjs.com/getting-started/fixing-npm-permissions).  You will need to add a symlink between `/usr/bin/nodejs` (where Ubuntu installs Node) and `/usr/bin/node` (where most libraries expect to find the Node executable) by running:

```
sudo update-alternatives --install /usr/bin/node node /usr/bin/nodejs 10
```

Create a new directory containing [the hodor app](https://gist.github.com/oampo/63f9f4d7f066d67a8d67) and install the dependencies.  Then test your installation by running code and making sure that there are no errors.

### Milestone 3: Set up nginx

Currently you can run your app on port 8080, but are unable to access the app from the outside world on port 80.  To allow this you are going to use the [nginx](http://nginx.org/) web server as a reverse proxy.

Install nginx using `apt-get`, then remove the default configuration at `/etc/nginx/sites-enabled/default`.  Create a new configuration at `/etc/nginx/sites-available/hodor` with the following configuration:

```
server {
    listen 80;
    location / {
        proxy_pass http://127.0.0.1:8080;
        access_log off;
    }
}
```

This tells nginx to pass all connections to port 80 to your app running on port 8080.  Enable the configuration by creating a symlink to `/etc/nginx/sites-available/hodor` from `/etc/nginx/sites-enabled/hodor`.  Restart nginx using `sudo service nginx restart`, then run your app.

Try visiting the app by visiting the IP address of your server from a browser.  You should see your Lorum Hodor.

### Milestone 4: Make it robust

If your app crashes or if your server needs to be rebooted then your app will stop running.  In this milestone you are going to set up [PM2](https://github.com/Unitech/pm2), a process manager which is designed to keep your app running no matter what happens.

To complete this milestone you should:

* Install PM2
* Start `hodor.js` running with PM2 using `pm2 start hodor.js`.
* Check that it is running using `pm2 list`.
* Save the current configuration using `pm2 save`.
* Make PM2 run on startup using `sudo pm2 startup -u ubuntu`.

Use the AWS dashboard to restart your EC2 instance.  Try visiting the IP address again.  You should see that your app is still running depite having restarted the server.

### Finishing touches

Don't forget to terminate your EC2 instance and the volume associated with it, if you don't intend on hosting the Hodor app in the long-term.
