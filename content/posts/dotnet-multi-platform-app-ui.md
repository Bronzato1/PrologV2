---
title: .Net multi-platform App UI
subtitle:
date: 2022-08-16T09:57:35+02:00
draft: true
author:
  name: "Thierry Langie"
  link: "/about/"
  email: thierry.langie@skynet.be
  avatar: "/images/avatar.png"
description:
keywords: [dotnet]
license:
comment: false
weight: 0
tags:
  - dotnet
categories:
  - development
hiddenFromHomePage: false
hiddenFromSearch: false
summary:
resources:
  - name: featured-image
    src: featured-image.jpg
  - name: featured-image-preview
    src: featured-image-preview.jpg
toc: false
math: false
lightgallery: false
password:
message:
repost:
  enable: false
  url:

# See details front matter: https://fixit.lruihao.cn/documentation/content-management/introduction/#front-matter
---

MAUI means Multi-Platform App UI which is an open-source cross-platform framework. We can develop and build native Android, iOS, macOS, and Windows applications from a single code base using MAUI. This is an evolution of Xamarin.Forms, which extended from Mobile to Desktop application. If you are already worked on Xamarin.Forms, you can easily relate .NET MAUI.

## MAUI vs Xamarin Forms

The evolution of Xamarin forms will be integrated into the single. NET. With .NET 6, the native application development becomes a part of. NET. Single MAUI project is for all platforms is the most important advantage.

## Similarities between MAUI and Xamarin Forms

- We still can use XAML and C# to develop the applications
- We can choose MVVM, Reactive UI, Model-View-Update
- We can build Android, iOS, macOS, Windows desktop applications using the MAUI framework.
- If you already have experience with Xamarin, you can easily relate to MAUI.

## Who can use MAUI Framework

- Developers who want to build cross-platform applications using C# and XAML from a single code base.
- Across platforms to share the same UI layouts and designs, which saves more time in design implementations.
- Across the platforms, to apply the same business logic, code, and testing.

## MAUI Architecture

In a .NET MAUI app, we write code that primarily interacts with,

- The .NET MAUI API first
- Then the .NET MAUI directly consumes the native platform APIs
- App code may directly exercise platform APIs if required

.NET MAUI apps compiled into native app packages,

- Android apps built using .NET MAUI compile from C# into an intermediate language (IL) which is then just-in-time (JIT) compiled to a native assembly when the app launches.
- iOS apps built using .NET MAUI are fully ahead-of-time (AOT) compiled from C# into native ARM assembly code.
- macOS apps built using .NET MAUI use Mac Catalyst, a solution from Apple that brings your iOS app built with UI Kit to the desktop, and augments it with additional App Kit and platform APIs as required.
- Windows apps built using .NET MAUI use Windows UI Library (WinUI) 3 to create native apps that can target the Windows desktop and the Universal Windows Platform (UWP).

## Features of MAUI

.NET MAUI provides cross-platform APIs for native device features. Here are some good features provided by MAUI,

- Access to sensors, such as the accelerometer, compass, and gyroscope on devices.
- Ability to check the device’s network connectivity state, and detect changes.
- Provide information about the device the app is running on.
- Copy and paste text to the system clipboard, between apps.
- Pick single or multiple files from the device.
- Store data securely as key/value pairs.
- Utilize built-in text-to-speech engines to read text from the device.
- Initiate browser-based authentication flows that listen for a callback to a specific app registered URL.
- .NET MAUI includes support for .NET hot reload

## IDEs for Developing MAUI Application

- Visual Studio
- Visual Studio Code

Using these two IDEs, we can build native Android, iOS, macOS, and Windows applications using MAUI. 

Just coding is all we need, then choosing Visual Studio Code is a wise option.

### MAUI for Web Applications

There is an option to integrate the Blazor application into MAUI using WebView.
