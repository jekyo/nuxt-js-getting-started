# nuxt-js-getting-started
A boilerplate SSR application using [Nuxt.js](https://nuxtjs.org/)

# Tutorial: Deploying a NuxtJS app on Jekyo

### Prerequisites

Make sure you have [NodeJS](https://nodejs.org/en/download/), [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) and [git](https://github.com/git-guides/install-git) installed.

If it's your first time using **Jekyo**, you can **install** it by running the following command in your terminal:

`npm install -g jekyo`

### Sign in to Jekyo

You can sign in to Jekyo by running `jekyo user:signin`

```
➜  ~ jekyo user:signin 
Your email?: **************
Your password?: **********
You have successfully signed in!
```
If you don't have a Jekyo account, you can create one in the terminal by running `jekyo user:signup`.

### Create a basic NuxtJS app

You can start your NuxtJS project by using `jekyo create`

Using the **arrows** on your keyboard, select nuxt-js and press **enter**. 

```
? Select template
  None Creates only the application
❯ nuxt-js A boilerplate SSR application using [Nuxt.js](https://nuxtjs.org/) 
```
When prompted, enter the desired name for your NuxtJS app. 

`Application name?: app-name`

This will create a basic NuxtJS app in the current directory by cloning this [boilerplate NuxtJS app](https://github.com/jekyo/nuxt-js-getting-started)

```
Cloning source code... OK
Application created!
```
### Deploying the NuxtJS app

To deploy the app, first navigate to the newly created directory:

`cd app-name`

Now you can deploy this app to Jekyo by running: 

`jekyo deploy`

After a while, you should see something like this: 

```
➜  Fetching source code ... OK
➜  Building application, this might take a while ... OK
➜  Publishing application, this might take a while  ... OK
➜  Deploying application ... OK        
➜  Waiting for application to start ... OK
➜  Visit your app on: https://app-name.jekyo.app ... OK
```

You can now browse to your NuxtJS app https://app-name.jekyo.app

### Pushing local changes to Jekyo 

In this example, we will change the welcome message on our app.

Edit the 'Tutorial.vue' file found in **components** folder. 

```
<h2 class="text-2xl leading-7 font-semibold">
    Welcome to your Nuxt Application
</h2>
```
```
<h2 class="text-2xl leading-7 font-semibold">
    Welcome to your Nuxt Application on Jekyo
</h2>
```
Add the newly modified file to the git index by using [git add](https://www.atlassian.com/git/tutorials/saving-changes)

`git add components/Tutorial.vue`

Create a [git commit](https://github.com/git-guides/git-commit)

`git commit -m "your commit message"`

Now, simply deploy your app again:

`jekyo deploy`

You will see your changes on your live app after a short while. 
