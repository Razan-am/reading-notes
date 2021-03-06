## **Application State with Redux**


### ***What are the advantages of storing tokens in “Cookies” vs “Local Storage”***

- Local Storage
   - **Pros: It's convenient.**

     - It's pure JavaScript and it's convenient. If you don't have a back-end and you're relying on a third-party API, you can't always ask them to set a specific cookie for your site.
Works with APIs that require you to put your access token in the header like this: `Authorization Bearer ${access_token}`.

  - **Cons: It's vulnerable to XSS attacks.**

     - An XSS attack happens when an attacker can run JavaScript on your website. This means that the attacker can just take the access token that you stored in your localStorage.

- Cookies
   - **Pros:** The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.

    - **Cons:** Depending on the use case, you might not be able to store your tokens in the cookies.

      - Cookies have a size limit of 4KB. Therefore, if you're using a big JWT Token, storing in the cookie is not an option.


### ***Explain 3rd party cookies.***

- Third-party cookies are created by domains that are not the website (or domain) that you are visiting. These are usually used for online-advertising purposes and placed on a website through adding scripts or tags. A third-party cookie is accessible on any website that loads the third-party server’s code.

### ***How do pixel tags work?***

- It’s a 1×1-pixel graphic used for tracking user behavior, site conversions, web traffic, and other metrics at a site’s server level. In other words, it is a tiny pixel-sized image, usually hidden, embedded in everything, from banner ads to emails.



-------------------------------------------------------------


## **Terms**

- **cookies**: Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

- **authorization**: Authorization is the process of giving someone the ability to access a resource.

- **access control**: Access control is a security technique that regulates who or what can view or use resources in a computing environment. It is a fundamental concept in security that minimizes risk to the business or organization.

- **conditional rendering**: Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition. This concept is applied often in the following scenarios:

   - Rendering external data from an API.
   - Showing or hiding elements.
   - Toggling application functionality.
   - Implementing permission levels.
   - Handling authentication and authorization.


----------------------------------------------

### ***worlds easiest guide to redux***

**What is Redux?**

  - Redux is a predictable state container for JavaScript apps.
  - It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger.

- While it’s mostly used as a state management tool with React, you can use it with any other JavaScript framework or library. 

- With Redux, the state of your application is kept in a store, and each component can access any state that it needs from this store.

**When to use Redux**

- Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app.

- Redux usually used when your app grows to the scale where managing app state becomes a hassle; and you start looking out for making it easy and simple.

**What is state management in Redux?**

- State management is essentially a way to facilitate communication and sharing of data across components. It creates a tangible data structure to represent the state of your app that you can read from and write to. That way, you can see otherwise invisible states while you’re working with them.

**How Redux works**

- The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

- There are three building parts: actions, store, and reducers.

**Actions in Redux**

- Simply put, actions are events. They are the only way you can send data from your application to your Redux store. The data can be from user interactions, API calls, or even form submissions.

**Reducers in Redux**

- Reducers are pure functions that take the current state of an application, perform an action, and return a new state. These states are stored as objects, and they specify how the state of an application changes in response to an action sent to the store.

**Store in Redux**

- The store holds the application state. It is highly recommended to keep only one store in any Redux application. You can access the state stored, update the state, and register or unregister listeners via helper methods.




-----------------------------------------------

**References:**

@By Michelle Wirantono/[LocalStorage vs Cookies: All You Need To Know About Storing JWT Tokens Securely in The Front-End](https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15id) 

@By cookiepro/[What is a Third-Party Cookie?](https://www.cookiepro.com/knowledge/what-is-a-third-party-cookie/)

@By Mike/[What Is a Tracking Pixel and How It Works?s](https://whatagraph.com/blog/articles/tracking-pixel)
