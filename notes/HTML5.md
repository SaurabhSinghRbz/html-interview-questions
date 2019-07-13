<dl>
  <dt>HTML Canvas Reference</dt>
  <dd><code>canvas</code> is an HTML element which can be used to draw graphics via JavaScript. This can, for instance, be used to draw graphs, combine photos, or create animations.</dd>

  <dt>Colors, Styles, and Shadows</dt>
  <dd>

|  Property    |	Description                                                                 |
|:-------------|:-------------------------------------------------------------------------------|
|fillStyle	   | Sets or returns the color, gradient, or pattern used to fill the drawing       |
|strokeStyle   | Sets or returns the color, gradient, or pattern used for strokes               |
|shadowColor   | Sets or returns the color to use for shadows                                   |
|shadowBlur	   | Sets or returns the blur level for shadows                                     |
|shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape           |
|shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape             |

  </dd>

  <dt>Line Styles</dt>
  <dd>

|Property	 |  Description                                                   |
|:-----------|:---------------------------------------------------------------|
|lineCap	 |Sets or returns the style of the end caps for a line            |
|lineJoin	 |Sets or returns the type of corner created, when two lines meet |
|lineWidth	 |Sets or returns the current line width                          |
|miterLimit	 |Sets or returns the maximum miter length                        |

  </dd>

  <dt>Rectangles</dt>
  <dd>
  
|Method	        |Description                                          |
|:--------------|:----------------------------------------------------|
|rect()	        |Creates a rectangle                                  |
|fillRect()	    |Draws a "filled" rectangle                           |
|strokeRect()	|Draws a rectangle (no fill)                          |
|clearRect()	|Clears the specified pixels within a given rectangle |
   
  </dd>

  <dt>Paths</dt>
  <dd>
  
| Method	      |   Description                                                                                 |
|:----------------|:--------------------------------------------------------------------------------------------- |
|fill()	          |Fills the current drawing (path)                                                               |
|stroke()	      |Actually draws the path you have defined                                                       |
|beginPath()	  |Begins a path, or resets the current path                                                      |
|moveTo()	      |Moves the path to the specified point in the canvas, without creating a line                   |
|closePath()	  |Creates a path from the current point back to the starting point                               |
|lineTo()	      |Adds a new point and creates a line to that point from the last specified point in the canvas  |
|clip()	          |Clips a region of any shape and size from the original canvas                                  |
|arc()	          |Creates an arc/curve (used to create circles, or parts of circles)                             |
|arcTo()	      |Creates an arc/curve between two tangents                                                      |
  
  </dd>

  <dt>Transformations</dt>
  <dd>
    
|Method	        |Description                                                                |
|:--------------|:------------------------------------------------------------------------- |
|scale()	    |Scales the current drawing bigger or smaller                               |
|rotate()	    |Rotates the current drawing                                                |
|translate()	|Remaps the (0,0) position on the canvas                                    |
|transform()	|Replaces the current transformation matrix for the drawing                 |
|setTransform()	|Resets the current transform to the identity matrix. Then runs transform() |
  
  </dd>

  <dt>Text</dt>
  <dd>
    
|Property	    |Description                                                       |
|:--------------|:---------------------------------------------------------------- |
|font	        |Sets or returns the current font properties for text content      |
|textAlign	    |Sets or returns the current alignment for text content            |
|textBaseline	|Sets or returns the current text baseline used when drawing text  |
|fillText()	    |Draws "filled" text on the canvas                                 |
|strokeText()	|Draws text on the canvas (no fill)                                |
|measureText()	|Returns an object that contains the width of the specified text   |

  </dd>

 <dt>HTML Layout Engines</dt>
 <dd>


|Engine	      |Status	        |Embedded in                                                                           |
|:------------|:--------------|:-------------------------------------------------------------------------------------|
|WebKit	      |Active	        |Safari browser, plus all browsers hosted on the iOS App Store                         |
|Blink	      |Active	        |Google Chrome and all other Chromium-based browsers like Opera and Microsoft Edge     |
|Gecko	      |Active	        |Firefox browser and Thunderbird email client, plus forks like SeaMonkey and Waterfox  |
|KHTML	      |Discontinued	  |Konqueror browser                                                                     |
|Presto	      |Discontinued	  |formerly in the Opera browser                                                         |
|EdgeHTML	    |Discontinued	  |formerly in the Microsoft Edge browser                                                |
|Trident	    |Discontinued	  |Internet Explorer browser and Microsoft Outlook email client                          |

 </dd>
</dl>


---

---

