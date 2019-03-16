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
-float let you slide the content of the `<span>`,more let you slide the image inside its container element
-two kinds of gradients(radial and linear)

-the css property called ’transition ’ to instruct the paragraph that anytime its height changes, it should build in a half-second delay.(do all together due to different browsers)
eg. transition: height .5s;
  -webkit-transition: height .5s;
  -moz-transition: height .5s;

- <script>
        $('div').on('click', function () {
            $(this).toggleClass('show-description');
        });
    </script>
    
    
 #HTML QUESTIONS FROM GA
 1, what is link and anchor element different?
The HTML External Resource Link element (<link>) specifies relationships between the current document and an external resource. This element is most commonly used to link to stylesheets, but is also used to establish site icons (both "favicon" style icons and mobile home screen/app icons) among other things.
Eg. <link href="/media/examples/link-element-example.css" rel="stylesheet">
Eg.  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">

The HTML <a> element (or anchor element) creates a hyperlink to other web pages, files, locations within the same page, email addresses, or any other URL.
<a href="https://example.com">Website</a>

2.
<th>morning</th>
<td rowspan=”2”>work</td>
<td rowspan=”3”>relax</td>
<td colspan=”2”>work</td>
Eg
<thead>
    <tr>
      <th colspan="2">
    <h1>Wine Festival Schedule</h1>
        </th>
      </tr>
    <tr>
      <th> <h2>Time</h2></th>
      <th><h2>Event</h2></th>
    <h2></h2>
    </tr>
    </thead>
显示出来结果
Wine Festival Schedule（这个会显示在中间）
TIME 	EVENT

------<label for="user-pw">Password:</label>
        <!--Add your code below-->
 	<input id="user-pw" type="password" name="user-pw">
Password同一行只有一个
如果<input id="user-password" type="password" name="user-password">
Password同一行就有两个


3.There are different types of validation. One type is server-side validation, this happens when data is sent to another machine (typically a server) for validation. An example of this type of validation is the usage of a login page. The form on the login page accepts username and password input, then sends the data to a server which checks that the pair matches up correctly.
On the other hand, we use client-side validation if we want to check the data on the browser (the client). This validation occurs before data is sent to the server. Different browsers implement client-side validation differently, but it leads to the same outcome.
 
4. How to change google image to a link which css accept format

## HTML STUDY NOTES FROM GA
HTML stands for HyperText Markup Language:
HTML is composed of elements. These elements structure the webpage and define its content.
1.Why would raw text need a structure?
---developers can create a hierarchy of information which serves several purposes
it allows users scanning a site to quickly pick out the most important ideas.
it helps visually impaired users navigate the content of a page using special software.
it helps search engines pick out important keywords that might otherwise get lost in a sea of text.
2.What type of content might an HTML element contain?
As you will learn, <p>, <div>, and <span> elements can contain text whereas elements like <ul> or <ol> should only contain <li> elements as direct children.
Block level tags like the <div> can contain all tags that can exist within the <body> (in other words, we can nest other elements within a <div>) whereas self-closing tags like <img> can not contain any content at all!

3.Do tags themselves count as content?

The content is just the information contained within the tags themselves.
 For example, the <img> tag is an example of a self-closing tag and it introduces content into the page differently than the <p> element.

4.Is there a sentence or a word element?
use an element like <span>, <em>, or <strong> to more specifically target content.

5.Why does the browser need information about the type of raw text it will display?
The browser needs this information so that it can give text meaning within the larger context of the document. In other words, the browser uses this information not only for rendering purposes but also so that it can create a structure which other programs (screen readers for example) can interpret.

6.Codecademy says that a markup language like HTML “defines structure and presentation of raw text”. Doesn’t CSS define the presentation of web content?
These days HTML is best categorized as a descriptive markup language which encourages developers to focus on the semantic meaning of information rather than its visual appearance. However, there are other markup languages which make no such separation of concerns. In fact, HTML used to be more presentational before the advent of CSS.

7.In this exercise 613, why does the paragraph display on the page but the title “My Coding Journey” does not?
Answer
The site <title> does not display on the page because this information is contained within the document’s <head>. Unlike the body element, the <head> element contains metadata which will not be displayed by the browser. You will learn more about the head and title elements in lesson 2 so stay tuned!

8.What is a web browser?
Answer
A browser is a piece of software which allows us to display content on the web (among other things). The most popular web browsers today include Chrome, Firefox, Safari, and Edge. In this lesson, the HTML that you write will be displayed in the emulated browser in the right of your workspace.

9.Question
In steps 1 and 2 of this exercise, both <p> elements display in the same exact way. As it doesn’t seem like anything special happened here, what is the point of nesting the <p> element in a <div> element?
Answer
In this case, this is done purely for demonstrative purpose. In the future you will find that <div> elements are often used to group related content. This can serve to give a page some added structure and to allow for more modular styling.


10.Question
This exercise 143 says that child elements can inherit from their parents. What sorts of things can child elements inherit from their parents?
Answer
When you dive into our CSS course you will learn that child elements inherit most of their styling from their parent elements. In other words, most styles cascade down from parents to children.

11.How does the browser know what language other documents are written in? For example, why doesn’t css need a doctype?
Answer
DOCTYPE declarations are only required for html based documents. Other JavaScript or CSS files are actually loaded into the page with <link> or tags. These tags signify the file type to the browser thereby allowing the browser to properly parse the file.

12.Without the html tags mentioned in this lesson, in what ways might the browser misinterpret our HTML code?
Answer
The <html> tag is actually an example of an optional tag which means that there are situations in which it can be omitted. Even though omitted optional tags will be inserted into the document by the browser and may not always be required, most developers would say that it is best practice to include these tags. Including optional tags enhances readability, improves cross-browser support, and takes some burden off of the browser.
In short, while the <html> tag can be omitted I do not believe it should be omitted.

13.Why does the browser need metadata about the page?
Answer
There exists different categorizations of metadata but most generally metadata is “data about data”. While the browser doesn’t need most metadata it does often use metadata to enhance the user experience in some way. Metadata not displayed on a page but behind the scenes it can be used by other software (web crawlers, search engines, browsers, etc.) to process, encode, extract or index all sorts of interesting information (geographic coordinates, calendar events, contact info, etc.). What’s more, businesses are often interested in using metadata to improve SEO or Search Engine Optimization.


TABLE
--There are many websites on the Internet that display information like stock prices, sports scores, invoice data, and more.
--The HTML <tr> element defines a row of cells in a table. The row's cells can then be established using a mix of <td> (data cell) and <th> (header cell) elements.

Sample
<!DOCTYPE html>
<html>
<head>
  <title>Ship To It - Company Packing List</title>
  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
<body>

  <ul class="navigation">
    <li><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-9/htmlcss1-img_logo-shiptoit.png" height="20px;"></li>
    <li class="active">Action List</li>
    <li>Profiles</li>
    <li>Settings</li>
  </ul>

  <div class="search">Search the table</div>

  <table>
    <thead>
      <tr>
        <th>Company Name</th>
        <th>Number of Items to Ship</th>
        <th>Next Action</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th>Adam's Greenworks</th>
        <td>14</td>
        <td>Package Items</td>
      </tr>
      <tr>
        <th>Davie's Burgers</th>
        <td>2</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Baker's Bike Shop</th>
        <td>3</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Miss Sally's Southern</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Summit Resort Rentals</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Strike Fitness</th>
        <td>1</td>
        <td>Enter Order</td>
      </tr>
      </tbody>
  </table>

</body>
</html>
 Run as below
Search the table
COMPANY NAME
NUMBER OF ITEMS TO SHIP
NEXT ACTION
Adam's Greenworks
14
Package Items
Davie's Burgers
2
Send Invoice
Baker's Bike Shop
3
Send Invoice
Miss Sally's Southern
4
Ship
Summit Resort Rentals
4
Ship
Strike Fitness
1
Enter Order


