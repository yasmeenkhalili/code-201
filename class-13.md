# “The Past, Present, and Future of Local Storage for Web Applications”

persistent local storage is one of the areas where native client applications have held an advantage over web application.

For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

These values may be stored in the registry, INI files, XML files, or some other place according to platform convention.

Cookies have three potentially dealbreaking downsides:

* Cookies are included with every HTTP request, thereby slowing down our web application by needlessly transmitting the same data over and over

* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless our entire web application is served over SSL)

* Cookies are limited to about 4 KB of data — enough to slow down our application (see above), but not enough to be terribly useful

What we really want is:

* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server
![cookies](https://images.slideplayer.com/39/10864762/slides/slide_30.jpg)

## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount.

Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain.

AMASS (AJAX Massive Storage System) is a prototype of a Flash-to-JavaScript bridge 

Flash gives each domain 100 KB of storage “for free.” Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.

Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage
could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

![html](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7f/HTML5_APIs_and_related_technologies_taxonomy_and_status.svg/420px-HTML5_APIs_and_related_technologies_taxonomy_and_status.svg.png)

## INTRODUCING HTML5 STORAGE

“HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.”

it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after we navigate away from the web site, close our browser tab, exit our browser, or what have we.

From our JavaScript code, we’ll access HTML5 Storage through the localStorage object on the global window object. Before we can use it, we should detect whether the browser supports it.

We can use Modernizr to detect support for HTML5 Storage.

![](http://technobytz.com/wp-content/uploads/2014/05/html5-web-storage.jpg)

## USING HTML5 STORAGE

HTML5 Storage is based on named key/value pairs. 
* We store data based on a named key, then we can retrieve that data with the same key. 
* The named key is a string. 
* The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. 

![](https://lh3.googleusercontent.com/proxy/HSjPJPOVsQQNSLKruAQmGlHlZ7KZFIXxQPjFMVm-LvhcxdcUUeKsEM9vVuC3t51BHHvkCfvNuVVJ3UwOr5zkYJDN7nuroU_Ij8bTD3fHZ78RceQV8U8n1w)

## TRACKING CHANGES TO THE HTML5 STORAGE AREA

If we want to keep track programmatically of when the storage area changes, we can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.

The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9).

## LIMITATIONS IN CURRENT BROWSERS

“5 megabytes” is how much storage space each origin gets by default.

Each digit in that float is being stored as a character, not in the usual representation of a floating point number.

 Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that we as a web developer can build into our web application.


In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite.

Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing us to do things like this from JavaScript:

openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});

There’s Oracle’s SQL, Microsoft’s SQL, MySQL’s SQL, PostgreSQL’s SQL, and SQLite’s SQL. Indeed, each of these products adds new SQL features over time, so even saying “SQLite’s SQL” is not sufficient to pin down exactly what we’re talking about. We need to say “the version of SQL that shipped with SQLite version X.Y.Z.”

The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. There are “databases” with “records,” and each record has a set number of “fields.” Each field has a specific datatype, which is defined when the database is created. We can select a subset of records, then enumerate them with a “cursor.” Changes to the object store are handled within “transactions.”

![](https://1.bp.blogspot.com/-938sYRmfH1Q/VqpbdlJp0EI/AAAAAAAAC6g/DOAaR8ihhnE/s1600/6029OT_06_03.png)

