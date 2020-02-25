# Code Inst. Milestone Project 01 - Personal Site built with Boostrap 

 

## Synopsis 

The purpose of the website is present the skills I have learned in building a responsive, mobile-first website. It demonstrates how I used HTML and CSS to create a website that dynamically changes layout structure based on the current users screen size while retaining a positive UX design and aesthetic.  

It’s second goal is to present information regarding me and my previous work to the public. To build on the promotional material online that represents me and my abilities to any prospective employer. It allows users to preview samples of my previous work and then direct them to live versions of working content. It allows users to connect to my github and linked-in profiles but also via a php mailer form. Obviously PHP is not part of this course so the pages were made as HTML but can be easily edited to work with any server side mailer. 

 

## UXD 

### Strategy 

There are 5 main goals of the website: 

1. Create a valuable online presence 
2. Promote skills in a positive light   
3. Increase public awareness of abilities  
4. Increase requests for a copy of CV 
5. Connect with Github & Linked-in 

 

### Scope 

This section determines what the users should be able to do on the website:

1. Organised list of technologies and how competent I am with them on the Home page. 
2. Demonstrate finished examples of work. 
3. Demonstrate finished examples of work and link to Github code examples. 
4. Users can use "Request CV" button to make direct contact. 
5. Users can use contact page to make direct contact. 

 

### Structure 

At this point I started working on what information, pages, features, and calls to action would be applicable and how they would be grouped. 

I proposed four pages. A home page detailing my skill both software and languages. I divided my work into two categories “Work” and “Games” which I then suggested might make separate pages, and finally a contact page. I felt this layout in four pages would allow a solid structure for the goals of the scope to easily sit into. I considered the remaining goals of the scope could be best met by placing request CV, GitHub and LinkedIn links in the footer, therefore providing a subtle prominence without being in a annoyance as they would have been as a floating sidebar. 

  

### Skeleton 

I started using https://www.draw.io to work up wireframes of the website. However, I found it very limited and moved to http://www.mocqups.com which provided extra functionality. Especially the ability to create click/touch areas that allow users to prototype interaction and navigation. If viewed using Adobe Acrobat or directly in a chrome browser the interface simulates interaction and navigation for better prototyping. Sadly, this functionality is void when viewed via the GitHub repository. 

