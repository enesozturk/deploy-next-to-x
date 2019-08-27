# Deploy Next to Heroku

ZEIT Now is a cloud platform for static sites and serverless functions. It enables developers to host websites and web services that deploy instantly, scale automatically, and requires no supervision, all with no configuration. For more information Visit [website](https://zeit.co/)

## Create account

Login to Zeit Now with your Github or Gitlab account [here](https://zeit.co/login)

## Install Now

To deploy with Now, you need to install Now CLI, let's install it with npm

```
npm i -g now
```

## Login

With Now CLI installed, you can now login using the following command 

```
now login
```

Now will send you a confirmation mail, click *Verify* to complete login

## Development

"For a seamless local development experience, you should use *now dev*." Now says.

You can start developing with now:

```
now dev
```

After installing your dependencies your app will start from localhost

## Project Settings

Make sure your Next js app have these scripts in *package.json*
```
{
  "scripts": {
    "dev": "next",
    "build": "next build",
    "start": "next start"
  }
}
```
    
## Deploy

To deploy your Next app to Now, you can use this simple command

```
now
```

After your project has been built and deployed, you will receive a deployment URL with the following format:

```
project-name.account-name.now.sh
```


