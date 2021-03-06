
## Serverless App

This is a quick demo to show how serverless application work.
I have created a simple search photo form where user can search for any random photo of subject.
There is no server configure in backend. The front end search photo using unsplash API Service.

<p align="center">
  <a href="https://brave-goodall-db8079.netlify.app/">
    <img src="./media/serverless.gif" alt="Serverless Logo">
  </a>
</p>

---
 <p align="center">
    <a href="https://brave-goodall-db8079.netlify.app/">View Demo</a>
    ·
    <a href="https://github.com/riteshprk/serverless-functions/issues">Report Bug</a>
    ·
    <a href="https://github.com/riteshprk/serverless-functions/issues">Request Feature</a>
  </p>

## Implementing Serverless Architecture key points.

* Serverless computing takes the original promises of cloud computing and delivers true pay only for resources used with almost infinite scalability while hiding the details of how servers used and maintained.
* Serverless computing is a new cloud computing paradigm with enormous eonomic growth potential.
* Serverless computing allows the developer to focus on developing business logic and gives the cloud provider additional control over optimizing resources.



#### Tech Stack

| Stack    | -                                                                                                  | -                                                                                                 | -                                                                                                 | 
| -------- | -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | 
| FrontEnd | <p align="center"><img src="./media/html.png" width="100" height="100"> <br />HTML</p> | <p align="center"><img src="./media/bulma-logo.png" width="100" height="100"> <br />CSS Framework</p>  |  <p align="center"><img src="./media/js.png" width="100" height="100"> <br />JavaScript</p>  | 
| BackEnd  | <p>No backend :)</p>   | 


#### :rocket: Quick start
Create the project and function file
On your computer, create a new folder for the functions to live in:

## create a new folder
```
mkdir serverless-functions
```

## move into the new folder
```
cd serverless-functions/
```
Next, make a functions folder in the new folder:

## create a directory called functions
```
mkdir functions
```
Inside the functions folder, create a new file called hello-world.js—this will be your serverless function:

## create the file for your first serverless function
```
touch functions/hello-world.js
```
Inside hello-world.js, add the following code:
```
exports.handler = async () => {
  return {
    statusCode: 200,
    body: 'Hello world!',
  };
};
```

This is a complete serverless function. No joke. This JavaScript function returns an HTTP status code of 200 (for “OK”) and a plain text body of “Hello world!”

Now that we’ve created the serverless function, let’s get set up to test it locally.

Set up Netlify
First, install the Netlify CLI on your computer and log in to make sure that you have access to your Netlify account:

## install the Netlify CLI 
```
npm i -g netlify-cli 
```

## log into your Netlify account 
```
ntl login
```
Note: If you don’t already have a Netlify account, you can set one up for free using your GitHub, GitLab, Bitbucket, or email address in a few seconds.

Next, create netlify.toml at the root of your project:

## create a Netlify config file in the project root 
```
touch netlify.toml
```
Inside netlify.toml, configure Netlify Functions by adding two lines of config:
```
[build]
  functions = "functions"
```
This tells Netlify that you want to enable Netlify Functions and that it should look in the functions folder to find them. Once you’ve set this, Netlify will do the rest!

Start the server
You have access to a local development server called Netlify Dev that supports serverless functions. To run it, you’ll use the CLI:
```
ntl dev
```


---

Made with ❤️ and JS