Sample 2
To add titles to rows and columns, you can use the table heading element: <th>.
<table>
  <tr>
    <th></th>
    <th scope="col">Saturday</th>
    <th scope="col">Sunday</th>
  </tr>
  <tr>
    <th scope="row">Temperature</th>
    <td>73</td>
    <td>81</td>
  </tr>
</table>

---row - this value makes it clear that the heading is for a row.
col - this value makes it clear that the heading is for a column.
--Question
This exercise discusses the scope attribute. What is the purpose of the scope attribute and are row and col the only values this attribute can have?
Answer
The scope attribute is used by screen readers to enhance accessibility for visually impaired users. In addition to the row and col values shown in this exercise, the scope attribute can also have the following values:
rowgroup: used for table headings that group multiple rows.
colgroup:used for table headings that group multiple columns.
auto: the default value
In lessons 8 and 9 you will learn how to create cells that span multiple rows or columns. For improved accessibility, we should use the appropriate rowgroup and colgroup values within these headings.

Sample
1.<tr>
  <td>Davie's Burgers</td>
  <td>2</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Baker's Bike Shop</td>
  <td>3</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Miss Sally's Southern</td>
  <td>4</td>
  <td>Ship</td>
</tr>
<tr>
  <td>Summit Resort Rentals</td>
  <td>4</td>
  <td>Ship</td>
</tr>
<tr>
  <td>Strike Fitness</td>
  <td>1</td>
  <td>Enter Order</td>
</tr>
---
Davie's Burgers
2
Send Invoice
Baker's Bike Shop
3
Send Invoice
Miss Sally's Southern
4
Ship
Summit Resort Rentals
4
Ship
Strike Fitness
1
Enter Order



Question
Why should we use CSS rather than HTML to create borders for our tables?
Answer
Within software engineering, there is a design principle known as “separation of concerns” which aims to create scalable, more easily maintainable coding architectures. For web developers, this principle guides us to keep our structure (HTML) separate from our presentation (CSS).


sample
<table>
  <tr>
    <th>Monday</th>
    <th>Tuesday</th>
    <th>Wednesday</th>
  </tr>
  <tr>
    <td colspan="2">Out of Town</td>
    <td>Back in Town</td>
  </tr>
</table>
----Monday Tuesday Wednesday
    Out of Town    Back in Town <!---In the example above, the data Out of Town spans the Monday and Tuesday table headings using the value 2 (two columns). The data Back in Town appear only under the Wednesday heading.--->

What should the example for colspan=“2” in this 215 exercise look like? What does a td element look like when it spans multiple columns?
Answer
Here is what the html will look like on the page (with a little extra css added to make the sections clearer).

Note that the “Out of Town” td element spans both the “Monday” and “Tuesday” columns, for a total colspan of 2.

Spanning Rows
Sample
<table>
  <tr> <!-- Row 1 -->
    <th></th>
    <th>Saturday</th>
    <th>Sunday</th>
  </tr>
  <tr> <!-- Row 2 -->
    <th>Morning</th>
    <td rowspan="2">Work</td>
    <td rowspan="3">Relax</td>
  </tr>
  <tr> <!-- Row 3 -->
    <th>Afternoon</th>
  </tr>
  <tr> <!-- Row 4 -->
    <th>Evening</th>
    <td>Dinner</td>
  </tr>
</table>

---- 
		Saturday   Sunday
Morning 
Afternoon 	Work	        Relax
Evening  	Dinner

<!----The rowspan attribute is used for data that spans multiple rows (perhaps an event goes on for multiple hours on a certain day). It accepts an integer (greater than or equal to 1) to denote the number of rows it spans across.---->
In index.html, span a <td> element across two rows.

Can the rowspan attribute only be used within <td> tags?
Answer
No. The rowspan attribute can also be used on <th> tags. For improved accessibility, when we create table headings that span multiple rows, we should also include the scope=”rowgroup” attribute within the opening <th> tag
 
Table Body
Long tables can be sectioned off using the table bodyelement: <tbody>.
The <tbody> element should contain all of the table's data, excluding the table headings (more on this in a later exercise).
Sample
<table>
  <tbody>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
    <tr>
      <th>Morning</th>
      <td rowspan="2">Work</td>
      <td rowspan="3">Relax</td>
    </tr>
    <tr>
     <th>Afternoon</th>
    </tr>
    <tr>
      <th>Evening</th>
      <td>Dinner</td>
    </tr>
  </tbody>
</table>
----		
Saturday   Sunday
Morning 
Afternoon 	Work	        Relax
Evening  	Dinner


1.
Enclose rows 2, 3, 4, 5, and 6 of the table in a <tbody> element.
Question
Why would we want to “section off” tables with the <tbody> tag?
Answer
The <tbody> tag together with the <thead> and <tfoot>tags (which you will learn about in the next two exercise) give our tables semantic meaning. These tags stand to improve the user experience in a number of ways:
enhanced screen reading experience for the visually impaired
<thead> and <tfoot> information can be shown on each page for printing
with a bit of CSS, <thead> and <tfoot> information can be seen while scrolling through long tables.
If th and thead are both headings in a table, what is the difference between them?
Answer
thead 111 is essentially a box to hold your headings for the table. It is used along with tbody and tfoot to make up the entirety of a table - header, body, footer.
On the otherhand, th 97 is a single heading element.

In this example given in the instructions for the table head 117 exercise, the whole top row is the thead for the table. The bolded bits of text are each th elements.

Sample
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title>Aguillar Family Wine Festival</title>
  <link rel="stylesheet" type="text/css" href="reset.css" />
  <link rel="stylesheet" type="text/css" href="style.css" />
  <link href="https://fonts.googleapis.com/css?family=Oswald" rel="stylesheet">
</head>

<body>
  <header>
    <h1>Annual Aguillar Family Wine Festival</h1>
  </header>
  
  <div class="container">
<table>
  <thead>
    <tr>
      <th colspan="2">
    <h1>Wine Festival Schedule</h1>
        </th>
      </tr>
    <tr>
      <th> <h2>Time</h2></th>
      <th><h2>Event</h2></th>
    <h2></h2>
    </tr>
    </thead>
  <tbody>
  <tr><td class="left">12:00PM</td>
    <td><h3>Welcome Reception</h3></td></tr>
  <tr><td class="left">01:00PM</td>
    <td><h3>Storytelling & Tasting</h3></td></tr>
  <tr><td class="left">02:00PM</td>
    <td><h3>Wine Luncheon</h3></td></tr>
  <tr><td class="left">03:00PM</td>
    <td><h3>Aguillar Family Wines</h3></td></tr>
  <tr><td class="left">04:00PM</td>
    <td><h3>Wine & Cheese Tasting</h3></td></tr>
    </tbody>
   </table>
  </div>
  
  <footer>
    <h3>Contact</h3>
    <h3>Location</h3>
    <h3>Privacy Policy</h3>
  </footer>
</body>

</html>

-----------COLSPAN = integer. ROWSPAN = integer. Table cells can span across more than one column or row. The attributes COLSPAN (“how many across”) and ROWSPAN (“how many down”) indicate how many columns or rows a cell should take up.

------
1.td, tr {
  border: 1px solid black;
}

th {
  border: 1px solid blue;
}
显示出来结果
1 pixel black border to rows and cells.
1 pixel blue border to headers.

---Which tag adds a new row header to an HTML table?
<th scope="row"></th>
------Which tag should surround an entire table of data?
<table></table>
-----Which tag adds new data to an HTML table?
<td></td>
----Which of the following tags is used to enclose the row of a table containing its headers?
<thead></thead>
----Which of the following tags is used to separate the footer of the table from its body?
<tfoot></tfoot>


FORM
Eg.
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>HTML Forms</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <!--Add your code below-->
      
      
    </section>
  </body>
</html>



---<form action="/example.html" method="POST">
</form>
In the above example, we've created the skeleton for a <form> that will send information to example.html as a POST request — the action attribute determines where the information is sent and the method attribute is assigned a HTTP verb that is included in the HTTP request. (Note: HTTP verbs like POST do not need to be capitalized for the request to work, but it's done so out of convention. In the example above we could have written method="post" and it would still work)