[Full Site Mobile & Desktop wireframe ](https://github.com/mcgarry/CI_Milestone_01/blob/master/UX/04-skeleton/04-skeleton.pdf)

 

### Surface 

The Surface design section of a website, or how it looks, feels. I wanted the design to be clean and the colour scheme to be light and refreshing.  

I decided on a simple white background all areas of the site. I separated the menu from the content area with a banner the indicates the current page and has an image as background. I separate the content area from the footer with my client list. The client list and bottom of the menu have a drop shadow effect. The shadow effect combined with the banner and client list act to define sections of the site and lift the remaining content area’s so that the user almost forgets they are all plain white. 

The introduction of the red and dark grey adds a dynamic nature to the visual experience. The red colour also acts as a highlight important content and define the separation on content. The dark grey make the smaller text easy on the eye and more legible than a straight black.  

The Google fonts “Playfair Display” and “Homemade Apple” make up the main stay of font choices within the content. “Playfair Display” expresses a strong traditional style and is mostly almost black in colour. “Homemade Apple” is more a risk to use. It is either red or reversed in white out of a red background. While not as immediately legible as the conservative “Playfair Display”, “Homemade Apple” offers a juxtaposed playful style that sits well with its opposing font. 

Does this smell like value? - In my opinion it reeks of it 😊 

 

### What changed after user design experience (UDX) phase 

I noticed that I had a big skillset that I was not listing. I made use of the home page to list both the software I've used and the software languages I can code and the ones I will be able to code when I'm finished the course. 

 

## Functionality 

The website is fully responsive, on desktop and larger screen sizes the structure is changed to allow better functionality by changing the location of buttons. All pages have a nav bar, banner, content and a footer. 

 

The navigation is a customed bootstrap solution with links to four pages. The banner is fully responsive showing a large logo on mobile screens and smaller on ipad an desktop.  

 

The content consists of four pages. They are About, Corporate Work, Games and Contact. While each page contains links to samples of my work or previous clients, the contact and request pages propose to eventually use a php mailer form that will not operate on the GitHub pages. 

 

The footer consists of a banner and some ways to contact me directly. The footer banner is mostly a client list that allows users to link the various companies I've provided services for in the past. Below that are links to my Linked-In and GitHub accounts. 

 

## Technologies Used 

* HTML5 
* CSS3 
* Bootstrap 
* GIT 
* GITHUB 
* Google Chrome developer tools 
* Gitpod IDE 
* WebStorm IDE 
* Javascript and JQuery are used by bootstrap 
* Javascript for fancybox email confirmation on contact form 


 

## Deployment 

 

The website was built using the Gitpod IDE and later the WebStorm IDE. An online Github.com repository was used but change to a local GIT directory. Both used version control and then saved/uploaded to Github. Because the site will evenutally use php it was deployed to a cpanel webserver and can be viewed at https://www.3rdcastle.com/ci/ 

 

## Installation 

 

Using the clone link above run this command in the directory you wish to copy the site to.   

Inside a command terminal use:  

$: git clone https://github.com/mcgarry/CI_Milestone_01.git  

 

## Unique Elements 

 

 

## Tests 

Making heavy use of the web developer tools in both Chrome and Firefox, all pages and functionality were testing using the Chrome web developer tools with the following screen size layouts: Galaxy S5, Pixel2, Pixel2(XL), iPhone 5/SE, iPhone 6/7/8, iPhone 6/7/8 Plus, iPhone X, iPad,  iPad, and the following standard screen width 480, 600, 768, 992, and 1382px. 

All pages were validated for html using: https://validator.w3.org/ 

The css file was validated using: https://jigsaw.w3.org/css-validator/ 

The following url highlights two errors that remain. 

https://validator.w3.org/nu/?doc=https%3A%2F%2Fwww.3rdcastle.com%2Fci%2F 

The errors still state that inputs and labels must not appear as a descendant of a button, but these errors assume that the form elements are being used to record information within a form. Actually, this nesting of tags allows the code to perform an animation of a font awesome icon on click/touch using only CSS and is a consequence of using only CSS to perform animations without an triggerable event.  

To drop down the mobile menu the user must click/touch the font awesome chevron down icon on the top navbar. Most instances leave the icon institute at the top and use an animated gif to indicate a change in icon purpose ( burger to an close “X” for instance). In this build, the menu opens and the icon animates down. I wanted to rotate the icon as animated down so that it ended with a chevron up, indicating that the used could click/touch the same icon to close the menu.  

Having not covered JavaScript yet on the course, I explored other possibilities of how to animate the icon within the material covered on the course so far. The problem was how to circumvent the necessity for JavaScript to trigger the onclick event, and hence trigger the animation. The solution was to wrap a label and input tag with a button tag, even though there was no form for the input or label. The validator assumes I’m making a form and it is correct that they strictly should not be wrapped in a button tag, but that is not what they are being used for. In short, the error is strictly correct, but the tag nesting is not being used for a form, its being used so that an event can be triggered within CSS without using JavaScript. 

 

## Work based on other code 

 

All of the code is my own. Naturally I used frameworks such as JQuery and Bootstrap covered on the course and I tried where possible to find solutions that matched the content taught. I also used Fancybox for my popup form 


#Attribution:

	
	Navbar:
	Navbar Icon
	URL: https://getbootstrap.com/docs/4.4/components/navbar/#toggler
	URL: 	https://stackoverflow.com/questions/54417421/how-to-change-bootstrap-4-navbar-collapse-icon-with-custom-svg-image
					
	Menu Icons:	
	Scale:
	URL: https://stackoverflow.com/questions/28564793/changing-width-of-font-awesome-icons/28565030
	Rotate:
	URL: http://jsbin.com/fulocomu/1/edit?html,css,output
	
	CSS onClick effect
	URL:https://stackoverflow.com/questions/13630229/can-i-have-an-onclick-effect-in-css/32721572
			
	Checked / unChecked
	URL: https://stackoverflow.com/questions/8846075/css3-unchecked-pseudo-class

	Div Frame - image wide white border and gradient shadow
	ref: https://www.w3schools.com/cssref/css3_pr_box-shadow.asp
	
	Buttons - 
	ref: https://www.w3schools.com/css/tryit.asp?filename=trycss_buttons_basic

	Rollover Icon -
	Ref: https://www.tutorialrepublic.com/faq/how-to-change-image-on-hover-with-css.php
	
	Popup Form -
	Ref: https://fancyapps.com/fancybox/3/docs/#iframe

	Scrolling content with still background
	URL: https://stackoverflow.com/questions/28563479/scroll-transparent-div-over-div-with-background-image

	Burger Menu
	URL: https://getbootstrap.com/docs/4.4/components/navbar/#toggler
	URL: https://www.w3schools.com/howto/howto_css_menu_icon.asp

