# REACT 4
1. Explain the concept of dynamic routes in Next.js and how they differ from static routes.

- A dynamic route is a route that is generated from dynamic data. This means that the route path is not known ahead of time, but is instead generated at runtime , a dynamic route takes the id
- Static routes are the opposite of dynamic routes. They are routes that are known ahead of time, and their path does not change. For example, you could have a static route for the home page that is always /

2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?
- Connect GitHub Repository to Vercel: Once you have a Vercel account, log in to the Vercel dashboard at https://vercel.com/login. After logging in, click the "New Project" button.

- Import Project from Git: Select the "Import Project" option, and then choose the "From Git Repository" option.

- Authorize Vercel to Access GitHub: You may need to authorize Vercel to access your GitHub account if you haven't done it before.

- Select GitHub Repository: Vercel will list your GitHub repositories. Choose the repository that contains your Next.js application.

- Configure Project Settings: Vercel will prompt you to configure your project settings. Make sure to set the following:

- Framework Preset: Choose "Next.js" since we're deploying a Next.js application.
Root Directory: If your Next.js application is located in a subdirectory within the repository, specify the path here (e.g., "/my-next-app").
- Build Command: The command to build your Next.js application. The default is usually "npm run build" for Next.js.
Output Directory: The directory where the built application files will be located. The default is usually "out" for Next.js.
- Deploy: Click the "Deploy" button to start the deployment process. Vercel will fetch your Next.js application's code from GitHub, build it, and deploy it automatically.

- View Deployment: After a successful deployment, Vercel will provide you with a unique URL for your deployed Next.js application. You can visit this URL to see your application live.


3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application

- Next.js can serve static files, like images, under a folder called public in the root directory. Files inside public can then be referenced by your code starting from the base URL (/).
- You can also use the assetPath function to get the absolute path to a static asset

