# Wedding Photographer Website

by Scott Edwards

[Click here to view the live website.](https://scotte13.github.io/Photographer-Website/)

Website developed for educational purposes as part of the Code Institute diploma in web development.

- - -

# Project Goals

## Purpose

The idea for this website was advertisement for a self-employed businessperson. This was a fictional career for the purpsoes of the project. The career chosen was a Wedding Photographer. The name of the photographer, 'Rhys Morgan', is made up. 

## Client Aims

The client aim is to ultimatley to obtain business. The website is a form of advertisement. It needs to provide information on the photography serivce, display a portoflio of work and provide methods of contact for potenntial customers. 

## User Aims

Users are the site are envisioned to be primarily people who are searching for a photographer for themselves or someone else. In addition friends, fans, clients and photography fans may view the site. 

## User Stories

1) As someone searching for a photogrpaher to hire I want to:

- Obtain an overview of the photographer and their service.
- View examples of the photographers work.
- Read reviews of the photographer.
- Be able to contact the photographer for more information, to ask questions or to request a booking. 
- Find links to social media accounts to connect with the photographer.

2) As a friend, fan or previous client I want to:

- View examples of the photographers work.
- Find links to social media accounts to connect with the photographer.
- View the testimonial if I have written one for the photographer. 

3) As a photography fan I want to:

- Obtain an overview of the photographer and their work.
- View examples of the photographers work.
- Be able to contact the photographer to discuss their work.
- Find links to social media accounts to connect with the photographer.

## Project Scope

The Scope of this project is to deliver a basic website that meets the client and user goals outlined above only. Additional functionality, content or features could be added in the future but will not be part of this release. In order to stay within this scope the basic site structure was planed in advance to outline the key pages required to meet the outlined goals. 

- - -

# Design & Structure

## Project Structure

The basic structure of the website was planned to include the following pages.

- Home page providing a photo of the photographer and basic about information.
- Portfolio page to display examples of work. 
- Testimonials page to display reviews from prior customers.
- Contact page to allow people to request business and ask any questions they may have. 

One additional page was added during development which was a thank you page following form submission. 

## Wireframes

Simple wireframes for the website pages were drawn up using [wireframe.cc](https://wireframe.cc/)

<details><summary>Home</summary>
<img src="assets/images/readme/wireframe-index.jpg">
</details>

<details><summary>Portfolio</summary>
<img src="assets/images/readme/wireframe-portfolio.jpg">
</details>

<details><summary>Testimonials</summary>
<img src="assets/images/readme/wireframe-testimonials.jpg">
</details>

<details><summary>Contact</summary>
<img src="assets/images/readme/wireframe-contact.jpg">
</details>

<br>

- - -

# Technologies Used

- HMTL
- CSS
- Git
- Git Hub
- Git Pod
- Bootstrap 5.3
- Google Fonts
- Font Awesome

- - -

# Testing

- All HTML pages were ran through the W3C Validator.
- The validator picked up duplicated body tags. These were removed.
- The validator returned that an "a" element should not be a descendant of a "button" element. I had tested the functionality of these buttons myself and the links were working. To fix this issue I removed the button elements completley and instead applied styling to the links themselves.
- The validator picked up an unclosed semantic tag (nav) in the footer section across all pages. This was corrected.
- Unneccesary "/" characters were removed from input elements in the contact.html page. 
- No other HTML errors were detected.
- CSS style sheet test using W3C Validator found no errors.
- I conducted a manual test of all links and found no errors.
- I viewed the live site on mobile and desktop to check for any responsiveness issues.

- - -

# Bugs 

During development I came across the following key bugs:

- BUG: The footer was not sitting at the bottom of the viewport on larger devices, leaving empty space below.
- FIX: I researcehed this issue online and found a solution using flexbox. This is credited in the style.css sheet. 

- BUG: White space was present on either side of my navigation bar. 
- FIX: I used chrome developer tools to inspect the problem. Padding was being inhertied from bootstrap classes. I initially fixed this by overwriting it with a class of my own, however I later read through the bootstrap documentation in more detail and realised the error. I had used an unneccessary container, and bootstrap have their own 'g-0' class which can be applied. I amended my code with these solutions as it was more efficient. 

- BUG: Too much white space was visible between bootstrap column content on lower screen sizes, for example images on the portfolio page. 
- FIX: I realised this was because I had added margins to the columns initially to push them down from the header. As these margins were applied to the columns themself, when they stacked on top of eachother on smaller screen sizes they impacted eachother. I fixed this issue by removing the margins from the columns and instead targetting the rows I wanted with a new class.

- BUG: The photographer images on my home page was pushing the whole screen down on larger devices.
- FIX: I fixed this by adding a max-height to limit this slightly. This was only a small change and did not visibly distort the image, but had the affect of ensuring the whole page was visible on larger screens without having to scroll. 

- BUG: Following deployment my image on the home page was not loading on the live page.
- FIX: I realised the address was wrong and needed to delete a "/" from the begging of the scr address.

- BUG: The testimonials page seemed to lack responsiveness compared to the other pages.
- FIX: The content container was missing it's bootstrap 'container-fluid' class. 

- - -

# Credits

- Header backround image was sourced from https://www.freepik.com/. Image by user15285612 on Freepik
- All other images used in this project were sourced from https://unsplash.com/
- Social media icons were sourced from https://fontawesome.com/
- Fonts used were from https://fonts.google.com/
- Bootstrap was used extensivley for responsiveness styling. https://getbootstrap.com/

- - -

# Deployment

This site was deployed using GitHub pages by taking the following steps:

- From the GitHub repository, go to the settings tab. 
- Select pages from the menu.
- Select the main branch.
- Save

Once completed the url will generate. 

The live URL is: https://scotte13.github.io/Photographer-Website/

To clone the repository for your own use you can take the following steps:

-From the GitHub repository select the code drop down button.
- Select HTTPS
- Copy the repository link
- Open your own integrated development environment. 
- enter the git clone command and then paste the copied URL
-"git clone url"