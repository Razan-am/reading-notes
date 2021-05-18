# **Local Storage**

## ***“The Past, Present, and Future of Local Storage for Web Applications”***

- Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

  - Cookies are included with every `HTTP` request, thereby slowing down your web application by needlessly transmitting the same data over and over.
  - Cookies are included with every `HTTP` request, thereby sending data unencrypted over the internet.
  - Cookies are limited to about 4 KB of data — enough to slow down your application, but not enough to be terribly useful.

- What we really want is

  - a lot of storage space on the client that persists beyond a page refresh and isn’t transmitted to the server.

**A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5**
- Microsoft invented a great many things and included them in their browser, Internet Explorer. One of these things was called `DHTML Behaviors`, and one of these behaviors was called `userData`.
- `userData` allows web pages to store up to `64 KB` of data per domain, in a hierarchical XML-based structure.
- In 2002, `Adobe` introduced a feature in `Flash 6` that gained the unfortunate and misleading name of `Flash cookies`.It allows Flash objects to store up to `100 KB` of data per domain. 
- By 2006,  `Flash 8` with accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker `dojox.storage`. Flash gives each domain `100 KB` of storage `for free`. Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

- By 2009, `dojox.storage` could auto-detect and provide a unified interface on top of `Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5` storage that was only implemented in older versions of Firefox.

**INTRODUCING HTML5 STORAGE**
- `HTML5 Storage` is a specification named Web Storage,certain browser vendors also refer to it as `Local Storage` or `DOM Storage`.

**what is HTML5 Storage?**
-  It’s a way for web pages to store named `key/value` pairs locally, within the client web browser,like cookies.

>this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.

**USING HTML5 STORAGE**
- It's store data based on a `named key`, then you can retrieve that data with the `same key`,the named key is a `string`. The data can be `any type supported by JavaScript`, including `strings, Booleans, integers, or floats`. 
>the data is actually stored as a string. 

- `Calling setItem()` with a named key that already exists will silently overwrite the previous value. 
- `Calling getItem()` with a non-existent key will return null rather than throw an exception.

>Like other JavaScript objects, you can treat the localStorage object as an `associative array`,instead of using the `getItem() and `setItem() methods`, you can simply use `square brackets`.

>Example:

`var foo = localStorage.getItem("bar");`

`localStorage.setItem("bar", foo);`

`…could be rewritten to use square bracket syntax instead:`

`var foo = localStorage["bar"];`

`localStorage["bar"] = foo;`

- `Calling removeItem()` it's a methods for removing the value for a given named key, and clearing the entire storage area that is deleting all the keys and values at once.

>Example:

`interface Storage {`

  `deleter void removeItem(in DOMString key);`

  `void clear();`

`};`

>Calling removeItem() with a non-existent key will do nothing.

-  Calling `key()` it's a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

>EXample:

`interface Storage {`

  `readonly attribute unsigned long length;`

  `getter DOMString key(in unsigned long index);`

`};`

>If you call key() with an index that is not between 0–(length-1), the function will return null.

**HTML5 STORAGE IN ACTION**
- HTML5 Storage, can save the progress locally, within the browser itself even if you close the browser tab, then re-open it,the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected.

**References:**

@ MMIX–MMXI Mark Pilgrim /[Local Storage
](http://diveinto.html5doctor.com/storage.html)