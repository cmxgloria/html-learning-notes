# html-learning-notes
```html
<input type="email" placeholder="Your email">
<input type="submit">
```


-there are two types of URL link
Absolute: http://dash.ga.co/assets/logo.png
Relative: /assets/logo.png

-background link
background:url(“url”)

-input[type=”email”]=input[placeholder=”email”]

-`<header></header>`think as container to hold other elements, kind of like the body,but specifically for a website’s header

-<link>tag will let you include css from external file, especially a big project who has a lot of line code
-href is url where the css file live
-rel is we should always be set to the stylesheet
-display include inline and block
-`<article></article>` let us group together the multi html element that forms a single piece content
-margin: 0 auto; means all those wrap in the center(mean 0 on the top and bottom, auto on the left and right)
-@media (max-width: 500px){}--- use for different browser
-advance color--hex code and rgba(255,255,255,.5)
-`<button>like</button>`
-`<script></script>` write just above the close tag`</body>`
 This one is to see if it works `<script>alert("Javascript works!")</script>`
-`<script>$("button").on("click", function() { alert("clicked!") });</script>`

-$(element).on( event-type,thing-to-be-done )
-recap:
-the` <article>`tag is a semantic tag: it says something useful and defining, about its content.other semantic tags have fairly explanatory names like`<header><nav><footer>`
The `<div>` tag is not-semantic,which means it’s all-purpose: you can use it as container to group any type of content so it can be styled by a single bit of css.

-on the restaurant menu sample:
Add relative positioning to the div
Set the paragraph’s bottom to 0px,
Position the paragraph absolutely

-advanced layout
Block element include[ paragraph<p> header`<h1>`list`<ul><ol><li> `div`<div>`]
Inline element include[hyperlink`<a>image<img>form-fill<input>spans<span>`]
