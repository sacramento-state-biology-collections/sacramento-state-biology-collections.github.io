---
title: "Understanding Progressive Web Apps"
date: 2022-10-11T17:53:32-07:00
draft: false
toc: false
---

## What is a Progressive Web App?

Progressive Web Apps (PWAs) are a new way to build web applications that are fast, reliable, and engaging. They are a combination of web technologies and best practices that allow users to install a web application on their mobile device or desktop.

## Why PWAs?

PWAs use web-platform technologies to deliver an app-like experience to users. Technologies like Service Workers, Web App Manifests, and Push Notifications allow PWAs to provide a native-like experience to users. PWAs are also discoverable, installable, linkable, and shareable. In combination with *Progressive Enhancement*, PWAs are a great way to build web applications that work for everyone. 

### Architectural Patterns for PWAs

There are two main architectural patterns for PWAs: Single Page Applications (SPAs) and Multi-Page Applications (MPAs).

---

SPAs are built using a single HTML page and JavaScript to dynamically update the page. 

> Pros
> - Mostly atomic in-page updates.
> - Client-side dependencies loaded on start-up.
> - Subsequent loads are fast, because of cache usage.

> Cons
> - High initial load cost.
> - Performance depends on device hardware and network connection.
> - Additional app complexity is required.

---

MPAs are built using multiple HTML pages and JavaScript to dynamically update the page. 

> Pros
> - Mostly full-page updates.
> - Initial render speed is critical.
> - Client-side scripting can be an enhancement.

> Cons
> - Secondary views require another server call.
> - Context doesn't carry over between views.
> - Requires a server or pre-rendering.

SPAs are more performant than MPAs, but MPAs are easier to develop and maintain.

### The Power of Service Workers!

The service worker is a script that runs in the background of a web application. It is a JavaScript file that can intercept network requests, cache resources, and push notifications to the user. Service workers are a great way to provide a native-like experience to users. Also, the service worker has a lot of power beyond basic routing, cache management, and networking as it can be used to provide offline support, background sync, and many more complex features.

### The Web App Manifest

The Web App Manifest is a JSON file that tells the browser about your web application and how it should behave when installed on the user's mobile device or desktop. The Web App Manifest provides information about the name of the app, the icons that should be used, and the URL that should be opened when the app is launched. The Web App Manifest also provides information about the app's theme color and display mode.

### Offline Support

Offline support is a great way to provide a native-like experience to users. Offline support allows users to access your web application even when they are offline. Offline support is achieved by caching resources using a service worker.

### Background Sync

Background Sync allows users to continue using your web application even when they are offline. Background Sync allows users to make changes to their data while offline and the changes will be synced to the server when the user is online.

### The PWA Checklist

The PWA Checklist is a great way to ensure that your web application is a PWA. The PWA Checklist provides a list of requirements that a web application must meet to be considered a PWA.

### External Resources

{{< youtube sFsRylCQblw >}}
---
{{< youtube ppwagkhrZJs >}}

---

## Final Thoughts

A PWA is a great way to build web applications that are fast, reliable, and engaging. A PWA is a combination of web technologies and best practices that allow users to install a web application on their mobile device or desktop. With tools to check if a web application is a PWA, it is easy to ensure that your web application is usable to everyone. Starting out with a PWA also allows for less server-side code thus reducing the cost of hosting your web application.