#### HTML 

---


---

#### What does a DOCTYPE do?

* DOCTYPE is an abbreviation for ```DOCument TYPE```.  
    A DOCTYPE is always associated to a ```DTD``` for ```Document Type Definition```.  

    A DTD defines how documents of a certain type should be structured (i.e. a `button` can contain a `span` but not a `div`), whereas a DOCTYPE declares what DTD a document supposedly respects (i.e. this document respects the HTML DTD).  

    For webpages, the DOCTYPE declaration is required. It is used to tell user agents what version of the HTML specifications your document respects.  
    Once a user agent has recognized a correct DOCTYPE, it will trigger the ```no-quirks mode``` matching this DOCTYPE for reading the document.  
    If a user agent doesn't recognize a correct DOCTYPE, it will trigger the ```quirks mode```.

    The DOCTYPE declaration for the HTML5 standards is `<!DOCTYPE html>`.

* it controls whether the browsers uses "standards" or "quirks" mode to render the document.

---

#### What happens when DOCTYPE is not given?
* The web page is rendered in quirks mode. 
    The web browsers engines use quirks mode to support older browsers which does not follow the W3C spec.
    
    In quirks mode CSS class and id names are case insensitive. In standards mode they are case sensitive.

---

#### What's the difference between standards mode and quirks mode?

* Quirks mode was to support websites built before standards became widely implemented.

* quirks mode in browser allows u to render page for as old browsers. This is for backward compatibility.

---

#### What's the difference between HTML and XHTML?

The Extensible Hypertext Markup Language, or XHTML, has two important notes for front end developers. 1) It needs to be well formed, meaning all elements need to be closed and nested correctly or you will return errors. 2) Since it is more strict than HTML is requires less pre-processing by the browser, which may improve your sites performance.

---

#### Why html5 doctype does not have a DTD definition?
    
* HTML5 is no longer based on SGML (Standard Generalized Markup Language) which actually requires a DTD for parsing/serializing, so we don't require a DTD anymore.
  

---

#### What does the lang attribute in html do?
    
* Helps in styling pages bu using them in css :lang() pseudo class Spelling and grammar checkers Languade detection by search engines


---

#### What is desktop first and mobile first design approach
* Desktop first : 
        General selectors and styles designed to make the site look good on DESKTOP screens defined globally. But they affect all devices, and must be overridden by max-width media queries targeting minimum screen size

* Mobile First : 
        General selectors and styles designed to make the site look good on small MOBILE screens go here. But they affect all devices, and must be overridden by min-width media queries targeting maximum scrren size
    
    In desktop first approach the media queries will be written with respect to max-width whereas in mobile first approach media queries will be written with respect to min-width
    

---

#### Are there any problems with serving pages as application/xhtml+xml?

---

#### How do you serve a page with content in multiple languages?

* The question is a little vague, I will assume that it is asking about the most common case, which is how to serve a page with content available in multiple languages, but the content within the page should be displayed only in one consistent language.

* When an HTTP request is made to a server, the requesting user agent usually sends information about language preferences, such as in the `Accept-Language` header. The server can then use this information to return a version of the document in the appropriate language if such an alternative is available. The returned HTML document should also declare the `lang` attribute in the `<html>` tag, such as `<html lang="en">...</html>`.

* In the back end, the HTML markup will contain `i18n` placeholders and content for the specific language stored in YML or JSON formats. The server then dynamically generates the HTML page with content in that particular language, usually with the help of a back end framework.

---

#### What kind of things must you be wary of when design or developing for multilingual sites?

* Use `lang` attribute in your HTML.
    
* Directing users to their native ```language``` Allow a user to change his country/language easily without hassle.
    
* Text in images is not a scalable approach Placing text in an image is still a popular way to get good-looking, non-system fonts to display on any computer. However, to translate image text, each string of text will need to have a separate image created for each language. Anything more than a handful of replacements like this can quickly get out of control.
    
* Restrictive words/sentence ```length``` Some content can be longer when written in another language. Be wary of layout or overflow issues in the design. It's best to avoid designing where the amount of text would make or break a design. Character counts come into play with things like headlines, labels, and buttons. They are less of an issue with free-flowing text such as body text or comments.
    
* Be mindful of how colors are ```perceived``` Colors are perceived differently across languages and cultures. The design should use color appropriately.
    
* Formatting dates and ```currencies``` Calendar dates are sometimes presented in different ways. Eg. "May 31, 2012" in the U.S. vs. "31 May 2012" in parts of Europe.

