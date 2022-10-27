# Testing 
In this section, I will be testing my site. 

---

## Code validation
First thing I did when testing my code was to run it through code validators (html and css respectively. 
### HTML code
- Multiple errors found on initial pass through the official W3C validator
- 1 error remains for booking.html, method attribute of form is blank.
Since I am not sending the booking form data anywhere for this project, I thought it would be okay to leave the method attribute blank for the form. post or get? one of these
### CSS code
- 2 errors regarding a media query appeared upon the initial validation check through the official Jigsaw CSS Validator
- removed media query and now have 0 errors.

--- 

## User Stories and Testing
### User Story 1 - User would like to learn key information about the theatre
- This can be achieved easily as the homepage shows all key information about the theatre. 
- Phone number is highlighted to draw the users eye
- Location information is aided by a Google maps iframe which allows the user to stay on the site without needing to go search the address in another browser tab.
#### Test of User Story 1
Expectation: All key information is available on the homepage
Testing: Navigate to the home page and look for information
Result: Found theatre key information
Fix: none required
### User Story 2 - User would like to know What is Currently showing? Which film should the user watch?
- This can be achieved by clicking the 'Current showings' tab on the navigation bar. This is available on every page so the journey to the page is simple. 
- Candidate can view movie posters, descriptions and reviews
#### Test of User Story
Expectation: To view the current showings at the theatre
Testing: Navigate to the current showings page
Result: All current showings information is available
Fix: none required
### User Story 3 - User would like to Navigate the site easily.
- This can be achieved by using the navigation bar, which is present on every page and runs the full width of the site. 
- The background of the navigation links change color when hovered over, to allow the user to see what they are selecting
Please see the screenshot below displaying this information.
#### Test of User Story
Expectation: Internal links work correctly, easy to get from one page to the next
Testing: Click on all internal links, can each page be reached?
Result: All internal links work, all 3 main pages accessible.
Fix: none required.
### User Story 4 - User would like to book tickets easily.
- This is achievable because the booking form is available as soon as you click onto the site, and as part of the navigation bar it is available across ALL pages.
- The single page booking form allows for a simple booking experience, with one submit button ensuring users will not have time to abandon purchase.
#### Test of User Story
Expectation: Booking form is easy and quick to use, easy to find, booking form submits when 'book now' button is pressed
Testing: fill out the form, submit. navigate to and from the book now page.
Result: Form initially did not work with my 'thankyou.html' page. Navigation links to and from the form work perfectly.
Fix: So instead I have replaced it with the codeinstitute provided form submission page. The form therefore submits. 
### User Story 5 - User would like to use the site on their mobile phone
- This is achievable because I have used the bootstrap column system. This system allows easily applied responsiveness. 
- All elements of the site are available on the desktop, tablet AND mobile viewpoints.
- When the site goes to fit the smallest screen-size, the information present on the sight moves into a single column for ease of use on smaller screens.
#### Test of User Story
Expectation: A fully responsive site, site adapts to different screen sizes and content is not squished or images are not deformed. 
Testing: use devtools to view and test all elements of the site within the altered parameters. Test at tablet and mobile level. 
Result: Site is completely responsive. No issues with responsiveness. Site looks good at all sizes.
Fix: none required.

---

## Links Testing
Expected: Associated link takes you to the associated page
Testing: Click on the links
Result: Arrived at the correct page
Fix: none required
- 'Home' navigation bar link: tested, no anomalies 
- 'Current showings' navigation bar link: tested, no anomalies 
- 'Book Now' navigation bar link: tested, no anomalies 
- Social Media icon links: tested, no anomalies 
- iframe link: tested, no anomalies
- 'Book Now' button, form submit link: tested, no anomalies

--- 

## Bugs
Whilst developing this project, I have come across 3 major bugs. 

1) The first was that the styles.css file was having no effect on the project. Initially I thought this was because of the bootstrap code I was using but it was a much much simpler fix! I had not linked the css file correctly. It was set to href="styles.css" but shouldve been href="css/styles.css".

2) The Second was that the navbar was not stretching all way across screen! After a lot of blank staring, I finally thought to compare my code with the other html files (as their nav bars were stretched fine). I then realised there was a div with class container-fluid present around the header content. Once this was removed the navbar went back to being stretched all across.

3) The Third was that all the radio buttons on the booking.html form would coincide so you couldnt pick a date and time, only a date OR time. I managed to change around the bootstrap applied IDs and this allowed the radio buttons to be separated and therefore choose date and time. 