Text Input
<form action="/example.html" method="POST">
  <input type="text" name="first-text-field">
</form>
 For a user to properly identify an <input> we use the appropriately named <label>element.
Eg.

<form action="/example.html" method="POST">
  <label for="meal">What do you want to eat?</label>
  <br>
  <input type="text" name="food" id="meal">
</form>

Password Input
<form>
  <label for="user-password">Password: </label>
  <input type="password" id="user-password" name="user-password">
</form>



-----restaurant sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Password Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
				<h1>Login to start creating a burger!</h1>
        <label for="username">Username:</label>
  			<input type="text" name="username" id="username">
        <br>
        <label for="user-pw">Password:</label>
        <!--Add your code below-->
				<input id="user-pw" type="password" name="user-pw">
      </form>
    </section>
  </body>
</html>

------<form>
  <label for="years"> Years of experience: </label>
  <input id="years" name="years" type="number" step="1">
</form>


Sample

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Range Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
				<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty" value="beef">
        </section>
        <hr>

        <section class="patties">
          <label for="amount">How many patties would you like?</label>
	        <!--Add your code below-->
					<input id="amount" type="number" step="1" name="amount">
          
        </section>
      </form>
    </section>
  </body>
</html>



Range input
Eg.
<form>
  <label for="volume"> Volume Control</label>
  <input id="volume" name="volume" type="range" min="0" max="100" step="1">
</form>

Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Range Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
				<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
				
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
		       <!--Add your code below-->
          <input id="doneness" name="doneness" type="range" min="0" max="5" step="0.5">
          
          <span>Well-Done</span>
        </section>
        
      </form>
    </section>
  </body>
</html>


Checkbox Input
<form>
  <p>Choose your pizza toppings:</p>
  <label for="cheese">Extra cheese</label>
  <input id="cheese" name="topping" type="checkbox" value="cheese">
  <br>
  <label for="pepperoni">Pepperoni</label>
  <input id="pepperoni" name="topping" type="checkbox" value="pepperoni">
  <br>
  <label for="anchovy">Anchovy</label>
  <input id="anchovy" name="topping" type="checkbox" value="anchovy">
</form>

sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Checkbox Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
        <section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
          <input type="range" name="doneness" id="doneness" value="3" min="1" max="5">
          <span>Well-Done</span>
        </section>
        <hr>
        
        <section class="toppings">
          <span>What toppings would you like?</span>
          <br>
          <!--Add your code below for the first checkbox-->
<input id="lettuce" name="topping" type="checkbox" value="lettuce">
					<label for="lettuce">Lettuce</label>
  <input id="tomato" name="topping" type="checkbox" value="tomato">        
          <!--Add your code below for the second checkbox-->
          <label for="tomato">Tomato</label>
          <!--Add your code below for the third checkbox-->
<input type="checkbox" name="topping" id="others" value="others">
          <label for="others">others</label>

        </section>
        
      </form>
    </section>
  </body>
</html>



Radio Button Input
<form>
  <p>What is sum of 1 + 1?</p>
  <input type="radio" id="two" name="answer" value="2">
  <label for="two">2</label>
  <br>
  <input type="radio" id="eleven" name="answer" value="11">
  <label for="eleven">11</label>
</form>
Which renders:



Dropdown list
<form>
  <label for="lunch">What's for lunch?</label>
  <select id="lunch" name="lunch">
    <option value="pizza">Pizza</option>
    <option value="curry">Curry</option>
    <option value="salad">Salad</option>
    <option value="ramen">Ramen</option>
    <option value="tacos">Tacos</option>
  </select>
</form>


Datalist Input
<form>
  <label for="city">Ideal city to visit?</label>
  <input type="text" list="cities" id="city" name="city">

  <datalist id="cities">
    <option value="New York City"></option>
    <option value="Tokyo"></option>
    <option value="Barcelona"></option>
    <option value="Mexico City"></option>
    <option value="Melbourne"></option>
    <option value="Other"></option>  
  </datalist>
</form>


Textarea element
<form>
  <label for="blog">New Blog Post: </label>
  <br>
  <textarea id="blog" name="blog" rows="5" cols="30">
  </textarea>
</form>


Submit Form
<form>
  <input type="submit" value="Send">
</form>



Whole sample of forms
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Textarea element</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form action="submission.html" method="POST">
        <h1>Create a burger!</h1>
					<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
          <input type="range" name="doneness" id="doneness" value="3" min="1" max="5">
          <span>Well-Done</span>
        </section>
        <hr>
        <section class="toppings">
          <span>What toppings would you like?</span>
          <br>
          <input type="checkbox" name="topping" id="lettuce" value="lettuce">
          <label for="lettuce">Lettuce</label>
          <input type="checkbox" name="topping" id="tomato" value="tomato">
          <label for="tomato">Tomato</label>
          <input type="checkbox" name="topping" id="onion" value="onion">
          <label for="onion">Onion</label>
        </section>
        <hr>
        <section class="cheesy">
          <span>Would you like to add cheese?</span>
          <br>
          <input type="radio" name="cheese" id="yes" value="yes">
          <label for="yes">Yes</label>
          <input type="radio" name="cheese" id="no" value="yes">
          <label for="no">No</label>
        </section>
        <hr>
        <section class="bun-type">
          <label for="bun">What type of bun would you like?</label>
          <select name="bun" id="bun">
            <option value="sesame">Sesame</option>
            <option value="potatoe">Potato</option>
            <option value="pretzel">Pretzel</option>
          </select>
        </section>
        <hr>
        <section class="sauce-selection">
          <label for="sauce">What type of sauce would you like?</label>
          <input list="sauces" id="sauce" name="sauce">
          <datalist id="sauces">
            <option value="ketchup"></option>
            <option value="mayo"></option>
            <option value="mustard"></option>
          </datalist>
        </section>
        <hr>
        <section class="extra-info">
          <label for="extra">Anything else you want to add?</label>
          <br>
          <textarea id="extra" name="extra" rows="3" cols="40"></textarea>
        </section>
        <hr>

        <section class="submission">
          <!--Add your code below-->
          <input type="submit" value="Submit">
        </section>
        
      </form>
    </section>
  </body>
</html>




 

Introduction to HTML Form Validation
Validation is the concept of checking user provided data against the required data.
There are different types of validation. One type is server-side validation, this happens when data is sent to another machine (typically a server) for validation. An example of this type of validation is the usage of a login page. The form on the login page accepts username and password input, then sends the data to a server which checks that the pair matches up correctly.
On the other hand, we use client-side validation if we want to check the data on the browser (the client). This validation occurs before data is sent to the server. Different browsers implement client-side validation differently, but it leads to the same outcome.

Requiring an Input
<form action="/example.html" method="POST">
  <label for="allergies">Do you have any dietary restrictions?</label>
  <br>
  <input id="allergies" name="allergies" type="text" required>
  <br>
  <input type="submit" value="Submit">
</form>


Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Number Guessing</title>
    <link rel="stylesheet" href="style.css" type="text/css">
    <link href="https://fonts.googleapis.com/css?family=Spicy+Rice" rel="stylesheet">
  </head>
  <body>
    <section class="overlay">
      <h1>Guess the right number!</h1>
      <form action="check.html" method="GET">
        <!--Add a required attribute to the input element-->
        <label for="guess">Enter a number between 1-10:</label>
        <br>
        <input type="number" name="guess" id="guess" required>
        <br>
        <input type="submit" id="submission" value="Submit">
      </form>
    </section>
  </body>
</html>

Set a Minimum and Maximum
<form action="/example.html" method="POST">
  <label for="guests">Enter # of guests:</label>
  <input id="guests" name="guests" type="number" min="1" max="4">
  <input type="submit" value="Submit">
</form>


Checking Text Length
<form action="/example.html" method="POST">
  <label for="summary">Summarize your fillings in less than 250 characters</label>
  <input id="summary" name="summary" type="text" minlength="5" maxlength="250" required>
  <input type="submit" value="Submit">
