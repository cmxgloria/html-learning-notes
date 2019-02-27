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








<!DOCTYPE html>






 