* Do not concatenate translated ```strings``` Do not do anything like `"The date today is " + date`. It will break in languages with different word order. Use a template string with parameters substitution for each language instead. For example, look at the following two sentences in English and Chinese respectively: `I will travel on {% date %}` and `{% date %} 我会出发`. Note that the position of the variable is different due to grammar rules of the language.

* Language reading ```direction``` In English, we read from left-to-right, top-to-bottom, in traditional Japanese, text is read up-to-down, right-to-left.

---

#### What are ```data-``` attributes good for?
* The HTML5 data attribute lets you assign custom data to an element. When we want to store more information/data about the element when no suitable HTML5 element or attribute exists

---

#### Consider HTML5 as an open web platform. What are the building blocks of HTML5?

* more semantic text markup

* new form elements

* new video and audio elements

* javascript API

* canvas and SVG

* geolocation API

* new data storage

---

#### Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

* ```cookie```: A text file saved on the users computer to store and retrieve data

* ```sessionStorage```: Is memory space in a browser to save temporary data until the window or tab is closed.

* ```localStorage```: Like cookie, where data can be saved and retrieved after browser sessions, but stored in memory like sessionStorage. Data is stored as plain key value pairs and can be stored as Json objects.

---

#### Describe the difference between ```<script>```, ```<script async>``` and ```<script defer>```.

* Normal Execution: script:
Parsing of the HTML code pauses while the script is executing. For slow servers and heavy scripts this means that displaying the webpage will be delayed.

* Deferred Execution: script defer
Delays script execution until the HTML parser has finished. A positive effect of this attribute is that the DOM will be available for your script. However, since not every browser supports defer yet, can’t rely on it.

* Asynchronous Execution: script async
HTML parsing may continue and the script will be executed as soon as it’s ready.    

---

#### Why is it generally a good idea to position CSS <link>s between <head></head> and JS <script>s just before </body>? Do you know any exceptions?
**Placing `<link>`s in the `<head>`**

Putting `<link>`s in the head is part of proper specification in building an optimized website. When a page first loads, HTML and CSS are being parsed simultaneously; HTML creates the DOM (Document Object Model) and CSS creates the CSSOM (CSS Object Model). Both are needed to create the visuals in a website, allowing for a quick "first meaningful paint" timing. This progressive rendering is a category optimization sites are measured in their performance scores. Putting stylesheets near the bottom of the document is what prohibits progressive rendering in many browsers. Some browsers block rendering to avoid having to repaint elements of the page if their styles change. The user is then stuck viewing a blank white page. Other times there can be flashes of unstyled content (FOUC), which can shows a webpage with no styling applied. 

**Placing `<script>`s just before `</body>`**

`<script>`s block HTML parsing while they are being downloaded and executed. Placing the scripts at the bottom will allow the HTML to be parsed and displayed to the user first.

An exception for positioning of `<script>`s at the bottom is when your script contains `document.write()`, but these days it's not a good practice to use `document.write()`. Also, placing `<script>`s at the bottom means that the browser cannot start downloading the scripts until the entire document is parsed. This ensures your code that needs to manipulate DOM elements will not throw and error and halt the entire script. If you need to put `<script>` in the `<head>`, use the `defer` attribute, which will achieve the same effect of downloading and running the script only after the HTML is parsed.

###### References

* https://developer.yahoo.com/performance/rules.html#css_top
* https://www.techrepublic.com/blog/web-designer/how-to-prevent-flash-of-unstyled-content-on-your-websites/
* https://developers.google.com/web/fundamentals/performance/critical-rendering-path/    

---

#### What is progressive rendering?

It is rendering the data as it’s being downloaded. This is particularly useful on documents that have tons of text. You can see it on a page that has a lot of text – and where the scrollbar will get shorter in length as more data comes in – increasing the vertical size of the document – yet, it would display the downloaded text immediately. As more data came down the pipe – the page would get longer. This didn’t rely on the closing body or html tag – and it certainly wouldn’t render the entire page on the server – then download – which is a standard complaint about modern frameworks. But there is a technique called “Flushing the Buffer” that can be implemented on the server. I don’t know that much about the technique, but found a few resources discussing it.

---

#### What is Critical Rendering Path

* Constructing the DOM Tree
* Constructing the CSSOM Tree
* Running JavaScript - parser blocking resource
* Creating the Render Tree
* Generating the Layout
* Painting

---

#### SSR VS CSR

* We are using server side rendering for two reasons:
    * performance benefit for our customers
    * Consistent SEO performance

