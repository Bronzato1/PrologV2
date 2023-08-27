---
title: "Dotnet Reliability With Azure"
image: '/images/dotnet-reliability-with-azure.png'
date: 2023-07-23
authors: [thierry]
description: Microsoft .NET is a reliable and robust developer platform that supports Windows, macOS, and Linux operating systems.
tags: [DotNet]
draft: false
---

 It has a set of best practices built on the Azure Well-Architected Framework that helps developers successfully migrate to the cloud and set a foundation for future modernization in Azure. The reliable web app pattern (RWA) is a part of this set of best practices that provides guidance on several business and technical objectives with focus on low-cost, high-value wins. It provides guidance on security, reliability design patterns, operational excellence, cost-optimized environments, and more.

The retry pattern is a technique for handling temporary interruptions in the service your code is trying to call. You expect these interruptions, or transient faults, to resolve themselves in a few seconds. The retry pattern handles transient faults by resending failed requests to the service. You can configure the amount of time between retries and how many times to attempt before throwing an exception.

The circuit-breaker pattern is another technique for handling temporary interruptions in the service your code is trying to call. It monitors for failures and trips a circuit breaker when failures reach a certain threshold. Once the circuit breaker is tripped, all further calls to the service are returned with an error without the need to make a request.