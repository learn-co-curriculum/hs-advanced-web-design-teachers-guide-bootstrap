###SWABATs

+ understand how to use Bootstrap, its limitations and when and why to use it
+ Install Bootstrap source code and add it to a project
Use the Bootstrap grid system - rows and columns - to organize/structure a page
+ Understand how to style content (text, lists, tables, forms, buttons. images, etc.) using Bootstrap
+ Incorporate additional features like glyph icons, dropdown menus, breadcrumbs, nav bars
+ Incorporate JavaScript components like modals, dropdown menus, tooltips, popovers, accordions, carousel
+ Understand Bootstrap best practices because with great power comes great responsibility

###Methods
You guys spent a lot of time with HTML and CSS in the last class, but we haven’t focused much on that here. Luckily there are some great tools out there to help you get up and running with a good looking site using preset CSS. Bootstrap is one of those resources and today we’re going to walk through how to use Bootstrap.

###Lesson Plan
<b>Bootstrap</b>

+ It's pretty easy to soup up your site with some Bootstrap. This walkthrough will take you through the necessary steps to integrate Bootstrap to get your site looking slick and professional.
+ Start by setting up a basic index.html file with your doctype, html tags, head, and bodt tags.
+ Include Bootstrap CSS
	+ Within the `<head>` tag, under the `<title>` tag, copy this link to the Bootstrap CSS.
		`<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css">`
	+ This will give your site/app access to all of Bootstrap’s CSS styles
+ Include jQuery and Bootstrap JavaScript Libraries
	+ Include the source code for jQuery and Bootstrap Javascript **right before the closing** `</body>` **tag**. 
	+ This code gives your site cool animations and added functionalities to make for a better user experience.

			<!-- Bootstrap core JavaScript================================================== -->
			<!-- Placed at the end of the document so the pages load faster -->
			<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
			<!-- Latest compiled and minified JavaScript -->
			<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/js/bootstrap.min.js"></script>
	
+ Add Internet Explorer support
	+ There are a lot of different browsers people use nowadays, so sometimes we need to include extra code to make sure our site displays correctly on every browser. Here's what you need to to add to make sure everything functions properly if the user is on Internet Explorer. Add it to the **bottom of your** `<head>` **section before the closing** `</head>` **tag**.

	
			<!--[if lt IE 9]>
			<script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js">
			</script><script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
			<![endif]-->
+ Set Up Your Container
	+ To make sure we're assigning the right styles to the right content, it's important to wrap content in containers. Web developers often use `<div>` tags to draw an imaginary box around a chunk of HTML. This defines a section of code separate from the rest of the code. 
	+ Our first container is going to wrap up all the code in the body. So **right after your opening** `<body>` **tag**, paste the following code. Make sure **Everything** you add to the body after this point goes inside this tag!

			<div class="container">
  			<!-- MAKE SURE EVERYTHING YOU WANT FOR YOUR BODY GOES INSIDE THIS TAG! -->
			</div>
+ Add in Cool Stuff: Navigation Bar
	+ Now comes the fun part. We'll start adding in different components to spruce up our website. 
	+ Check out the Bootstrap documentation to see the variety of elements you can play around with. 
	+ Basically all you need to do is copy the html code from the documentation and throw it into your project. 
	+ The essence of Bootstrap is that Bootstrap has a bunch of class selectors that are added html elements that assign the pre-defined styles to that particular element.
	+ Let's add a navigation bar first. A navigation bar is important to keep your users from getting lost on your site. Add this code as the first line under the `<div class="container">` tag, and don't forget to link to other pages on your site in each of the `<a>` tags.

			<div class="navbar navbar-default navbar-static-top" role="navigation">
			    <div class="container">

			        <div class="navbar-header">
			            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
			            <span class="sr-only">Toggle navigation</span>
			            <span class="icon-bar"></span>
			            <span class="icon-bar"></span>
			            <span class="icon-bar"></span>
			            </button>
			            <a class="navbar-brand" href="index.html">Home</a>
			        </div>
			<div class="navbar-collapse collapse">
			            <ul class="nav navbar-nav">
			                <li class="active">
			                    <a href="#">Turtles</a>
			                </li>
			                <li>
			                    <a href="#">Movie</a>
			                </li>
			                <li>
			                    <a href="#">Legacy</a>
			                </li>
			            </ul>
			        </div><!--/.nav-collapse -->

			    </div>
			</div>
