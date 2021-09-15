# Lab 1 Writeup

## Introduction
**Name:** Garrett Cooper  
**Date:** 14/09/2021  
**Lab Title:** Lab 1  


## Executive Summary
In this lab, I created a visually pleasing task list website. I wrote and implemented the HTML, CSS, and JavaScript it uses to display different task as well as 
style components. Those conponents include multiple input types, classes, and events. I created a development environment using Docker and a live server 
environment using Amazon Web Services. Using git, I pushed my files to a GitHub repository. 


## Design Overview
### Files:
- *index.html* - Contains HTML code for website, loads HTML base of page
- *style.css* - Contains CSS code for website, loads CSS styling for page
- *script.js* - Contains JavaScript code for website, displays JSON of new task data in an alert
- *docker-compose.yml* - Creates Docker development environment
- *favicon.io* - Favicon image
- *instructions.md* - Lab instructions
- *Screen Shot 2021-09-14 at 8.02.15 PM.png* - Design overview screenshot
- *Screen Shot 2021-09-14 at 8.02.38 PM.png* - Design overview screenshot
- *Screen Shot 2021-09-15 at 10.17.01 AM.png* - Design overview screenshot

### Screenshots
- Screenshot before CSS  
![favicon](https://github.com/gncoop/ITC-210-Lab1b/blob/main/instructions/Screen%20Shot%202021-09-15%20at%2010.17.01%20AM.png)
  
- Screenshot of web page upon load with CSS
![webpage load](https://github.com/gncoop/ITC-210-Lab1b/blob/main/instructions/Screen%20Shot%202021-09-14%20at%208.02.15%20PM.png)  
  
- Screenshot of web page demonstrating functionality of components
![webpage functionality](https://github.com/gncoop/ITC-210-Lab1b/blob/main/instructions/Screen%20Shot%202021-09-14%20at%208.02.38%20PM.png)


## Questions
- What is the purpose of using Docker containers?
  - Docker containers allow us to create a local development environemt. This gives us an easy way to test our code as we write it and host it on our machine.
- Why is it useful to have both a development environment and a live server environment?
  - It's useful to have both because a development environment allows us to easily test any changes to make sure they are working before we add them to the 
 live server. If we don't do that we risk introducing bugs to our live server or breaking it.
- What is the purpose of using a code versioning tool (i.e. Git)?
  - The purpose is that it conveniently improves our ability to code. It allows us to track the changes in the code, maintains the original code, and allows more 
  than one person to work on source code without affecting each other.
- What is the difference between a CSS rule with an *element* selector and one with a *class* selector? When would you use each?
  - The difference is what gets the style rules dictated by the CSS. A rule with an *element* selector will add style rules to a whole HTML element, while a rule 
  with a *class* selector will only apply style rules to elements of the HTML with the class added to it. You would use *element* when you want a whole block 
  of HTML to match stylisticly, and *class* when you want to style a single or several specific elements with a style rule.
- What are the advantages of putting your styles in a separate .css stylesheet instead of in the `<style>` element of `<head>`?
  - The advantages include the ability to present a document in mupltiple styles by using multiple stylesheets, restyle the document without changing the HTML 
  code, edit the appearance of mutliple web pages with one stylesheet, and it reduces the file size of the HTML document, which leads to faster loading.
- How do web browsers choose which CSS to use for an HTML element when the CSS rules contradict each other?
  - They choose depending on the order of significance of the selector of the HTML element. ID selectors will be applied in preference of a conflicting class 
  selector, and class selectors in preference of a conflicting element selector.
- Why should you disable directory access for your server?
  - You should disable it because when enabled it allows attackers to browse the directory, giving them the potential to exploit web server vulnerabilities and 
  access to all the information in the directory.


## Lessons Learned
### CSS Style Sheet Linking
The problem was the HTML not linking to the CSS stylesheet. The name of the CSS stylesheet and the href in the HTML document must match. If it does not, the 
HTML will not be able to access the stylesheet and the page will be loaded in basic HTML. This is becasue the HTML document does not have the correct address 
and therefore cannot find the stylesheet. The solution to this was to enter the correct filepath and file name in the href of the HTML document.

### Create Task Buttom Input Type
The problem was the "Create Task" button did not have the correct input type. A button is an input type, and the input type must be set to the correct identifier
for the button to function properly. If a button has the input type "button", *input type="button"*, it will just be a button. The "Create Task" button required 
for the lab needs to have a submit function. For that to happen, the input type must be changed to *input type="submit"*. This gives the button the submit function,
as the lab requires.

### Delete Icon Name
The problem was the delete icon did not have the correct icon name. This lab required changing the delete buttons to custom icons drawn from fonts.google.com. 
Each icon in the Material Icons Directory has a unique name and it must be entered correctly for the icon to display. Once the the correct name entered, 
in this case *highlight_off*, the correct icon displayed.


## Conclusions
- Write code in HTML
- Write code in CSS
- Link multiple external files to one HTML file
- Display JavaScript data in JSON
- SSH into a live server
- Set up a local development environment
- Access HTML through id's and classess
- Use git in the terminal


## References
- https://www.w3schools.com/tags/att_input_type_button.asp
- https://www.w3schools.com/css/css_positioning.asp
- https://stackoverflow.com/questions/6940669/how-can-i-move-the-position-of-an-image-thats-inline-with-some-text
- https://www.inmotionhosting.com/support/website/website-design/align-float-images-css/
- https://html.spec.whatwg.org/multipage/dom.html#flow-content-2
- https://developer.mozilla.org/en-US/docs/Web/CSS/float


