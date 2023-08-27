---
title: Single Page Application
image: '/images/single-page-application.png'
date: 2023-03-01
authors: [thierry]
description: Being online and with a cell phone with our hands is so easy that often we don’t even stop to think about what kind of technology is helping us run this or that app. Usually, that’s not a problem – we don’t think about the electricity when we turn on the lights. However, when you face the decision to create an app for your business, then it’s conducive to understand what does SPA (single page application) means and how is it different from Multi-Page Applications (MPA).
tags: [Blazor]
featured: false
draft: false
---

Let's talk about what is Single Page Application (SPA), what benefits does SPA bring to users and businesses, how does it work with SEO, what are its pros and cons, and finally how SPA works with such technologies as Blazor, Angular, React.js, and Vue.js.

## Why Do We Need SPA ?

A single-page application is an app that doesn’t need to reload the page during its use and works within a browser. Think of the apps you use daily: Facebook, Google Maps, Gmail, Twitter, Google Drive, or even GitHub. All these are examples of a SPA. One of the best advantages of a correctly-configured SPA is the user experience (UX), where the user enjoys a natural environment of the app without having to wait for the page reloads and other things. You remain on the same page, which is powered by JavaScript programming language.

Before we go further, there are three abbreviations you’ll see in this article:

- SPA – single-page application (like we’ve mentioned above)
- MPA – multi-page application (a traditional app that loads new pages when you click a link)
- PWA – progressive web application (a website that is built using JavaScript or its frameworks and can act like an app, i.e., you can, for example, add it to your mobile phone homepage as an app)

## SPA Advantages

The main advantage of single-page applications is its speed. Most resources SPA needs (HTML + CSS + Scripts) are loaded at the launch of the app and don’t need to be reloaded during the usage. The only thing that changes is the data that is transmitted to and from the server. As a result, the application is very responsive to the user’s queries and doesn’t have to wait for client-server communication all the time.

Numerous studies by Google and key findings by companies such as Amazon and Wal*Mart show that if a page takes more than 200 milliseconds to load, it has the potential to ruin your business or, at the very least, cost you much money. For example, Amazon says that 1 second of additional delay in page load costs them 1% of sales (which, considering Amazon’s amount of sales, is $1.6 billion per year).

From a developer’s point of view, the creation of such an app is streamlined and optimized. You don’t need to write code to render the pages on the server. It’s not even really need a server to begin the development process. You can kick off from a file to get started. Besides, the developer can completely reuse the same backend server-side code and efficient API for the web application and a native mobile app. 

Single-page applications are excellent when you have a team of developers working together. It allows backend developers to focus on the API, while the frontend developers can pay more attention to creating the best user experience based on the backend API and implementing a beautiful user interface. 

Debugging a single-page application is also easy using the Chrome browser since it has special tools for Angular Batarang and React (the technologies used for SPAs.) Using a console, you can monitor network operations as well as investigate various page elements and associated data. 

Caching process is also quite efficient – the application sends only one request, stores all data transmitted, and can use this data. This is especially important at times when the user can have poor connectivity – s/he can still use your app since it’s synchronized with the server when the connection improves. 

We’ve mentioned Progressive Web Apps (PWA) above, and SPAs can easily be transformed into a PWA. In turn, this enables the developers to provide local caching and offer the offline experience to the clients and users.

## SPA Disadvantages

Despite all the advantages of the single-page applications, nothing is ever perfect. Let’s check out the times when the SPA can be not an ideal solution. What do we mean by single page application disadvantages? Single-page applications put a more significant load on the browser. For example, if your users have low power devices, they will have a poor app experience in terms of speed.

Additional problems with JavaScript arise because you have to make sure there are no memory leaks. Since the app can run for a long time – hours at a time (as opposed to the MPA, where the lifespan of a page was counted in minutes), you need to make sure your SPA doesn’t consume more memory than it needs. Otherwise, the pleasure of fast-loading pages will be destroyed by the sluggishness of unavailable memory on the user’s device. 

One more disadvantage of JavaScript is that users simply can have it disabled on their devices, and then you need to think of additional ways of how they can access the information on your website or your app without JavaScript. Another critical thing to remember about using or building a SPA is security. Due to cross-site scripting (XSS) and the fact that no new pages are loaded, hackers can gain access to your website and inject new scripts on the client-side. Therefore, if you are thinking about building a single-page application for your business, make sure you take the necessary precautions not to let this happen. 

