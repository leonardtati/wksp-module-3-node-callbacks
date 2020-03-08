# Questions

**With a partner**, answer these questions as completely as possible. Feel free to look at past lecture notes, the web, anything. 

Take the time to explain it to each other. 

The power of this exercise is in the act of _formulating_ and _explaining_ the concepts to someone else (your teammate).

## One

Run the app. Write out the steps, the _pseudo code_, required to create this app. It doesn't have to be totally accurate, or in the right order.

Only move on to the next question when you have enough detail that you would be able to start coding it yourself.

```
// Answer here
/// set up the server
backend servers.js file
create views/pages/partials
///In the html create a form tag with the input text and the input submit button

///create the li box where the input goes

/create the css for style the button

//javascript
function every time you submit it creates a new line. this line's innerText=input.innerText



## Two - `server.js`

Take a look at the `server.js` file.

We have a new module in there, `body-parser` that is required on line `4`. What is it for? What is its use-case? What other lines are related to this module?

//body-parser extract the entire body portion of an incoming request stream and exposes it on req.body.

The actual definition of "parse" in Wiktionary is "To split a file or other input into pieces of data that can be easily stored or manipulated." So we are splitting a string into parts then recognizing the parts to convert it into something simpler than a string.

The bodyParser object exposes various factories to create middlewares. All middlewares will populate the req.body property with the parsed body when the Content-Type request header matches the type option, or an empty object ({}) if there was no body to parse, the Content-Type was not matched, or an error occurred.

_The NPM site might be a good place to start. Feel free to provide links as relevant._

```
// Answer here

```

## Three - `server.js`

Look at lines `23` and `24`. Explain the methods used. How are they different? What are the usecases for each?

```get the  telling ther server to get the data from .handlers page, where handleHOmePage is declared

POST and GET are two common HTTP Request used for building REST API’s. Both of these calls are meant for some special purpose.

As per the documentation GET request are meant to fetch data from specified resource and POST are meant to submit data to a specified resource.Post carries request parameter in message body which makes it more secure way of transferring data from client server in http protocol

// Answer here

```

## Four - `server.js`

Line `6`. That's new. What do you think it's for?

```
// Answer here

```to make server your server page cleaner

## Five - `handlers.js`

Explain line `1`. Where, why and how is `items` being used?

it's an empty array used in the handleHomePage handler to populate the list of the items with each new input the same way.

```
// Answer here

```

## Six - `handlers.js`

Why is there `redirect` on line `11`;

```
// Answer here

res.redirect is used to to redirect a request. the res to the req is stay on that page

``` 

## Seven - `handlers.js`

The `handle404` function is a more complex than we've seen thus far, what is the extra functionality for?

The req.accepts method checks if the specified content types are acceptable, based on the request’s Accept HTTP header field. The method returns the best match, or if none of the specified content types is acceptable, returns false (in which case, the application should respond with 406 "Not Acceptable").


```
// Answer here

```

## Eight - `ejs`

Take a look at `homepage.ejs` and `todoInput.ejs`. What is happening in there? Explain line-by-line...

including the header.ejs partial 
creating a div in which we include the todoInput.ejs

```
// Answer here

```

## Nine - `styles.scss`

What are lines `2` to `7` for this file? Where are these values being used? Take a look at `_homepage.scss` as well? What do you notice?

```
// Answer here

```

## Ten - `_homepage.scss`

Line `16`. See if by searching the Sass documentation, you can determine what _exactly_ is going on here. That `#{}` notation very specific to this use-case. Why?

```
// Answer here

```