* The main difference is that for SSR your server’s response to the browser is the HTML of your page that is ready to be rendered, while for CSR the browser gets a pretty empty document with links to your javascript. That means for SSR your browser will start rendering the HTML from your server without having to wait for all the JavaScript to be downloaded and executed.
    
* for SSR, the user can start viewing the page while all of that is happening. For the CSR world, you need to wait for all of the above to happen and then have the virtual dom moved to the browser dom for the page to be viewable.


---

#### Have you used different HTML templating languages before? what did you like about them?

---

#### Why you would use a srcset attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.

https://github.com/FAQGURU/FAQGURU/blob/master/topics/en/html5.md#why-you-would-use-a-srcset-attribute-in-an-image-tag-explain-the-process-the-browser-uses-when-evaluating-the-content-of-this-attribute

---

#### Why does invalid HTML work?

---

#### What is XHTML?
* https://www.thoughtco.com/what-is-xhtml-3464702

---

#### What is a Favicon? Where are favicons displayed?

---

#### Are HTML 5 tags case sensitive?

---

#### Why must the ID attribute be unique on each page?

---

#### What is a blockquote?

---

#### What is a meta tag?

---

#### How many cookies can you use on one website?

---

#### How big can a web cookie be?

---

#### What is the difference between Canvas and SVG graphics?    

https://www.sitepoint.com/how-to-choose-between-canvas-and-svg/

---

#### What is the difference between a ```<span>``` and a ```<div>```?
* ```<div>``` is a block level element which means it will render it on it's own line with a width of a 100% of the parent element.
* ```<span>``` is an inline element which means it will render on the same line as the previous element, if it is also an inline element, and it's width will be determined by it's content.


---

#### Name 5 common block-level and inline HTML elements.
* block elements ```<h1>, <p>, <ul>, <ol>, <li>```,
* inline elements ```<span>, <a>, <strong>, <i>, <img>```

---

#### What are semantic and non-semantic elements?
* A semantic element clearly describes its meaning to both the browser and the developer.
  
* non-semantic elements: ```<div>``` and ```<span>``` Tells nothing about its content. semantic elements: ```<form>, <table>, and <article>``` Clearly defines its content.

---

#### What is the purpose of ```main``` element?

The HTML ```<main>``` element represents the dominant content of the <body> of a document, portion of a document or application. The main content area consists of content that is directly related to or expands upon the central topic of a document, or the central functionality of an application. One important facet of ```<main>``` is that it can only be used once per page.

```<main>``` doesn't contribute to the document's outline; that is, unlike elements such as ```<body>```, headings such as ```<h2>```, and such, ```<main>``` doesn't affect the DOM's concept of the structure of the page. It's strictly informative.

---

#### Why to use HTML5 semantic tags?

As their name says, this is for semantic purposes only. It's for improving the automated processing of documents. Automated processing happens more often than you realize - each website ranking from search engines is derived from automated processing of all the website out there.

```css
// machine: okay, this structure looks like it might be a navigation element?
<div class="some-meaningless-class"><ul><li><a href="internal_link">...</div>

// machine: ah, a navigation element!
<nav class="some-meaningless-class"><ul><li><a>...</nav>
```

---

#### Define semantic markup. What are the semantic meanings for ```<section>, <article>, <aside>, <nav>, <header>, <footer>``` and when/how should each be used in structuring html markup?

* ```<header>``` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

* ```<article>``` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it’s meaining. Individual blog posts or news stories are good examples.

* ```<section>``` is a flexible container for holding content that shares a common informational theme or purpose.

* ```<footer>``` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.


---

#### When should you use ```section```, ```div``` or ```article```?

* ```<section>```, group of content inside is related to a single theme, and should appear as an entry in an outline of the page. It’s a chunk of related content, like a subsection of a long article, a major part of the page (eg the news section on the homepage), or a page in a webapp’s tabbed interface. A section normally has a heading (title) and maybe a footer too.

* ```<article>```, represents a complete, or self-contained, composition in a document, page, application, or site and that is, in principle, independently distributable or reusable, e.g. in syndication. This could be a forum post, a magazine or newspaper article, a blog entry, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.

* ```<div>```, on the other hand, does not convey any meaning, aside from any found in its class, lang and title attributes.

---

#### What is the difference between (```<i>``` and ```<em>```) and (```<b>```, ```<strong>```) and how will screen-readers react the to each tag?

---

#### What is the purpose of aria attributes?

---

#### Explain what inline styles and javascript are and when they are appropriate to use.

---

#### When is it acceptable to use font tags?

---

#### What is Character Encoding?

To display an HTML page correctly, a web browser must know which character set (character encoding) to use. This is specified in the tag:

```css
<meta charset="UTF-8">
```

---

#### What is the purpose of meta tags?

* Meta tags always go inside head tag of the HTML page
* Meta tags is always passed as name/value pairs
* Meta tags are not displayed on the page but intended for the browser
* Meta tags can contain information about character encoding, description, title of the document etc

```css
<!DOCTYPE html>
<html>
<head>
  <meta name="description" content="I am a web page with description"> 
  <title>Home Page</title>
</head>
<body>
  
</body>
</html>
```

---

#### What is the purpose of Charset meta tag?

---

#### What does async and defer refer in script tag ? Describe the difference between ```<script>```, ```<script async>``` and ```<script defer>```
* Async: Downloads the script file during HTML parsing and will pause the HTML parser to execute it when it has finished downloading.

* Defer: Defer downloads the script file during HTML parsing and will only execute it after the HTML parser has completed. Not all browsers support this.
    
* the async attribute is used to indicate to the browser that the script file can be executed asynchronously. The HTML parser does not need to pause at the point it reaches the script tag to fetch and execute, the execution can happen whenever the script becomes ready after being fetched in parallel with the document parsing.

* The defer attribute tells the browser to only execute the script file once the HTML document has been fully parsed.     

---

#### Experience with website optimization?

---

#### How to handle form validation?

---

#### What is viewport?

---

#### What is the difference between cookies, sessionStorage and localStorage?

---

#### Where should we place Javascript ```files``` top OR bottom. What are the advantages and disadvantages of either method. Where would you use these (Google webfonts you need to place on top + jQuery down or top)
        
        

---

#### Behavioral

---



---

#### What are your biggest strengths? Weaknesses?


---

#### What is your greatest achievement?
   

---

#### Tell me about 3 times you have failed. 
    // Almost anyone can come up with 1 or 2, but it can be hard to think of 3. 
    // Be sure to wait and be quiet while the candidate thinks and ponders the answer 
    // I often feel like the most insightful answers come towards the end of this question.
    

---

#### How did you prepare for this interview?


---

#### What are some of your hobbies or passions outside of work? How did you first get into them?


---

#### What is your availability?


---

#### Do you consider yourself weird? Why or why not?


---

#### Are there any questions that we didn’t ask you that we should have?



---


---

#### Why did you choose to learn FE?


---

#### How did you learn to code?


---

#### What sort of project are you looking for?    


---

#### Give me an example of a goal you set for yourself and how you achieved it.


---

#### If money weren’t an issue and you had to work on a project for 3 months, what would you create?


---

#### Where do you see yourself/ What do you want to do in 3/5 years? What kind of environment? How would this job fit into your plan and help you toward your goals?


---

#### If you could master one technology this year, what would it be?


---

#### What was your greatest challenge in FE?


---

#### What was your favorite part about FE?


---

#### What excites or interests you about coding?


---

#### What has been the hardest part about learning to code so far?


---

#### What did you learn yesterday/this week?


---

#### What are 3 big contributors to your success?  Who inspires you in the front-end community?


---

#### What is the last technical book you read?


---

#### What sort of websites or blogs do you read regularly? What do you like about them?


---

#### Do you use Git, GitHub?


---

#### Tell me about a time you improved a tool, task, or project you were working on. What was the circumstances? Why did you do it?  Do you have any other examples?


---

#### Do you have any side projects? What kind?


---

#### What's the coolest thing/project you've ever coded, what are you most proud of?


---

#### What is a recent technical challenge you experienced and how did you solve it?


---

#### Talk about your preferred development environment. 


---

#### What tools you use in regular workflow? 


---

#### What tools do you use for your day to day work? Language, IDEs/editors, version control, build systems, provisioning, etc.?


---

#### Which version control systems are you familiar with?


---

#### How do you stay on up-to-date with current web trends/innovations, latest front-end technologies and best practices? how do you decide what to invest time into and what not to?


---

#### What are some things you like about the developer tools you use?


---

#### What is a recent challenges you experienced and how did you solved those?


---

#### What was the last new technology or tool you learned?  Where did you learn about it?  Have you used it since?


---

#### When was the last time you got something wrong?  How did you know?  What did you learn from it?



---


---

#### Can you describe your workflow when you create a web page?


---

#### If you have 5 different stylesheets, how would you best integrate them into the site?


Break them up onto to different CDN servers to leverage domain sharding.

Employ the “new old” technique of adding “above the fold” css inline in the head of your document – reducing http requests and improve perceived performance.