Another security issue is the privacy of sensitive data. The initial page load should not contain any information that shouldn’t be available for all users. Since the entire SPA loads right away to the user’s device, you might accidentally give away data that should be behind a login or not available at all.

## SEO Optimization for SPA

SEO optimization is tricky when you have a single-page application, which is why we decided to dedicate a separate section to it in the SPA Disadvantages. It’s safer to use SPAs when you don’t rely on search engine optimization (SEO) as much, for example, if your app can only be accessed via a login. If you have a blog, on the other hand, it’s harder for the search engines to index your SPA website as opposed to traditional server-rendered pages. This is because the URL doesn’t really change, and different pages don’t usually have their URL addresses. 

Therefore, our advice to you: if you don’t want to bother with the URL settings, choose a framework that supports server-side rendering (SSR). Additionally, don’t use iframe windows, use static URLs, and optimize the scripts on your page to speed them up. Finally, make sure your pages have HTML5 for Google crawler to be able to access them.

You also should pay special attention to the server messages, especially the 200 and 404 errors.

## SPA Architecture

How do single-page applications work? Single-page application architecture is quite straightforward – it consists of the client-side technologies (at HUSPI, we rely on React.js, Angular, and Vue.js) and the server-side technologies (for which we usually use Node.js).

### 1. CLIENT-SIDE RENDERING (CSR)

The browser sends a request for HTML file from the server     
The server responds quickly with a simple HTML file with styles and scripts linked     
The user sees an empty page or some loader image while the js is executing     
The application fetches data, generates views, and injects into DOM     
Application is ready for use     
This might be an option for simple websites, but keep in mind that rendering the information on the client-side requires a lot of resources from the device and might overload the browser. As a result, this option might be the slowest of the three. At the same time, if you have a high-trafficked website, CSR would be better since it would present the information to the user without having to talk to the server too much.

Also, if you need social sharing options, keep in mind that all pages in CSR usually have the same open graph (og:) values, therefore you need to use either SSR or SSG.

### 2. SERVER-SIDE RENDERING (SSR)

The browser sends a request for HTML file from the server     
The server fetches all needed data, renders the application, and generates the app’s HTML file on the fly     
The user sees the available content     
The single-page application framework is what attaches events, generates a virtual DOM, and performs other actions     
Application is ready for use     
Server-side rendering is the option we rely on at HUSPI, because it combines both the speed of the single-page application and doesn’t overload the user’s browser, making the app fast.

### 3. STATIC SITE GENERATORS (SSG)

The browser sends a request for an HTML file from the server     
The server responds quickly with an already prepared HTML file     
The user sees the page     
The application fetches data, generates views, and injects it into DOM     
Application is ready for use     
Good and fast option, but remember that if you have dynamic content on your website, static site generators wouldn’t be your best friends because they are oriented more at static pages (as you could’ve already guessed from the name.)

## SPA AND ASP.NET (BLAZOR)

There’s a new kid on the block called Blazor. It’s a .NET framework that uses C#/Razor and HTML that runs in the browser with WebAssembly, according to the GitHub repository. Microsoft announced the release of this framework earlier in 2019 and currently, it looks like version 1.0 is ready. This serious backing from a large corporation is a great advantage of Blazor because it immediately makes this open-source instrument a part of the 60,000+ OSS contributors’ community with 3,700+ OSS company contributors.

Blazor is a convenient tool because there’s no need for TypeScript or JavaScript, you can write all logic in C#. That said, Blazor offers interoperability with JavaScript APIs and libraries, so if your ecosystem is large and consists of JS libraries, you’re not lost in the transition. .NET Blazor also offers two different options – client-only Blazor and server-side Blazor. The latter should be shipped with the .NET Core 3.0. Does it mean that Blazor will kill Angular, React, or Vue? We don’t think so. However, it is something to keep an eye on. For SPA using .NET, you can also use ASP.NET Core and ASP.NET MVC. How to create single page application in ASP.NET MVC? You set it up on the backend to serve the HTML on the frontend.
