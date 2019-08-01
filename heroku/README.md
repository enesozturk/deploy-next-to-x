# Deploy Next to Heroku

Heroku is one of the Cloud Platform as a Service that you can deploy your applications written by any language like Javascript, Go, Python, Ruby etc. in seconds. For more information Visit [website](https://www.heroku.com/)

## Create account

- Create a [Heroku](https:///Users/enesozturk/Desktop/deploy-next-to-x/netlify/README.mdwww.heroku.com/) account and login

## Heroku CLI

- Install [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) for your OS
    - Heroku CLI let us manage all steps on terminal

## Login

1. Login Heroku
    - `heroku login`
        - Heroku cli will open up browser to login via their website, enter your cridentals and login


## Create Heroku App
1. Go to your project folder
    - `cd /your/project/path`
2. Create a Heroku app
    - `heroku create my-heroku-app`
        - This command will craete a heroku app named with *my-heroku-app* that you can see it in your [Heroku Dashboard](https://dashboard.heroku.com/apps)

## Project Settings


Make sure your Next js app have these scripts in *package.json*
```
{
  "scripts": {
    "dev": "next",
    "build": "next build",
    "start": "next start -p $PORT"
  }
}
```

1. If you don't have git in your project, create first 
    - `git init`
    - `git add .`
    - `git commit -m "initialize commit"`

- Initialize remote heroku for the project
    - `heroku git:remote -a my-heroku-app`
    
## Publish Project

Lastly, push your changes to heroku via git
- `git push heroku master`

That's all.

Your app is running on https://my-heroku-app.herokuapp.com


