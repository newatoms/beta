# WebComponents: an easy way to make your business adaptable

How able you are to adapt your software will to some degree decide how able you will be to adapt your business. Having one singular architecture makes this significantly harder. Enter WebComponents.

## Every company is a software company

Almost every new web app that is built is either a Single Page App or a server side rendered one.

At New Atoms we build monolithic applications that: either have a single entry point that uses one set of data. One HTML file and one script backed by one big object in memory. Or: applications where every view is constructed by a more complex server process that mixes and matches the right bits for the right pages.

Your company is as adaptable as the software you use. Don’t get me wrong; I think these are valid architectures. Especially when you are doing a one-off project with a known and limited scope. I’ve been an avid user of frameworks including Backbone, Angular, Knockout and Ember.

Yet, in my experience, the reality of building software in this age is that you need to be:

* Adaptable
* Scalable
* Pivotable

Nowadays every company is a software company. And at the core of this, there is often a website and/or app. Whether it only impacts the way that people will reach out to you for a mere studio website or change the way that work comes to you.

## WebComponents to the rescue

WebComponents is not a framework; it is a core part of the HTML & CSS & JavaScript trinity and the way modern browsers work. It bundles structure & presentation & code for elements of your page, with their own scope and predictably reusable.

In short, this is how every browser has worked forever since HTML elements in the Document Object Model (DOM) are all components with their own meaning, styling and API’s. The modern WebComponents standardisation serves to provide uniform and open APIs for the way that browsers deal with this.

WebComponents will let you specify your own HTML elements. These custom elements can have their own semantic meaning, templates, their own styling and their own logic attached to them and exposed through an API. They can send HTML events and provide JavaScript methods to be used by the elements around it. They can inherit Styling or have their own.

## What is new

Next to the *single-page-app* and *server-side-rendered-app* WebComponents adds an exciting new architecture to the playground. We can use WebComponents to build a constellation of mini-apps that can be plugged and played to create a bigger application.

Something about this doesn’t sound new at all, after all, we have Directives in Angular, Components in React and Ember etcetera. Yet all of those require you to use those libraries, which are clearly designed to be used to develop a whole application.

WebComponents enable you to develop components in isolation as individual mini-apps with singular functionality. For instance showing a short profile of a user, the settings for an account, a self-validating email form that changes colour if invalid, a list of current projects etcetera.

Each component can have its own API, expose methods and fire events. Each component can use the global browser state through localStorage, cookies, etc. And each component can communicate on its own with the server to display the right state at the right moment.

This means you can use the elements that you create in any circumstance, use its API and events. WebComponents are easy to integrate into almost any web property that allows you to use HTML.

* Do you want to use your `user-chip` in a different app? No problem.

* Do you want to use your authentication form on another website? No problem. Do you want to recursively use an element within another instance of the same element? No problem.

WebComponents seldom work by themselves, although they just as well could. Every one of your components could work with its parents and its children to deliver the experience that is needed.

## From cores to constellations

These individual mini-apps are many times more portable than any other type of component. They can be reconfigured almost arbitrarily.

If your elements are not reliant on some specific app architecture, it will enable you to easily try out new things and be able to build new purpose built apps.

We’ve had cases where we have little mini-apps out of certain elements of one of our bigger apps, and where we’ve embedded some of our bigger apps into our other apps. Cases where we’ve taken an app and split it over multiple isolated navigations and the opposite.

## Distributed development at New Atoms

Our architecture is built on the notion that our organisation is a platform we develop, and can then use to create products on.

The idea here is that we build an operating system for our company. A layer of software that can connect the people and services in the company, and can expose certain functionality they offer to the outside world.

We believe that if the software is your operating system, the people need to be in control of that. This calls for everyone in the company to understand what the software does. This does not mean knowing how to develop it, but it does mean that people should have a basic literature of the code. This imposes methods of development that WebComponents can assist in greatly.

Most of our company processes are in (web)apps, and some in micro-services. Connecting all of this is a Firebase Real Time Database that we use to keep every one of these in Sync and to authenticate users.

## We develop elements to fit into this constellation.

All our elements contain the logic they need to function. They will get information from the server on their own and cache it with browser cache API’s. If they need to store local state, for instance, an authentication token, they will use global storage facilities like Cookies or localStorage for that.

For example, an element that displays a user and its avatar on our platform contains all the logic to get that information from the server and display it correctly. The server will just reply with an error if the element is not allowed to.

At first, we were all like ‘Holy smokes, but how the hell could we do with no global object’? It turns out that between the things that you want to be storing on the server with the user, the things that you want to store in the browser across sessions and the things that you need to store in your elements, there is really not that much left.

## Developing for divergence

In modern business, you are seldom going to know where you will be in two years. So to enable quick development and pivoting you want to create an open and flexible codebase.

By using Polymer’s element design principles, calling for uniform API’s on WebComponents and providing the tools to document their API’s and create the catalog of them, we’re able to quickly try out new applications or reconfigure existing ones for new needs.

For example, our `material-firebase-authentication` element, which contains the logic for authentication on all of our services and its interface elements, is developed to enable multiple use cases.

It allows you to choose what providers you want to offer to the user, and the interface will adapt to your selection. It enables you to make separate forms for signing up and in, or use the same form. It can display errors for you or you can handle errors yourself.

But perhaps most importantly, the authentication element authenticates your browser, not the app, to make server calls. So it doesn’t matter whether the form is on a different page, or within a complex app, or multiple times within a complex app. Wherever you use it, it will do its job.

This enables us to quickly integrate user authentication in any new project we make without batting an eye. If we want to try out something new on our API, we can quickly put together a mini app that can work perfectly in production as well.

## A library to pick from

We feel like we’re building a component library that actually enables you to think less about it when we add new elements. Where every element, through its limited scope, is easy to understand. And we believe this enables us to share the web development project with people who were, up to now, not involved.

And even in a small company like ours, being able to continue to build on what is there, as opposed to building something new with every new project, is a huge time saver.

When we want to do our sign in different for a different project, we find a way to build that into the login element, so that we have the ability to easily reuse it, or even switch an older app to newer thinking with the flick of an attribute.

---

New Atoms is an early stage journalistic company. We use WebComponents to build our apps. This enables us to easily share components and functionality between our properties and integrate the tools that we develop for ourselves and our clients to a very deep degree. We create individual elements that can stand on their own and come with their own documentation and their own API.
