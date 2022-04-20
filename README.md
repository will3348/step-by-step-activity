# Step-by-step-activity
# To Create a React Web Application with Next.js
## Next.js
- Next.js is a framework that makes building React applications super easy to get started with. It's usually used to create static and server-rendered applications. The basic install will give you styling and routing out of the box.

- In the steps below, we'll show you how to get an application up and running.

- Make sure you have Node.js installed on your machine before proceeding.
### Create the Application
- To create a React application with Next.js, open a terminal window and create a new and empty directory:
- ``` mkdir your-app ```
- and cd into it:
- ``` cd your-app ```
- Then, install these dependencies in your project:
- ``` npm install --save next react react-dom ```
- When the installation is complete, open your package.json file and add this code to the "scripts" section:
-   ```Javascript
    {
    "scripts": {
      "dev": "next",
      "build": "next build",
      "start": "next start"
    }
    }
    ```
- Here's a quick rundown on what each script does:
  - dev: used to run the application when you're in development mode. This means your code will run with special error handling, hot-reloading, and other features that make the development process easier.
  - build: will compile your code into server and browser code that will run on a server in production.
  - start: how you start and run the production code in the production environment.
- The last thing you need to do is create your first page.
- Open a new file called index.js in the /pages directory of your project:
- ``` touch /pages/index.js```
- And add this code to the file:
- ``` JavaScript
  function Homepage() {
    return <div>Your Next.js Application</div>
  }

  export default Homepage
  ```
- Your application is ready to go! Now, all we need to do is run it!
### Run the Application
- To run your application, navigate to the root of your directory and run this command:
- ``` npm run dev``` 
- And you can preview your application at http://localhost:3000.
- To build the application for production, all you need to do is run the npm run build command we added to the package.json file. And then you can run it with the npm start command.