</form>

<form action=”/example.html” method=”post”>
<label for=”summary”>summarize your filling in less than 250 characters</label>
<input id=”summary” name=”summary” type=”text” minlength=5” maxlength=”250” required>
<input type=”submit” value=”submit”>
</form>


Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Sign Up Page</title>
    <link rel="stylesheet" href="style.css" type="text/css">
    <link href="https://fonts.googleapis.com/css?family=Fjalla+One" rel="stylesheet">
  </head>
  <body>
    <section class="overlay">
      <h1>Sign Up</h1>
      <p>Create an account:</p>
      <form action="submission.html" method="GET">
        <!--Add the minlength and maxlength attributes to the input fields-->
        <label for="username">Username:</label>
        <br>
        <input id="username" name="username" type="text" required minlength="3" maxlength="15">
        <br>
        <label for="pw">Password:</label>
        <br>
        <input id="pw" name="pw" type="password" required minlength="8" maxlength="15">
        <br>
        <input type="submit" value="Submit">
      </form>
    </section>
  </body>
</html>


Matching a Pattern
<form action="/example.html" method="POST">
  <label for="payment">Credit Card Number (no spaces):</label>
  <br>
  <input id="payment" name="payment" type="text" required pattern="[0-9]{14,16}">
  <input type="submit" value="Submit">
</form>

Sample
	<input id="username" name="username" type="text" required minlength="3" maxlength="15" pattern="[a-zA-Z0-9]+">


Validation Review


------------Form a Story
Forms are great for collecting information on users, like job applications or insightful surveys. However, we can also stretch our creative muscles and have a little fun with forms. For this project, we'll use our knowledge of the HTML <form> and grab user input to put a spin on a classic story!
The logic for parsing and inserting of user inputs is already taken care of in main.js using JavaScript . 



updated more html notes 16/3/2019
HTML stands for HyperText Markup Language:
HTML is composed of elements. These elements structure the webpage and define its content.
1.Why would raw text need a structure?
---developers can create a hierarchy of information which serves several purposes
it allows users scanning a site to quickly pick out the most important ideas.
it helps visually impaired users navigate the content of a page using special software.
it helps search engines pick out important keywords that might otherwise get lost in a sea of text.
2.What type of content might an HTML element contain?
As you will learn, <p>, <div>, and <span> elements can contain text whereas elements like <ul> or <ol> should only contain <li> elements as direct children.
Block level tags like the <div> can contain all tags that can exist within the <body> (in other words, we can nest other elements within a <div>) whereas self-closing tags like <img> can not contain any content at all!

3.Do tags themselves count as content?

The content is just the information contained within the tags themselves.
 For example, the <img> tag is an example of a self-closing tag and it introduces content into the page differently than the <p> element.

4.Is there a sentence or a word element?
use an element like <span>, <em>, or <strong> to more specifically target content.

5.Why does the browser need information about the type of raw text it will display?
The browser needs this information so that it can give text meaning within the larger context of the document. In other words, the browser uses this information not only for rendering purposes but also so that it can create a structure which other programs (screen readers for example) can interpret.

6.Codecademy says that a markup language like HTML “defines structure and presentation of raw text”. Doesn’t CSS define the presentation of web content?
These days HTML is best categorized as a descriptive markup language which encourages developers to focus on the semantic meaning of information rather than its visual appearance. However, there are other markup languages which make no such separation of concerns. In fact, HTML used to be more presentational before the advent of CSS.

7.In this exercise 613, why does the paragraph display on the page but the title “My Coding Journey” does not?
Answer
The site <title> does not display on the page because this information is contained within the document’s <head>. Unlike the body element, the <head> element contains metadata which will not be displayed by the browser. You will learn more about the head and title elements in lesson 2 so stay tuned!

8.What is a web browser?
Answer
A browser is a piece of software which allows us to display content on the web (among other things). The most popular web browsers today include Chrome, Firefox, Safari, and Edge. In this lesson, the HTML that you write will be displayed in the emulated browser in the right of your workspace.

9.Question
In steps 1 and 2 of this exercise, both <p> elements display in the same exact way. As it doesn’t seem like anything special happened here, what is the point of nesting the <p> element in a <div> element?
Answer
In this case, this is done purely for demonstrative purpose. In the future you will find that <div> elements are often used to group related content. This can serve to give a page some added structure and to allow for more modular styling.


10.Question
This exercise 143 says that child elements can inherit from their parents. What sorts of things can child elements inherit from their parents?
Answer
When you dive into our CSS course you will learn that child elements inherit most of their styling from their parent elements. In other words, most styles cascade down from parents to children.

11.How does the browser know what language other documents are written in? For example, why doesn’t css need a doctype?
Answer
DOCTYPE declarations are only required for html based documents. Other JavaScript or CSS files are actually loaded into the page with <link> or tags. These tags signify the file type to the browser thereby allowing the browser to properly parse the file.

12.Without the html tags mentioned in this lesson, in what ways might the browser misinterpret our HTML code?
Answer
The <html> tag is actually an example of an optional tag which means that there are situations in which it can be omitted. Even though omitted optional tags will be inserted into the document by the browser and may not always be required, most developers would say that it is best practice to include these tags. Including optional tags enhances readability, improves cross-browser support, and takes some burden off of the browser.
In short, while the <html> tag can be omitted I do not believe it should be omitted.

13.Why does the browser need metadata about the page?
Answer
There exists different categorizations of metadata but most generally metadata is “data about data”. While the browser doesn’t need most metadata it does often use metadata to enhance the user experience in some way. Metadata not displayed on a page but behind the scenes it can be used by other software (web crawlers, search engines, browsers, etc.) to process, encode, extract or index all sorts of interesting information (geographic coordinates, calendar events, contact info, etc.). What’s more, businesses are often interested in using metadata to improve SEO or Search Engine Optimization.


TABLE
--There are many websites on the Internet that display information like stock prices, sports scores, invoice data, and more.
--The HTML <tr> element defines a row of cells in a table. The row's cells can then be established using a mix of <td> (data cell) and <th> (header cell) elements.

Sample
<!DOCTYPE html>
<html>
<head>
  <title>Ship To It - Company Packing List</title>
  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
<body>

  <ul class="navigation">
    <li><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-9/htmlcss1-img_logo-shiptoit.png" height="20px;"></li>
    <li class="active">Action List</li>
    <li>Profiles</li>
    <li>Settings</li>
  </ul>

  <div class="search">Search the table</div>

  <table>
    <thead>
      <tr>
        <th>Company Name</th>
        <th>Number of Items to Ship</th>
        <th>Next Action</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th>Adam's Greenworks</th>
        <td>14</td>
        <td>Package Items</td>
      </tr>
      <tr>
        <th>Davie's Burgers</th>
        <td>2</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Baker's Bike Shop</th>
        <td>3</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Miss Sally's Southern</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Summit Resort Rentals</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Strike Fitness</th>
        <td>1</td>
        <td>Enter Order</td>
      </tr>
      </tbody>
  </table>

</body>
</html>
 Run as below
Search the table
COMPANY NAME
NUMBER OF ITEMS TO SHIP
NEXT ACTION
Adam's Greenworks
14
Package Items
Davie's Burgers
2
Send Invoice
Baker's Bike Shop
3
Send Invoice
Miss Sally's Southern
4
Ship
Summit Resort Rentals
4
Ship
Strike Fitness
1
Enter Order


Sample 2
To add titles to rows and columns, you can use the table heading element: <th>.
<table>
  <tr>
    <th></th>
    <th scope="col">Saturday</th>
    <th scope="col">Sunday</th>
  </tr>
  <tr>
    <th scope="row">Temperature</th>
    <td>73</td>
    <td>81</td>
  </tr>
</table>


