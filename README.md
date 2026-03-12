# Event Center Website – The Breakers


![Homepage Screenshot](/AssignmentEventCenter/img/websitePreview.png)


## Project Description
This project is a multi-page website for an event center called **The Breakers**. It showcases wedding event spaces, allows users to check availability, and provides a contact form for booking inquiries.


## Features
- Fixed navigation bar
- Event showcase cards with images
- Event availability calendar
- Contact & booking inquiry form
- Responsive layout for mobile and tablet
- Hover animations and interactive UI elements

## Technologies Used

- HTML5
- CSS3
- Google Fonts (Poppins, Playfair Display)

## How to Run the Project

1. Download or clone the repository.
2. Ensure all files remain in the same folder structure.
3. Open **index.html** in a web browser.

## Educational Materials 

### Concepts on the properties for the flex container and flex items: 
https://codepen.io/enxaneta/pen/adLPwv 


### Flex:1; Declaration
```
In Flexbox, flex is a shorthand property that sets three properties at once:

flex: <flex-grow> <flex-shrink> <flex-basis>
When you write
flex: 1;

It actually means:

flex-grow: 1;
flex-shrink: 1;
flex-basis: 0%;

So the element:

grows to fill available space (flex-grow:1)
can shrink if needed (flex-shrink:1)
starts with a base size of 0 (flex-basis:0%)

When you write
flex-grow: 1;

You are only allowing the element to grow, but the other properties stay at their defaults:

flex-grow: 1
flex-shrink: 1
flex-basis: auto

In your layout:

body {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex: 1;
}

main expands to fill all remaining space, pushing the footer to the bottom of the page when content is short.
```
### Display: Grid; Declaration
https://www.w3schools.com/css/tryit.asp?filename=trycss_display2