Using SASS I would break up my files into related chunks – all of which are concatenated and compressed using compass, sass with gulp or grunt in your build process.


---

#### Can you describe the difference between progressive enhancement and graceful degradation?

* Graceful degradation is when you initially serve the best possible user experience, with all modern functionality, but use feature detection to “gracefully degrade” parts of your application with a fallback or polyfill.

* Progressive enhancement ensures a page works at the lowest expected abilities of browsers. So if you have a JavaScript web application that enhances a persons ability to send information to a database with features like ajax – at the very least you need to provide the ability for a person to send that same information without JavaScript enabled. In this case a simple form with full-page refresh will do what you need.

---

#### How would you optimize a website's assets/resources?

Concatenate and compress CSS, JavaScript and HTML files wherever possible, configure your server to deliver a Gzip files, cache resources, set longer expirations dates on http headers of resources you don’t expect to change often – such as a logo. Images can be some of the heaviest files we deliver, so compress wisely. Soon the picture element will be implemented across browsers, so we can optimize the delivery of image content. Also in the near future consider using WebP format for images – it is quite smaller in size than JPEG and PNG files. Finally, use a CDN or other domains to host your resources and leverage domain sharding.

---

#### What is the purpose of cache busting and how can you achieve it?

Browsers have a cache to temporarily store files on websites so they don't need to be re-downloaded again when switching between pages or reloading the same page. The server is set up to send headers that tell the browser to store the file for a given amount of time. This greatly increases website speed and preserves bandwidth.

However, it can cause problems when the website has been changed by developers because the user's cache still references old files. This can either leave them with old functionality or break a website if the cached CSS and JavaScript files are referencing elements that no longer exist, have moved or have been renamed.

Cache busting is the process of forcing the browser to download the new files. This is done by naming the file something different to the old file.

A common technique to force the browser to re-download the file is to append a query string to the end of the file.

```css
    src="js/script.js" => src="js/script.js?v=2"
```

The browser considers it a different file but prevents the need to change the file name.    


---

#### How many resources will a browser download from a given domain at a time?


---

#### Name 3 ways to decrease page load (perceived or actual load time).

1) LocalStorage 2) Caching resources 3) dns-prefetch (sample below) 4) Keep resources on a CDN

---

#### If you jumped on a project and they used tabs and you used spaces, what would you do?


---

#### What is Flash of Unstyled Content? How do you avoid FOUC?

---

#### What is Flash of Unstyled Text? How do you avoid FOUT?


---

#### Explain what ARIA and screenreaders are, and how to make a website accessible.

Screen readers are software programs that  provide assistive technologies that allow people with disabilities (such as no sight, sound or mouse-ing ability) to use web applications. You can make your sites more accessible by following ARIA standards such as semantic HTML, alt attributes and using [role=button] in the expected ways

---

#### What is the purpose of the ```alt``` attribute on images?

The ```alt``` attribute provides alternative information for an image if a user cannot view it. The ```alt``` attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

---

#### Explain some of the pros and cons for CSS animations versus JavaScript animations.

Regarding optimization and responsiveness the debate bounces back and forth but, the concept is:

* CSS animations allows the browser to choose where the animation processing is done, CPU or the GPU. (Central or Graphics Processing Unit)

* That said, adding many layers to a document will eventually have a performance hit.

* JS animation means more code for the user to download and for the developer to maintain.

* Applying multiple animation types on an element is harder with CSS since all transforming power is in one property transform

* CSS animations being declarative are not programmable therefore limited in capability. 

---

#### What does CORS stand for and what issue does it address?

Cross Origin Resource Sharing. To address the fact that browsers restrict cross-origin HTTP requests initiated from within scripts. CORS gives web servers cross-domain access controls, which enable secure cross-domain data transfers.

---

#### Describe how you would create a simple slideshow page.


---

#### What's your favorite feature of Internet Explorer?


---

#### What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?


---

#### Some people write good HTML, some people write bad HTML. What do you consider to be good HTML?


---

#### Tell me about a responsive project you have worked on recently?


---

#### Do you have any personal projects? Tell me about them.


---

#### Ways to decrease page load?


---

####  Ways to improve website performance

* Minimize HTTP Requests
    * Sites are mainly slow because of too many (or too large) HTTP requests. We can eliminate unnecessary request;
        * combined files: js to a file, css to a file
        * CSS sprites: CSS Sprites are the preferred method for reducing the number of image requests. Combine your background images into a single image and use the CSS background-image and background-position properties to display the desired image segment.