---row - this value makes it clear that the heading is for a row.
col - this value makes it clear that the heading is for a column.
--Question
This exercise discusses the scope attribute. What is the purpose of the scope attribute and are row and col the only values this attribute can have?
Answer
The scope attribute is used by screen readers to enhance accessibility for visually impaired users. In addition to the row and col values shown in this exercise, the scope attribute can also have the following values:
rowgroup: used for table headings that group multiple rows.
colgroup:used for table headings that group multiple columns.
auto: the default value
In lessons 8 and 9 you will learn how to create cells that span multiple rows or columns. For improved accessibility, we should use the appropriate rowgroup and colgroup values within these headings.

Sample
1.<tr>
  <td>Davie's Burgers</td>
  <td>2</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Baker's Bike Shop</td>
  <td>3</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Miss Sally's Southern</td>
  <td>4</td>
  <td>Ship</td>
</tr>
<tr>
  <td>Summit Resort Rentals</td>
  <td>4</td>
  <td>Ship</td>
</tr>
<tr>
  <td>Strike Fitness</td>
  <td>1</td>
  <td>Enter Order</td>
</tr>
---
Davie's Burgers
2
Send Invoice
Baker's Bike Shop
3
Send Invoice
Miss Sally's Southern
4
Ship
Summit Resort Rentals
4
Ship
Strike Fitness
1
Enter Order



Question
Why should we use CSS rather than HTML to create borders for our tables?
Answer
Within software engineering, there is a design principle known as “separation of concerns” which aims to create scalable, more easily maintainable coding architectures. For web developers, this principle guides us to keep our structure (HTML) separate from our presentation (CSS).


sample
<table>
  <tr>
    <th>Monday</th>
    <th>Tuesday</th>
    <th>Wednesday</th>
  </tr>
  <tr>
    <td colspan="2">Out of Town</td>
    <td>Back in Town</td>
  </tr>
</table>
----Monday Tuesday Wednesday
    Out of Town    Back in Town <!---In the example above, the data Out of Town spans the Monday and Tuesday table headings using the value 2 (two columns). The data Back in Town appear only under the Wednesday heading.--->

What should the example for colspan=“2” in this 215 exercise look like? What does a td element look like when it spans multiple columns?
Answer
Here is what the html will look like on the page (with a little extra css added to make the sections clearer).

Note that the “Out of Town” td element spans both the “Monday” and “Tuesday” columns, for a total colspan of 2.

Spanning Rows
Sample
<table>
  <tr> <!-- Row 1 -->
    <th></th>
    <th>Saturday</th>
    <th>Sunday</th>
  </tr>
  <tr> <!-- Row 2 -->
    <th>Morning</th>
    <td rowspan="2">Work</td>
    <td rowspan="3">Relax</td>
  </tr>
  <tr> <!-- Row 3 -->
    <th>Afternoon</th>
  </tr>
  <tr> <!-- Row 4 -->
    <th>Evening</th>
    <td>Dinner</td>
  </tr>
</table>

---- 
		Saturday   Sunday
Morning 
Afternoon 	Work	        Relax
Evening  	Dinner

<!----The rowspan attribute is used for data that spans multiple rows (perhaps an event goes on for multiple hours on a certain day). It accepts an integer (greater than or equal to 1) to denote the number of rows it spans across.---->
In index.html, span a <td> element across two rows.

Can the rowspan attribute only be used within <td> tags?
Answer
No. The rowspan attribute can also be used on <th> tags. For improved accessibility, when we create table headings that span multiple rows, we should also include the scope=”rowgroup” attribute within the opening <th> tag
 
Table Body
Long tables can be sectioned off using the table bodyelement: <tbody>.
The <tbody> element should contain all of the table's data, excluding the table headings (more on this in a later exercise).
Sample
<table>
  <tbody>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
    <tr>
      <th>Morning</th>
      <td rowspan="2">Work</td>
      <td rowspan="3">Relax</td>
    </tr>
    <tr>
     <th>Afternoon</th>
    </tr>
    <tr>
      <th>Evening</th>
      <td>Dinner</td>
    </tr>
  </tbody>
</table>
----		
Saturday   Sunday
Morning 
Afternoon 	Work	        Relax
Evening  	Dinner


1.
Enclose rows 2, 3, 4, 5, and 6 of the table in a <tbody> element.
Question
Why would we want to “section off” tables with the <tbody> tag?
Answer
The <tbody> tag together with the <thead> and <tfoot>tags (which you will learn about in the next two exercise) give our tables semantic meaning. These tags stand to improve the user experience in a number of ways:
enhanced screen reading experience for the visually impaired
<thead> and <tfoot> information can be shown on each page for printing
with a bit of CSS, <thead> and <tfoot> information can be seen while scrolling through long tables.
If th and thead are both headings in a table, what is the difference between them?
Answer
thead 111 is essentially a box to hold your headings for the table. It is used along with tbody and tfoot to make up the entirety of a table - header, body, footer.
On the otherhand, th 97 is a single heading element.

In this example given in the instructions for the table head 117 exercise, the whole top row is the thead for the table. The bolded bits of text are each th elements.

Sample
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title>Aguillar Family Wine Festival</title>
  <link rel="stylesheet" type="text/css" href="reset.css" />
  <link rel="stylesheet" type="text/css" href="style.css" />
  <link href="https://fonts.googleapis.com/css?family=Oswald" rel="stylesheet">
</head>

<body>
  <header>
    <h1>Annual Aguillar Family Wine Festival</h1>
  </header>
  
  <div class="container">
<table>
  <thead>
    <tr>
      <th colspan="2">
    <h1>Wine Festival Schedule</h1>
        </th>
      </tr>
    <tr>
      <th> <h2>Time</h2></th>
      <th><h2>Event</h2></th>
    <h2></h2>
    </tr>
    </thead>
  <tbody>
  <tr><td class="left">12:00PM</td>
    <td><h3>Welcome Reception</h3></td></tr>
  <tr><td class="left">01:00PM</td>
    <td><h3>Storytelling & Tasting</h3></td></tr>
  <tr><td class="left">02:00PM</td>
    <td><h3>Wine Luncheon</h3></td></tr>
  <tr><td class="left">03:00PM</td>
    <td><h3>Aguillar Family Wines</h3></td></tr>
  <tr><td class="left">04:00PM</td>
    <td><h3>Wine & Cheese Tasting</h3></td></tr>
    </tbody>
   </table>
  </div>
  
  <footer>
    <h3>Contact</h3>
    <h3>Location</h3>
    <h3>Privacy Policy</h3>
  </footer>
</body>

</html>

-----------COLSPAN = integer. ROWSPAN = integer. Table cells can span across more than one column or row. The attributes COLSPAN (“how many across”) and ROWSPAN (“how many down”) indicate how many columns or rows a cell should take up.

------
1.td, tr {
  border: 1px solid black;
}

th {
  border: 1px solid blue;
}
显示出来结果
1 pixel black border to rows and cells.
1 pixel blue border to headers.

---Which tag adds a new row header to an HTML table?
<th scope="row"></th>
------Which tag should surround an entire table of data?
<table></table>
-----Which tag adds new data to an HTML table?
<td></td>
----Which of the following tags is used to enclose the row of a table containing its headers?
<thead></thead>
----Which of the following tags is used to separate the footer of the table from its body?
<tfoot></tfoot>


FORM
Eg.
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>HTML Forms</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <!--Add your code below-->
      
      
    </section>
  </body>
</html>



---<form action="/example.html" method="POST">
</form>
In the above example, we've created the skeleton for a <form> that will send information to example.html as a POST request — the action attribute determines where the information is sent and the method attribute is assigned a HTTP verb that is included in the HTTP request. (Note: HTTP verbs like POST do not need to be capitalized for the request to work, but it's done so out of convention. In the example above we could have written method="post" and it would still work)

Text Input
<form action="/example.html" method="POST">
  <input type="text" name="first-text-field">
</form>
 For a user to properly identify an <input> we use the appropriately named <label>element.
Eg.

<form action="/example.html" method="POST">
  <label for="meal">What do you want to eat?</label>
  <br>
  <input type="text" name="food" id="meal">
</form>

Password Input
<form>
  <label for="user-password">Password: </label>
  <input type="password" id="user-password" name="user-password">
