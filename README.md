# nuxt-js-getting-started
A boilerplate SSR application using [Nuxt.js](https://nuxtjs.org/)

## Setup
Make sure you have [Node.js](nodejs.org) installed
### Install jekyo
```bash
npm install -g jekyo
```
### Sign In
Use the `jekyo user:signin` or `jekyo signin` to the Jekyo CLI
```bash
➜  ~ jekyo user:signin 
Your email?: **************
Your password?: **********
You have successfully signed in!
```
## Prepare your application
```bash
git clone https://github.com/jekyo/nuxt-js-getting-started
cd nuxt-js-getting-started
```
## Deploy your application
Create an application on Jekyo, which deploys your source code.
```bash
➜  ~ jekyo service:create
Service name?: nuxt-js-getting-started
service created!

```
Now deploy your application:
```
➜  jekyo deploy               
Enumerating objects: 32, done.
Counting objects: 100% (32/32), done.
Delta compression using up to 32 threads
Compressing objects: 100% (25/25), done.
Writing objects: 100% (32/32), 163.87 KiB | 11.71 MiB/s, done.
Total 32 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Debugger listening on ws://127.0.0.1:35565/e856ecd4-42ee-4e73-91ac-d99c733fd1a9
remote: For help, see: https://nodejs.org/en/docs/inspector
remote: Debugger attached.
remote: =============================================
remote: 👋 - Hello, x4139
remote: 🚀 - Launching getting-started onto the jekyo platform !
remote: =============================================
remote: 🔨 - Fetching source code for getting-started
remote: ------ Done.
remote: 🔨 - Building container for getting-started service. 🕐 This might take a while !
remote: ------ Done.
remote: 🔨 - Pushing container for getting-started service into the registry. 🕐 This might take a while !
remote: ------ Done.
remote: 🚀 - Deploying getting-started service on jekyo.
remote: =============================================
remote: 🎉 Deployment success !. Visit your app on: https://getting-started.jekyo.app
remote: Waiting for the debugger to disconnect...
To http://localhost:8000/api/repository/x4139/getting-started.git
 * [new branch]      master -> master
```
