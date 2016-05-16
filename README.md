# Deploying to Heroku From Nitrous

You've worked so hard these past two weeks to build an awesome web application, now it's time to share your product with the world! Deploying an application means taking the code you’ve written on your computer or Nitrous(locally), and uploading it to a server that runs continuously, so that your application is accessible to anyone on the internet. The process of deploying and maintaining applications on servers is known as DevOps.

To deploy your Ruby application, we’re going to be using Heroku, a cloud-based server. Follow these steps to deploy your application using Heroku’s servers:


## Creating a Free Heroku Account

First, let's create a free Heroku account. Go to [www.heroku.com](www.heroku.com) and click "Sign Up". Enter the desired information, then check your email to confirm the account. 

## Installing the Command Line Tool

Heroku has a command line tool which makes it super simple to deploy your application directly from your Nitrous terminal. Let's go ahead and install it. 
+ From your terminal, run `wget -O- https://toolbelt.heroku.com/install.sh | sh`. 
+ Next, we need to add the command to our path. From the same terminal window, run `echo 'PATH="/usr/local/heroku/bin:$PATH"' >> ~/.profile`. 
+ Finally, we need to reload our profile so our terminal knows about the heroku command. Run `source ~/.profile`. 

You should be all set - run `heroku version` - you should see something like this 
```bash
heroku-toolbelt/3.39.1 (x86_64-linux) ruby/2.1.5
You have no installed plugins.
```

### Deploy Your App!!

You're now ready to deploy your application! 
+ Navigate to your project’s folder, and type `heroku create` + a project name (for example, `heroku create my-cool-app`)
+ Add your heroku credentials.
+ Make sure you have added and committed your changes using git.
+ type `git push heroku master`
+ Sit back and smile OR Google your error!


<p data-visibility='hidden'>View <a href='https://learn.co/lessons/hs-deploying-to-heroku-with-nitrous' title='Deploying to Heroku From Nitrous'>Deploying to Heroku From Nitrous</a> on Learn.co and start learning to code for free.</p>