</form>



-----restaurant sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Password Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
				<h1>Login to start creating a burger!</h1>
        <label for="username">Username:</label>
  			<input type="text" name="username" id="username">
        <br>
        <label for="user-pw">Password:</label>
        <!--Add your code below-->
				<input id="user-pw" type="password" name="user-pw">
      </form>
    </section>
  </body>
</html>

------<form>
  <label for="years"> Years of experience: </label>
  <input id="years" name="years" type="number" step="1">
</form>


Sample

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Range Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
				<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty" value="beef">
        </section>
        <hr>

        <section class="patties">
          <label for="amount">How many patties would you like?</label>
	        <!--Add your code below-->
					<input id="amount" type="number" step="1" name="amount">
          
        </section>
      </form>
    </section>
  </body>
</html>



Range input
Eg.
<form>
  <label for="volume"> Volume Control</label>
  <input id="volume" name="volume" type="range" min="0" max="100" step="1">
</form>



Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Range Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
				<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
				
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
		       <!--Add your code below-->
          <input id="doneness" name="doneness" type="range" min="0" max="5" step="0.5">
          
          <span>Well-Done</span>
        </section>
        
      </form>
    </section>
  </body>
</html>


Checkbox Input
<form>
  <p>Choose your pizza toppings:</p>
  <label for="cheese">Extra cheese</label>
  <input id="cheese" name="topping" type="checkbox" value="cheese">
  <br>
  <label for="pepperoni">Pepperoni</label>
  <input id="pepperoni" name="topping" type="checkbox" value="pepperoni">
  <br>
  <label for="anchovy">Anchovy</label>
  <input id="anchovy" name="topping" type="checkbox" value="anchovy">
</form>



sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Checkbox Input</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form>
        <h1>Create a burger!</h1>
        <section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
          <input type="range" name="doneness" id="doneness" value="3" min="1" max="5">
          <span>Well-Done</span>
        </section>
        <hr>
        
        <section class="toppings">
          <span>What toppings would you like?</span>
          <br>
          <!--Add your code below for the first checkbox-->
<input id="lettuce" name="topping" type="checkbox" value="lettuce">
					<label for="lettuce">Lettuce</label>
  <input id="tomato" name="topping" type="checkbox" value="tomato">        
          <!--Add your code below for the second checkbox-->
          <label for="tomato">Tomato</label>
          <!--Add your code below for the third checkbox-->
<input type="checkbox" name="topping" id="others" value="others">
          <label for="others">others</label>

        </section>
        
      </form>
    </section>
  </body>
</html>



Radio Button Input

<form>
  <p>What is sum of 1 + 1?</p>
  <input type="radio" id="two" name="answer" value="2">
  <label for="two">2</label>
  <br>
  <input type="radio" id="eleven" name="answer" value="11">
  <label for="eleven">11</label>
</form>


Which renders:



Dropdown list
<form>
  <label for="lunch">What's for lunch?</label>
  <select id="lunch" name="lunch">
    <option value="pizza">Pizza</option>
    <option value="curry">Curry</option>
    <option value="salad">Salad</option>
    <option value="ramen">Ramen</option>
    <option value="tacos">Tacos</option>
  </select>
</form>


Datalist Input
<form>
  <label for="city">Ideal city to visit?</label>
  <input type="text" list="cities" id="city" name="city">

  <datalist id="cities">
    <option value="New York City"></option>
    <option value="Tokyo"></option>
    <option value="Barcelona"></option>
    <option value="Mexico City"></option>
    <option value="Melbourne"></option>
    <option value="Other"></option>  
  </datalist>
</form>


Textarea element
<form>
  <label for="blog">New Blog Post: </label>
  <br>
  <textarea id="blog" name="blog" rows="5" cols="30">
  </textarea>
</form>


Submit Form
<form>
  <input type="submit" value="Send">
</form>



Whole sample of forms
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Rubik" rel="stylesheet">
    <title>Textarea element</title>
  </head>
  <body>
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form action="submission.html" method="POST">
        <h1>Create a burger!</h1>
					<section class="protein">
          <label for="patty">What type of protein would you like?</label>
    			<input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="patties">
          <label for="amount">How many patties would you like?</label>
          <input type="number" name="amount" id="amount">
        </section>
        <hr>
        <section class="cooked">
          <label for="doneness">How do you want your patty cooked</label>
          <br>
          <span>Rare</span>
          <input type="range" name="doneness" id="doneness" value="3" min="1" max="5">
          <span>Well-Done</span>
        </section>
        <hr>
        <section class="toppings">
          <span>What toppings would you like?</span>
          <br>
          <input type="checkbox" name="topping" id="lettuce" value="lettuce">
          <label for="lettuce">Lettuce</label>
          <input type="checkbox" name="topping" id="tomato" value="tomato">
          <label for="tomato">Tomato</label>
          <input type="checkbox" name="topping" id="onion" value="onion">
          <label for="onion">Onion</label>
        </section>
        <hr>
        <section class="cheesy">
          <span>Would you like to add cheese?</span>
          <br>
          <input type="radio" name="cheese" id="yes" value="yes">
          <label for="yes">Yes</label>
          <input type="radio" name="cheese" id="no" value="yes">
          <label for="no">No</label>
        </section>
        <hr>
        <section class="bun-type">
          <label for="bun">What type of bun would you like?</label>
          <select name="bun" id="bun">
            <option value="sesame">Sesame</option>
            <option value="potatoe">Potato</option>
            <option value="pretzel">Pretzel</option>
          </select>
        </section>
        <hr>
        <section class="sauce-selection">
          <label for="sauce">What type of sauce would you like?</label>
          <input list="sauces" id="sauce" name="sauce">
          <datalist id="sauces">
            <option value="ketchup"></option>
            <option value="mayo"></option>
            <option value="mustard"></option>
          </datalist>
        </section>
        <hr>
        <section class="extra-info">
          <label for="extra">Anything else you want to add?</label>
          <br>
          <textarea id="extra" name="extra" rows="3" cols="40"></textarea>
        </section>
        <hr>

        <section class="submission">
          <!--Add your code below-->
          <input type="submit" value="Submit">
        </section>
        
      </form>
    </section>
  </body>
</html>




 

Introduction to HTML Form Validation
Validation is the concept of checking user provided data against the required data.
There are different types of validation. One type is server-side validation, this happens when data is sent to another machine (typically a server) for validation. An example of this type of validation is the usage of a login page. The form on the login page accepts username and password input, then sends the data to a server which checks that the pair matches up correctly.
On the other hand, we use client-side validation if we want to check the data on the browser (the client). This validation occurs before data is sent to the server. Different browsers implement client-side validation differently, but it leads to the same outcome.

Requiring an Input
<form action="/example.html" method="POST">
  <label for="allergies">Do you have any dietary restrictions?</label>
  <br>
  <input id="allergies" name="allergies" type="text" required>
  <br>
  <input type="submit" value="Submit">
</form>


Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Number Guessing</title>
    <link rel="stylesheet" href="style.css" type="text/css">
    <link href="https://fonts.googleapis.com/css?family=Spicy+Rice" rel="stylesheet">
  </head>
  <body>
    <section class="overlay">
      <h1>Guess the right number!</h1>
      <form action="check.html" method="GET">
        <!--Add a required attribute to the input element-->
        <label for="guess">Enter a number between 1-10:</label>
        <br>
        <input type="number" name="guess" id="guess" required>
        <br>
        <input type="submit" id="submission" value="Submit">
      </form>
    </section>
  </body>
</html>

Set a Minimum and Maximum
<form action="/example.html" method="POST">
  <label for="guests">Enter # of guests:</label>
  <input id="guests" name="guests" type="number" min="1" max="4">
  <input type="submit" value="Submit">
</form>


Checking Text Length
<form action="/example.html" method="POST">
  <label for="summary">Summarize your fillings in less than 250 characters</label>
  <input id="summary" name="summary" type="text" minlength="5" maxlength="250" required>
  <input type="submit" value="Submit">
