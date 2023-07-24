---
title: Mobile Blazor bindings
image: '/images/blazor-ready.jpg'
date: 2023-03-13T08:43:22+02:00
authors: [thierry]
description: Blazor is a Web UI framework based on .Net and C# instead of JavaScript. As you know .Net has a great support for building server rendered web apps for a long time with Asp.Net and Asp.Net Core. But previously if you wanted to do anything in the browser that meant writing some JavaScript. Blazor enables you to add client-side functionality and interactivity to your Asp.Net Core web apps using just .Net. No JavaScript required.
tags: [Blazor]
featured: true
draft: true
---

With Blazor you can use your existing .Net skills and code to do full stack web development. Blazor is based purely on open web standards and works in any modern web browser. No browser plugins required. Blazor is part of Asp.Net Core your modern web framework for .Net. Asp.Net Core comes with everything you need to build beautiful web UI and powerful backend services. The addition of Blazor to Asp.Net Core expands the reach of your .Net web apps to the client. There is no need to rewrite your existing Asp.Net Core apps to take advantage of Blazor. You can add Blazor components to your existing apps while preserving existing functionalities. Getting started with Blazor is super easy. You just go to blazor.net and install the latest .Net SDK. You can then develop on the platform of your choice using Visual Studio, Visual Studio for Mac or Visual Studio Code.

Now what if building a web app is insufficient ? What if you need more than what the web platform offers you and you require full unfiltered access to the client device's native capibilities ? Well .Net has many great options for building native client apps. But if you are a web developer, one compelling option might be to build a hybrid app.

## What is a hybrid app ?

Hybrid apps are native apps that leverage web technologies for their functionality. For example, a hybrid app might use an embedded WebView control to render web UI. This means you can write your app UI using web technologies like HTML and CSS while also leveraging native device capabilities. For web developers, building hybrid apps has many benefits. You can reuse your existing web development skills, you can reuse your existing code you might even be able to reuse your entire web app to build native applications. You get full access to the native capabilities of the device including native UI elements together with your web UI. 

Now not every app needs to be a hybrid app but for many scenarios, the hybrid model can significantly reduce app development time. You can buid hybrid desktop and mobile apps with .Net and Blazor. Blazor hybrid apps combine all the benefits of the web, native apps and the .Net platform. In a Blazor hybrid app, your Blazor components run natively on the device. They don't run in the browser and WebAssembly is not involved. This means your Blazor components run fast and they have full access to the native capabilities of the device through the .Net platform. Your components then render to an embedded WebView control through a local interop channel.

Mobile Blazor Binding enables hosting Blazor components in a Xamarin Forms app. Your Blazor components run natively on .Net using Xamarin and have full access to the native functionality through .Net APIs including Xamarin Essentials. Your Blazor components render to a WebView control provided by the underlying platform and you can add native UI controls too.