* Use a Content Delivery Network CDN

    * A CDN is essentially many optimized servers around the world that deliver web content to users based on their geographic location. This means big performance improvements for site users. Because, say, if a person accessing your site in India, they will be retrieving web content from a server nearby

* Optimize Images:

    * image sizes make a huge difference to site speed. The larger content/images, the slower the site. we could:
        * Changing the resolution: reducing the “quality” of the image (and thereby the file size)
        * Compressing the picture: increasing the efficiency of image data storage
        * Cropping the picture: when cropping, you are cutting out unneeded areas and thus making the image smaller in size

* Put Scripts at the Bottom:

    * Javascript files can load after the rest of your page. The simplest solution is to place your external Javascript files at the bottom of your page, just before the close of your body tag. Now more of your site can load before your scripts. Another method that allows even more control is to use the defer or async attributes when placing external .js files on your site.
        
        * Async tags load the scripts while the rest of the page loads, but this means scripts can be loaded out of order. Basically, lighter files load first. This might be fine for some scripts, but can be disastrous for others.
        
        * The defer attribute loads your scripts after your content has finished loading. It also runs the scripts in order. Just make sure your scripts run so late without breaking your site.

* Add an Expires or a Cache-Control Header

    * Web page designs are getting richer and richer, which means more scripts, stylesheets, images, and Flash in the page. A first-time visitor to your page may have to make several HTTP requests, but by using the Expires header you make those components cacheable. This avoids unnecessary HTTP requests on subsequent page views. Expires headers are most often used with images, but they should be used on all components including scripts, stylesheets, and Flash components.

* Gzip Components

    * Compression reduces response times by reducing the size of the HTTP response. Gzipping generally reduces the response size by about 70%.

* Put Stylesheets at the Top:

    * This is because putting stylesheets in the HEAD allows the page to render progressively.

* Avoid CSS Expressions

* Use GET for AJAX Requests:

    * Ajax is that it provides instantaneous feedback to the user because it requests information asynchronously from the backend web server

* Make JavaScript and CSS External:

    *  Using external files in the real world generally produces faster pages because the JavaScript and CSS files are cached by the browser. JavaScript and CSS that are inlined in HTML documents get downloaded every time the HTML document is requested. This reduces the number of HTTP requests that are needed, but increases the size of the HTML document. On the other hand, if the JavaScript and CSS are in external files cached by the browser, the size of the HTML document is reduced without increasing the number of HTTP requests.

* Use get to ajax request:

    *  POST is implemented in the browsers as a two-step process: sending the headers first, then sending data. So it's best to use GET, which only takes one TCP packet to send (unless you have a lot of cookies).

* No 404s:

    * HTTP requests are expensive so making an HTTP request and getting a useless response (i.e. 404 Not Found) is totally unnecessary and will slow down the user experience without any benefit.

* Reduce Cookie Size:

    * HTTP cookies are used for a variety of reasons such as authentication and personalization. Information about cookies is exchanged in the HTTP headers between web servers and browsers. It's important to keep the size of cookies as low as possible to minimize the impact on the user's response time.

* Reduce DNS Lookups

* Minify JavaScript and CSS

* Avoid Redirects

* Remove Duplicate Scripts

* Configure Etags

* Make Ajax Cacheable

* Post-load Components

* Preload Components

* Reduce the Number of DOM Elements

* Minimize the Number of iframes

* Minimize DOM Access

* Optimize CSS Sprites

* Don't Scale Images in HTML

* Make favicon.ico Small and Cacheable

* Avoid Empty Image src

---

#### What tools do you use to test your code's performance?


---

#### How many resources will a browser download from a given domain at a time?


---

#### How would you optimize a website's assets/resources?


---

#### Can you talk about how you have considered performance when developing a website?


---

#### What performance issues do you anticipate when building a website?


---

#### How would you go about troubleshooting a slow website?


---

#### What are some ways to prevent web browser caching?


---

#### How do you do browser compatibility testing?


---

#### What is your favorite browser?  What sort of tools do you use to debug websites?


---

#### What do you think of “hacks”? When should they be used in your code and when should they be avoided?


---

#### What are the advantages of client side rendering vs. server side rendering? If you were building our site which would you use and why?


---

#### How do you test the performance of your code and/or web pages?


---

#### What is Flash of unstyled content?


---

#### How to avoid Flash of unstyled content.


---

#### How does the browser rendering engine work?

In order to render content the browser has to go through a series of steps:

* Document Object Model(DOM)
    
* CSS object model(CSSOM)
    
* Render Tree
    
* Layout
    
* Paint.
    

---