</form>

<form action=”/example.html” method=”post”>
<label for=”summary”>summarize your filling in less than 250 characters</label>
<input id=”summary” name=”summary” type=”text” minlength=5” maxlength=”250” required>
<input type=”submit” value=”submit”>
</form>


Sample
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Sign Up Page</title>
    <link rel="stylesheet" href="style.css" type="text/css">
    <link href="https://fonts.googleapis.com/css?family=Fjalla+One" rel="stylesheet">
  </head>
  <body>
    <section class="overlay">
      <h1>Sign Up</h1>
      <p>Create an account:</p>
      <form action="submission.html" method="GET">
        <!--Add the minlength and maxlength attributes to the input fields-->
        <label for="username">Username:</label>
        <br>
        <input id="username" name="username" type="text" required minlength="3" maxlength="15">
        <br>
        <label for="pw">Password:</label>
        <br>
        <input id="pw" name="pw" type="password" required minlength="8" maxlength="15">
        <br>
        <input type="submit" value="Submit">
      </form>
    </section>
  </body>
</html>


Matching a Pattern
<form action="/example.html" method="POST">
  <label for="payment">Credit Card Number (no spaces):</label>
  <br>
  <input id="payment" name="payment" type="text" required pattern="[0-9]{14,16}">
  <input type="submit" value="Submit">
</form>

Sample
	<input id="username" name="username" type="text" required minlength="3" maxlength="15" pattern="[a-zA-Z0-9]+">


Validation Review


------------Form a Story
Forms are great for collecting information on users, like job applications or insightful surveys. However, we can also stretch our creative muscles and have a little fun with forms. For this project, we'll use our knowledge of the HTML <form> and grab user input to put a spin on a classic story!
The logic for parsing and inserting of user inputs is already taken care of in main.js using JavaScript . 

Example
<!DOCTYPE html>
<html lang="en" dir="ltr">
 <head>
   <meta charset="utf-8">
   <link rel="stylesheet" href="style.css">
   <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
   <title>Form a Story</title>
 </head>
 <body>
   <section id="top">
     <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-html-forms/formAStoryLogo.svg" alt="Form A Story Logo">
   </section>

   <section id="main">
     <h1>Complete the Form -<br> Complete the Story!</h1>
     <hr>
     <!--Add your form below:-->
     <form action="story.html" method="GET">
     <label for="animal-1">Animal</label>
       <input id="animal-1" name="animal-1" type="text" required>
       <br/>
         <label for="animal-2">animal-2</label>
       <input id="animal-2" name="animal-2" type="text" required>
       <br/>
       <label for="animal-3">animal-3</label>
       <input id="animal-3" name="animal-3" type="text" required>
       <br/>
       <label for="adj-1">Adjective(past tense)</label>
       <input id="adj-1" name="adj-1" type="text" required>
       <br/>
       <label for="verb-1">Verb(ends-in-ing)</label>
       <input id="verb-1" name="verb-1" type="text" required>
       <br/>
<label for=”num-1”>Number:</label>
       <input id="num-1" name="num-1" type="number" required >
       <br/>
 <span>Yes or No:</span>     
   <input id="yes" type="radio" name="answer" value="yes" required>
       <label for="yes">Yes</label>
   <input id="no" type="radio" name="answer" value="no" required>
   <label for="no">No<label>
     <br/>
   <label>Relative speed(end in -er)</label>
     <select id="speed" name="speed" required>
     <option value="faster">Faster</option>
     <option value="quciker">Quicker</option>
   <option value="speedir">Speedir</option>  
  </select>
     <br/>
     <label for="quote">Motivational Quote</label>
     <input id="quote" name="quote" type="text" list="quote-choices" required>
     <datalist id="quote-choices">
     <option value="codecodemy">Codecodemy</option>>
     <option value="code">Code</option>
     <option value="example">Example</option>
</datalist>
     <br/>
     <label for="message">Meaningful Message</label>
     <textarea id="message" name="message" row="8" cols="40"required></textarea>>
       <br/>
<input type="submit" value="Form My Story!">

   </section>
 </body>
</html>



Example from GA
<h1>Welcome to my page</h1>
<p>This is a page about puppies</p>
<p>My favourite puppy are:</p>
<ul>
  <li>poodle</li>
  <li>german shephard</li>
</ul>
<img src="https://images.pexels.com/photos/1108099/pexels-photo-1108099.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="this is an image of a puppy">

<a href="https://www.google.com">Click here to go to Google</a>


--Image Alts
The alt attribute, which means alternative text, brings meaning to the images on our sites. The altattribute can be added to the image tag just like the src attribute. The value of alt should be a description of the image.
<img src="#" alt="A field of yellow sunflowers" />

-Videos
<video src="myVideo.mp4" width="320" height="240" controls>
  Video not supported
</video>
After the src attribute, the width and heightattributes are used to set the size of the video displayed in the browser. The controls attribute instructs the browser to include basic video controls: pause, play and skip.
The text, “Video not supported”, between the opening and closing video tags will only be displayed if the browser is unable to load the video.



-Linking to Other Web Pages
The anchor element in the example above is incomplete without the href attribute. This attribute stands for hyperlink reference and is used to link to a path, or the address to where a file is located (whether it is on your computer or another location). The paths provided to the href attribute are often URLs.
<a href="https://www.wikipedia.org/">This Is A Link To Wikipedia</a>

-Opening Links in a New Window
For a link to open in a new window, the targetattribute requires a value of _blank. The targetattribute can be added directly to the opening tag of the anchor element, just like the href attribute.
<a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">The Brown Bear</a>

-Linking to Relative Page
Many sites also link to internal web pages like Home, About, and Contact.
Before we learn how to link between internal pages, let’s establish where our files are stored. When making multi-page static websites, web developers often store HTML files in the root directory, or a main folder where all the files for the project are stored. As the size of the projects you create grows, you may use additional folders within the main project folder to organize your code.
project-folder/
|—— about.html
|—— contact.html
|—— index.html
The example above shows three different files — about.html, contact.html, and index.html in one folder.
HTML files are often stored in the same folder, as shown in the example above. If the browser is currently displaying index.html, it also knows that about.html and contact.html are in the same folder. Because the files are stored in the same folder, we can link web pages together using a relative path.
<a href="./contact.html">Contact</a>

-Linking At Will
You’ve probably visited websites where not all links were made up of text. Maybe the links you clicked on were images or some other form of content.
<a href="https://en.wikipedia.org/wiki/Opuntia" target="_blank"><img src="#" alt="A red prickly pear fruit"/></a>

Eg
<!DOCTYPE html>
<html>

<head>
  <title>Brown Bears</title>
</head>

<body>
  <a href="./index.html">Brown Bear</a>
  <a href="./aboutme.html">About Me</a>
  <h1>The Brown Bear</h1>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the
      Atlas bear and the Himalayan brown bear.</p>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">Learn More</a>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <ol>
      <li>Russia</li>
      <li>United States</li>
      <li>Canada</li>
    </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank"><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/web101-image_brownbear.jpg"/></a>
    <video src="https://s3.amazonaws.com/codecademy-content/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" height="240" width="320" controls>Video not supported</video>
  </div>
</body>

</html>

-Linking to Same Page
When users visit our site, we want them to be able to click a link and have the page automatically scroll to a specific section.
<p id="top">This is the top of the page!</p>
<h1 id="bottom">This is the bottom! </h1>
An id should be descriptive to make it easier to remember the purpose of a link. The target link is a string containing the # character and the target element’s id.
<ol>
  <li><a href="#top">Top</a></li>
  <li><a href="#bottom">Bottom</a></li>
</ol>
Eg
<ul>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#habitat">Habitat</a></li>
    <li><a href="#media">Media</a></li>
  </ul>

-Whitespace
Programmers use two tools to visualize the relationship between elements: whitespace and indentation.

-Indentation
he second tool web developers use to make the structure of code easier to read is indentation. The spaces are inserted using the space and tab bars on your keyboard.
 
 
eg