+ Add in Cool Stuff: A Heading
	+ Headings let a user know where they are. Let's add a heading underneath the navigation bar, like so:
	
				<div class="page-header">
	    			<h1>Steph's Sweet Teenage Mutant Ninja Fan Page</h1>
				</div>
+ Add in Cool Stuff: A Table
	+ Here's a standard table that has information about the different ninja turtles. The added Bootstrap classes give the table visual pizzazz.
		
		
				<table class='table table-hover table-responsive table-bordered'>
				  <tr>
				    <th>Turtle</th>
				    <th>Color</th>
				    <th>Personality</th>
				  </tr>
				  <tr>
				    <td>Michelangelo</td>
				    <td>Orange</td>
				    <td>Best turtle. Comedian of the bunch.</td>
				  </tr>
				  <tr>
				    <td>Leonardo</td>
				    <td>Blue</td>
				    <td>Courageous leader. Oldest child syndrome.</td>
				  </tr>
				  <tr>
				    <td>Raphael</td>
				    <td>Red</td>
				    <td>The bad boy. Very New York attitude.</td>
				  </tr>
				  <tr>
				    <td>Donatello</td>
				    <td>Purple</td>
				    <td>Techy and smart. Probs a good programmer.</td>
				  </tr>
				</table>
+ Code Recap
	+ You can see all the code for a demo site in the `index.html` file included in the [https://github.com/flatiron-school-curriculum/hs-bootstrap-walkthrough](https://github.com/flatiron-school-curriculum/hs-bootstrap-walkthrough)  repository. This is a very simple implementation of Bootstrap's features. Have fun exploring the different Bootstrap elements and incorporating them into your projects. 
	+ Remember, the key to Bootstrapping your site is adding the Bootstrap classes to HTML tags that enclose your content.
+ Resources
	+ [http://getbootstrap.com](http://getbootstrap.com)
	+ [http://bootstrapbay.com/blog/bootstrap-3-carousel-tutorial](http://bootstrapbay.com/blog/bootstrap-3-carousel-tutorial) 

<b>UX/UI</b>

+ We covered a lot of design principles in the Intro to Web Design course but we haven’t talked about that much in this class. As you guys prepare to build your own projects it’s important to think about designing your application or web site with your user in mind.
+ Let’s review a few of the design principles that will help you build a project that is user friendly and visually pleasing:
+ The easiest way to make your site usable is to reduce options and make the options available as clear as possible. 
+ Users have a tendency to read/click on the first thing that looks good - your job is to guide them to that text/button/link and make sure it is what they want.
+ How do you do this?
+ Visual Hierarchy
	+ Figure out what is most important and MAKE IT BIG! Or make it bright or make it dark. Just make sure it stands out so that everyone will want to read it, click on it, be friends with it.
+ White Space
	+ White space is your friend. It makes your site look clean and it let’s the important things stand out more readily. Don’t forget about white space on the small screen too. Strategic white space can make designing a responsive page and designing for mobile easier and more visually pleasing.
+ Color Theory
	+ The colors you choose set the tone for your website. Take a look at the color theory resources on Learn for help picking out a color scheme that fits the design and tone of your page. It’s probably a good idea to stick to 3 color at most.
+ Typography
	+ Remember to not only think about how the font reflects the tone of your website - also be mindful of spacing and sizing. It’s a good idea to stick with two fonts - one for headers and one for body text. Check out the resources on Learn for help.
+ And of course do not lose sight of the purpose of your application/site. Who are you creating this for? How will they use it? Not sure? TEST
+ Testing out your application/site and getting feedback from users is THE BEST way to figure out what works and what doesn’t. 
	+ Show what you are working on to your friends and family 
	+ Pay close attention to how they interact with the site
	+ Ask lots of questions
	+ Be open to their feedback - And REMEMBER people are commenting on your work and not on YOU as a person - don’t take it personally.


<p data-visibility='hidden'>View <a href='https://learn.co/lessons/hs-advanced-web-design-teachers-guide-bootstrap' title='SWABATs'>SWABATs</a> on Learn.co and start learning to code for free.</p>
