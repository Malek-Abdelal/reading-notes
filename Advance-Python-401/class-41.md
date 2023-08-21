# class-41

## React 4

### Q: Explain the concept of dynamic routes in Next.js and how they differ from static routes

Dynamic routes in Next.js allow you to create pages with variable parts in the URL, enabling dynamic content generation. These pages are created when a user requests them, and you use placeholders like `[id]` in the URL structure. Static routes, on the other hand, involve fixed URLs with separate files for each page, and their content is pre-generated during build time. Dynamic routes are suited for frequently changing or user-specific content, while static routes are better for stable, unchanging content.

-------

### Q: Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

**Deploying a Next.js app involves:**

1. Building the app.
2. Choosing a platform (like Vercel, Netlify, Heroku).
3. Connecting your repo to the platform.
4. Configuring build settings and environment variables.
5. Deploying the app on the platform.
6. Configuring domains and SSL.
7. Testing and monitoring the deployed app.

Popular deployment platforms include Vercel, Netlify, Heroku, AWS Amplify, and DigitalOcean. These platforms simplify the deployment process by automating many of the steps, including build, deployment, scaling, and more.

--------

### Q: How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application. 

Next.js handles static file serving through the `/public` folder. This folder is the default location for storing static assets like images, fonts, and other files.

**Folder Structure:**

- Place static assets in the `/public` folder.
- For example: `/public/images/logo.png`

**Referencing Assets:**

- Reference assets in your code using the `/` as the root.
- For example: `<img src="/images/logo.png" alt="Logo" />`.

Next.js automatically handles the mapping of files from the `/public` folder to the root URL path, making static assets accessible directly through their paths.