<body>
	<h1>Whitespace</h1>    
	<div>
		<p>Whitespace and indentation make html documents easier to read.</p>
	</div>  
</body>

-Comments
Comments begin with <!-- and end with -->. Any characters in between will be ignored by your browser
-HTML Tags
 found in Mozilla documentation.
<!DOCTYPE html>
<html>

<head>
  <title>Brown Bears</title>
</head>

<body>
  <nav>
    <a href="./index.html">Brown Bear</a>
    <a href="./aboutme.html">About Me</a>
  </nav>
  <h1>The Brown Bear</h1>
  <nav>
    <ul>
      <li><a href="#introduction">Introduction</a></li>
      <li><a href="#habitat">Habitat</a></li>
      <li><a href="#media">Media</a></li>
    </ul>
  </nav>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the
      Atlas bear and the Himalayan brown bear.</p>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">Learn More</a>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <ol>
      <li>Russia</li>
      <li>United States</li>
      <li>Canada</li>
    </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
    <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/web101-image_brownbear.jpg" />
    <video src="https://s3.amazonaws.com/codecademy-content/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" height="240" width="320" controls>Video not supported</video>
  </div>
</body>

</html>

-new chapter Table
<!DOCTYPE html>
<html>
<head>
  <title>Ship To It - Company Packing List</title>
  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
<body>

  <ul class="navigation">
    <li><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-9/htmlcss1-img_logo-shiptoit.png" height="20px;"></li>
    <li class="active">Action List</li>
    <li>Profiles</li>
    <li>Settings</li>
  </ul>

  <div class="search">Search the table</div>

  <table>
    <thead>
      <tr>
        <th>Company Name</th>
        <th>Number of Items to Ship</th>
        <th>Next Action</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th>Adam's Greenworks</th>
        <td>14</td>
        <td>Package Items</td>
      </tr>
      <tr>
        <th>Davie's Burgers</th>
        <td>2</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Baker's Bike Shop</th>
        <td>3</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <th>Miss Sally's Southern</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Summit Resort Rentals</th>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <th>Strike Fitness</th>
        <td>1</td>
        <td>Enter Order</td>
      </tr>
      </tbody>
  </table>

</body>
</html>


Eg
<table>
  <tbody>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
    <tr>
      <th>Morning</th>
      <td rowspan="2">Work</td>
      <td rowspan="3">Relax</td>
    </tr>
    <tr>
     <th>Afternoon</th>
    </tr>
    <tr>
      <th>Evening</th>
      <td>Dinner</td>
    </tr>
  </tbody>
</table>
//		Saturday Sunday
Morning        Work	Relax
Afternoon
Evening    Dinner
Work cover morning and afternoon,relax cover m,a ,e

These attributes have numeric values, for example, colspan=3 will span three columns.

-Table Headings
eg
<table>
  <tr>
    <th></th>
    <th scope="col">Saturday</th>
    <th scope="col">Sunday</th>
  </tr>
  <tr>
    <th scope="row">Temperature</th>
    <td>73</td>
    <td>81</td>
  </tr>
</table>

-Table Borders
<table border="1">
  <tr>
    <td>73</td>
    <td>81</td>
  </tr>
</table>
And as below similar for border
table, td {
  border: 1px solid black;
}

-Spanning Columns
Data can span columns using the colspan attribute. The attributes accepts an integer (greater than or equal to 1) to denote the number of columns it spans across.
In the example above, the data Out of Town spans the Monday and Tuesday table headings using the value 2 (two columns). The data Back in Town appear only under the Wednesday heading.
<table>
  <tr>
    <th>Monday</th>
    <th>Tuesday</th>
    <th>Wednesday</th>
  </tr>
  <tr>
    <td colspan="2">Out of Town</td>
    <td>Back in Town</td>
  </tr>
</table>
-Spanning Rows
-Table Body
-Table Head
<thead>tag is table’s headings using the <thead> element.
<thead> table’s heading and <th> is inside the body Example
<html>
<head></head>
<title></title>
<body>
<table>
<thead>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
  </thead>
<tbody>
……..
</tbody>
</table>
</body>
</html>

-Table Footer
<table>
  <thead>
    <tr>
      <th>Quarter</th>
      <th>Revenue</th>
      <th>Costs</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Q1</th>
      <td>$10M</td>
      <td>$7.5M</td>
    </tr>
    <tr>
      <th>Q2</th>
      <td>$12M</td>
      <td>$5M</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>Total</th>
      <td>$22M</td>
      <td>$12.5M</td>
    </tr>
  </tfoot>
</table>

-Styling with CSS
table, th, td {
  border: 1px solid black;
  font-family: Arial, sans-serif;
  text-align: center;
}

-Let’s review what you’ve learned so far:
The <table> element creates a table.
The <tr> element adds rows to a table.
To add data to a row, you can use the <td>element.
Table headings clarify the meaning of data. Headings are added with the <th> element.
Table data can span columns using the colspanattribute.
Table data can span rows using the rowspanattribute.
Tables can be split into three main sections: a head, a body, and a footer.
A table’s head is created with the <thead>element.
A table’s body is created with the <tbody>element.
A table’s footer is created with the <tfoot>element.
All the CSS properties you learned about in this course can be applied to tables and their data.
Good example to explain
 -html
<!DOCTYPE html>
<html>
<head>
  <title>Ship To It - Company Packing List</title>
  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
<body>

  <ul class="navigation">
    <li><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-9/htmlcss1-img_logo-shiptoit.png" height="20px;"></li>
    <li class="active">Action List</li>
    <li>Profiles</li>
    <li>Settings</li>
  </ul>

  <div class="search">Search the table</div>
  
  <table>
    <thead>
      <tr>
        <th>Company Name</th>
        <th>Number of Items to Ship</th>
        <th>Next Action</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Adam's Greenworks</td>
        <td>14</td>
        <td>Package Items</td>
      </tr>
      <tr>
        <td>Davie's Burgers</td>
        <td>2</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <td>Baker's Bike Shop</td>
        <td>3</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <td>Miss Sally's Southern</td>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <td>Summit Resort Rentals</td>
        <td>4</td>
        <td>Ship</td>
      </tr>
      <tr>
        <td>Strike Fitness</td>
        <td>1</td>
        <td>Enter Order</td>
      </tr>
    </tbody>
    <tfoot>
      <td>Total</td>
			<td>28</td>
    </tfoot>
  </table>


</body>
</html>


---CSS
body {
  background: #EEE;
  margin: 0;
  padding: 0;
}

/* Navigation */

.navigation {
  box-sizing: border-box;
  background-color: #3587A4;
  overflow: auto;
  padding: 18px 50px;
  position: relative;
  top: 0;
  width: 100%;
  z-index: 999;
}

ul {
  padding: 0;
  margin: 0;
}

li {
  color: #FFF;
  display: inline-block;
  font-family: 'Oxygen', sans-serif;
  font-size: 16px;
  font-weight: 300;
  letter-spacing: 2px;
  margin: 0;
  padding: 20px 18px 10px 18px;
  text-transform: uppercase;
}

.active {
  color: #88CCF1;
}

/* Table */

table {
  height: 40%;
  left: 10%;
  margin: 20px auto;
  overflow-y: scroll;
  position: static;
  width: 80%;
}

thead th {
  background: #88CCF1;
  color: #FFF;
  font-family: 'Lato', sans-serif;
  font-size: 16px;
  font-weight: 100;
  letter-spacing: 2px;
  text-transform: uppercase;
}

tr {
  background: #f4f7f8;
  border-bottom: 1px solid #FFF;
  margin-bottom: 5px;
}

th, td {
  font-family: 'Lato', sans-serif;
  font-size: 18px;
  font-weight: 400;
  padding: 20px;
  text-align: left;
  width: 33.3333%;
}

.search {
  background-color: #FFF;
  border: 1px solid #DDD;
  border-radius: 3px;
  color: #AAA;
  padding: 20px;
  margin: 50px auto 0px auto;
  width: 77%;
}





























 






