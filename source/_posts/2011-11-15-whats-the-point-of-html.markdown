---
layout: post
title: "What's the point of HTML?"
date: 2011-11-15 22:44
comments: true
categories: 
---

I'm a big fan of code separation and the <a href="http://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller">MVC</a> pattern. As we slowly move towards a world where everything is a web app, I think forcing the model of MVC on most frameworks has been the greatest move towards clean code that we'll see for a while.

But lets look at the View portion of MVC. What is the View for a web app? Most people would say it's the html file that gets sent back to the browser. This is close to the truth, but clearly breaks down once you start considering javascript. A View shouldn't be self modifying, able to handle events, etc.

The truth is that web apps don't run on servers, they run in the browser. The cases are few and far between of useful web apps that don't require javascript. Once you consider javascript, our MVC paradigm breaks.

The truth is, in the browser, we have our own MVC. In an ideal world, the Model is HTML, the View is CSS, and the Controller is Javascript. In practice, HTML is so ingrained into browser rendering, that it's impossible to separate from the View. As a Model, HTML documents are rather lacking. No one wants to store anything that's not being rendered in the HTML structure, as it's not easy to work with.

Perhaps it's time to give up on HTML being a source of clean data, and to accept it's role as part of the view. How then do we achieve proper code separation in our web pages? How do we enable the semantic web when our fundamental form of document is rendering information and not data? The answer is to pull your data from an API. Look at Twitter; Loading up their webpage gives an HTML page with no data. Javascript on the page consumes an API, and passes it into HTML for rendering. If you're interested in a clean form of the data itself (the Model from which the page is built), you can grab it from the API(In my case: <http://api.twitter.com/1/statuses/user_timeline.json?include_entities=1&include_available_features=1&contributor_details=true&pc=false&include_rts=true&user_id=243506131>).

Looking at HTML this way allows us to not feel guilty about non-semantic divs, and not knowing the right microformat for calendar events.

What we do need to make sure of is that our new html pages don't lock up data, that there is an API for everything, and that it is publically accessible. After all, people only are scraping your HTML for information if it's not available in a better form.