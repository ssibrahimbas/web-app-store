# web-app-store
Get a more modern and less costly solution than search engine and ssr

## What is this project?

If you are a Web Developer, you know that lately most JavaScript frameworks have been developing on SSR (Server Side Rendering).

These;
 - React Server Components
 - NextJS
 - NuxtJS
 - Fresh by Deno

can be listed as.

Server Side Rendering provides you the following in general;
- Faster site initial launch
- Search Engine Optimization (SEO)

How do I get a faster site launch?
- Make your website PWA (Progressive Web Application) by adding a manifest file and a worker to your website and the first load will be much faster.

So what we will understand here is that SSR does not have a monopoly on the initial loading of the website.

So what is Search Engine Optimization?

Search engine optimization is the process of improving the quality and quantity of website traffic to a website or a web page from search engines. SEO targets unpaid traffic rather than direct traffic or paid traffic. (source: [Wikipedia](https://en.wikipedia.org/wiki/Search_engine_optimization))

Okey I understood. But we also use mobile applications in daily life. And we don't need any search engine here. What kind of solution is there on the mobile side?

There are app stores on the mobile site.

App developers to app stores;
  - application title
  - application category
  - application description
  - application images
  - application target audience

They publish their own applications by entering information such as.

Users can also sort and filter applications by popularity or category, both locally and globally. For example, shopping apps, social media apps, etc.

Hmm, I understand. So what is the connection between search engine and ssr?

The search engine scans your website before it is loaded and performs certain actions according to certain parameters to better serve the next search.
While doing this, if your website is doing Server Side Rendering, it will report faster and better. It also expects you to make good use of html elements.

Okay, so what kind of problem does SSR and Search Engine cause?

SSR has many problems in terms of development.
These;
  - JavaScript is developed for the browser side and can work with certain runtimes (Node, Deno etc.) on the Server. However, these runtimes are not 100% equal to web api's and there are some problems here.
  - If you are using the JavaScript Framework, you should also use a framework to run Server Side. Also, these frameworks are not 100% stable.
  - Server Side Frameworks use a system similar to file system routing, which was previously developed by php developers and proved to be unnecessary by everyone.
  - If you have developed the frontend and the backend seperately, since the user information must be included in the server when you render server side, session etc. for your frontend application. You will be dealing with processes and essentially your frontend app will be a monolithic app.
  - Since Javascript is dependent on a runtime when running Server Side, you have to run a runtime every second your application runs. This may seem like a minor issue, but when you use devops solutions like Docker it comes at various costs in terms of size and time.
  - In order for Search Engine to crawl your site well, you should pay attention to html elemtns and use meta atgs. You are not free.
  - Every time the Search Engine algorithm changes, you should understand the new developments and transfer them to your website.
  - When you want to make a dynamic optimization to Search Engine (for example, a product detail and user detail), maybe you will only request the values that you will use for the meta from the database.
  - You will keep unnecessary metadata in your database to server to Search Engine.

So how will the Web App Store solve the Search Engine problem?
  - Just like mobile applications, developers will include their own applications in the store.
  - Developers will have enetered a lot of metadata (category, target audience, description, title, image etc.) while including their applications in the store. In this way, categorization, sorting and searching will be easier.
  - Since there will be a control while the developers include their applications in the system, the chance of visiting spam sites will be much less.
  - You don't have to deal with SSR or Search Engine Optimization as the meta operations are done while the site is included in the Store. Write your JavaScript freely without using any SSR framework.
  - Your frontend becomes a real frontend in projects where you seperate backend and frontend, get rid of monolithic and try modern technologies without fear. eg microfrontends
  - You will be able to comment on the websites, so you will be able to see the experiences of people who have entered before.
  - You will be able to see when the website was established and what has changed with the last updates.

This is how I want to maximize the user and developer experience.

What isn't this project?

This project is not the end of Search Engine. Search engine doesn't just crawl website, it can crawl almost anything today. My goal with this project is to modernize the website development process.
