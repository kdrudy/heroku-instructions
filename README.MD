##Heroku Instructions

`brew install heroku-toolbelt` to install the Heroku command line tools

`heroku login` to log in to your heroku account

To deploy go into your app directory and type the following:

`heroku create myapp` -- Creates a new project called myapp

`git push heroku master` -- Pushes the code in the project up to the app you just created

`heroku ps` -- Shows information about the currently running app

`heroku logs -t` -- Shows the logs of the current app


###Environmental Variables

Define them as config vars in your project settings page

Access them 1 of two ways.

1. `String variable = System.getenv().get("VARNAME");

2. In your application.properties using ${VARNAME}


###Database

Heroku allows you to provision a free tier of postgresql, the URL is at environmental variable ${JDBC_DATABASE_URL}


###Deploy from Github

If you want to deploy from your github repository you can set that up from the Deploy section of your App Dashboard

It can be set up to automatically deploy whenever you push to github.
