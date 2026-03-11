

#Concepts on the properties for the flex container and flex items
https://codepen.io/enxaneta/pen/adLPwv 



#Flex:1 Declaration
Not exactly — but flex: 1 includes flex-grow: 1.

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

The important difference is:

Property	flex:1	flex-grow:1
flex-grow	1	1
flex-shrink	1	1
flex-basis	0%	auto
Why flex:1 is commonly used for sticky footers

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

If you only used:

flex-grow:1;

the layout might not stretch the same way because flex-basis remains auto.

✅ Best practice for page layouts (like your site):

main {
  flex:1;
}

If you want, I can also show you a cleaner modern layout pattern for headers + sticky footer + responsive sections that professors often like to see in web design assignments.


https://www.w3schools.com/css/tryit.asp?filename=trycss_display2