#### Can you explain the difference between GET and POST?
* https://stackoverflow.com/questions/3477333/what-is-the-difference-between-post-and-get    
        

---

#### What is the DOM? How does the DOM work? Explain in as much detail as possible.

The DOM (Document Object Model) is a cross-platform API that treats HTML and XML documents as a tree structure consisting of nodes. These nodes (such as elements and text nodes) are objects that can be programmatically manipulated and any visible changes made to them are reflected live in the document. In a browser, this API is available to JavaScript where DOM nodes can be manipulated to change their styles, contents, placement in the document, or interacted with through event listeners.


* The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.

* The DOM is constructed progressively in the browser as a page loads, which is why scripts are often placed at the bottom of a page, in the <head> with a defer attribute, or inside a DOMContentLoaded event listener. Scripts that manipulate DOM nodes should be run after the DOM has been constructed to avoid errors.

* document.getElementById() and document.querySelector() are common functions for selecting DOM nodes.

* Setting the innerHTML property to a new value runs the string through the HTML parser, offering an easy way to append dynamic HTML content to a node.


---

#### What is the SAME ORIGIN POLICY


---

#### Comparision of browsers like Chrome, Firefox, Internet explorer, Safari etc
* Chrome: 
    * Layout rendering ```engine``` Webkit. 
    * JavaScript ```engine``` V8

* Firefox: 
    * Layout rendering ```engine``` Gecko. 
    * JavaScript ```engine``` Spider monkey
        
* Internet explorer: 
    * Layout rendering engine``` Trident. 
    * JavaScript ```engine``` Chakra
        
* Safari:
    * Layout rendering ```engine``` Webkit. 
    * JavaScript ```engine``` JavascriptCore i.e Nitro


---

#### Open up your last project, explain your code and thought process.
    // This is probably one of my favorite and most important questions. 
    // When I hire I like to hire candidates who are very passionate about what they do, 
    // and so programming isn’t something they just do at their job. 
    // They are actually passionate about it and pursue their own projects outside of work.
    

---

#### Teach me about something for the next 10 minutes.  
    // You are looking for them to select a topic they know 
    // I generally don’t care if they are technical or not
    // and how well they communicate and break things down.


---

#### Explain the concept of cloud computing to my older (not-very-technical) mother. 
    // I actually had to do this in real life and it was harder than I expected. 
    // Another example is explain a database to someone’s grandparents.
    

---

#### In as much detail as you like, explain what happens when I type "google.com" into my browser's address bar and press enter.    
  

---

#### How would you explain the Internet to a child?  


---

#### Explain the importance of standards and standards bodies.
  
  
---

#### What happens when somebody hits the URL in browser?


---

#### What are HTTP methods? List all HTTP methods that you know, and explain them.


---

#### Why has it been better to serve site assets from multiple domains?


---

#### Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.



---

---

#### Version Control

---



---

#### What is your preferred version control software? 

---

#### Do you have experience working on a project versioned with Git?

---

#### What is your opinion on pull requests (and code reviews)?

---

#### What is the difference between Git and Github?

---

#### What would you consider an effective Git workflow?

---

#### What are build tools good for? Which ones are you familiar with?



---

---

#### Agile

---


---

#### Do you have experience working in an agile team?

---

#### Do you work in sprints, or using the kanban approach? 

---

#### Do you have a preference, and why?

---

#### Work in Agile / Scrum?

---

#### Have you worked with QA? How you QA/test your code?

---

#### How did you communicate progress in your previous role?  Did that process always work?  What could have been done differently to keep everyone on the same page?

---

#### Tell me about a time when you had a miscommunication at work.  What happened?  If you could do it all over again would you alter your actions?  Why or why not?

---

#### Have you ever disagreed with your boss or manager?  What did you do?  If you haven’t had this happen, imagine that it did, how would you handle this situation?

---

#### Give me an example of a time when you were able to communicate and work with another person even when they may not have personally liked you (or vice versa).

---

#### How well do you work on teams?

---

#### What did you like/not like about your last job?

---

#### What would your peers and instructors say about you?

---

#### Do you still write code in your job? Do you love it? 
    // This is more targeted at managers or leaders, 
    // since many do not need to be writing code to do their jobs. 
    // Hopefully this question could lead to an interesting conversation on role, etc.

---

#### Why do you want to work at [company name]? Have you used our products? Is there a particular area or feature that got you excited?

---

#### Give an example of when you completed a task without being asked. Can you give me another example?  Another?

---

#### If you were hiring someone in this role, what would you look for?  What sort of interview questions would you ask? Do you have a favorite question?

