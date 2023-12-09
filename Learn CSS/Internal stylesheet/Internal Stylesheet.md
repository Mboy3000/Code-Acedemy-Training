## Internal Stylesheet

As previously stated, inline styles are not the best way to style HTML elements. If you wanted to style, for example, multiple  <h1> elements. you would have to add inline styling to each element manually. In addition, you would also have to maintain the HTML code when additional h1 elements are added. 

Fortionately, HTML allows you to write CSS code in its own dedicated section with a style element nested inside of the head element. The CSS code inside the style element is often referred to as an internal stylesheet. 

An internal stylesheet has certain benefits and use cases over inlines styles , but once again, it's not best practice. 

Understanding how to use internal stylesheets is nonetheless helpful knowledge to have. 

To create an internal stylesheet, a style element must be placed inside of the head element. 


After adding opening and closing style tags in the head section you can begin to write CSS code. 

The CSS code in the example above changes the color of all paragraph text to red and also changes the sizw of the text to 20 pixels. not how the syntax of the CSS code matches ( for the most part ) the syntax you used  for inline styling. The main difference is that you can specify which elements aplly the styling. 