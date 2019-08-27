# Deploy Next to Netlify

Heroku is one of the static web hosts that cloud base. It can work intagrated with your For more information Visit [website](https://www.netlify.com/)

To deploy your project to Netlify follow the instructions below.

## Create account
- Create a [Netlify](https://www.netlify.com/) account
    - You can create an accout with popular git providers like Github, Gitlab or Bitbucket

## Create site from Git
- Click **New site from Git** button
- Select your git provider service, I use Github
- Select your application's repository
    - Here, you may need to manage which repositories Netlify can access

## Deploy settings
Let's configure deployment & building settings.

- Select **branch**
    - Until the production, I use develop branch as master. You can use your own branch here.
- Build command: **yarn run build && yarn run export**
- Publish directory: **out/**

Our deployment is done.

After deploy your site, you can make changes like site name, build & deploy settings, domain configurations in **Settings** tab in Netlify. 

## Change site name

In **General** tab
- Click **Change site name**
- Write your name and save

## Change build and deploy settings
In **Build&Deploy** tab
- Click *Edit settings* 
- Make your changes and save
