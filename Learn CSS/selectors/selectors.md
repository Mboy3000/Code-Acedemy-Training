# type
Remeber that declarations are a fundamental part of CSS because they apply a style to a selected element. But how do you decide which elements will get the style? with a selector. 

A selector is used to target the specific HTML elements to be styled by the declartion. One selector you may already be familiar with is the type selector. Just like the name suggests, the type selector matches the type of the element in the HTML document. 

## Some important notes on the type selector. 
The type selector does not include the angle brackets. 
since element types are often referred to by their opening tag name, the type selector is sometimes referred to as the tag name or element selector. 

# Universal
The universal slector selects all elements of any type. 
Targeting all of the elements on the page has a few specific use cases, such as resetting default browser styling, or selecting all children of a parent element. 

The universal selector uses the * character in the same place where you specified the type selector in a ruleset. 

# Class
CSS is not limited to selecting elements by their type. As you know, HTML elements can also have attributes. When working with HTML and CSS a class attribute is one of the most common ways to select an element. 

To select a HTML element by its class using CSS, a period must be prepended (come before ) to the class's name.

# Multiple Classes
We can use CSS to select an HTML element's class attribute by name. And so far, we;ve selected elements using only one class name per element. If every HTML element had a single class, all the style information for each element would require a new class. 
Luckily, it's possible to add more than one class name to an HTML element's class attribute. 

For instance , perhaps there's a heading element that needs to be green and bold. You could write two CSS rulesets. 

We can add multiple classes to an HTML element's class attribute by separating them with a space. This enables us to mix and match CSS classes to create many unique styles without writting cusotm code. 

# ID selectors
Oftentimes it's important to select a single element with CSS to give it its own unique style. If an HTML element needs to be styled uniquely, we can give it and ID using the id attribute. 
In contrast to class which accepts multiple  values , and can be used broadly throught an HTML document, an element's id can only have a single value, and only be used once per page. 
To select an element's ID with CSS, we prepend the id name with a number sign. 

# Attribute
You may remember that some HTML elements use attributes to add extra detail or functionality to the element. Some familiar attributes may be href and src but there are many more including class and id

The attribute selector can be used to target HTML elements that already contain atttributes .
Elements of the same type can be targeted differently by their attribute or attribute value. 
this alleviates the need to add new code, like the class or id attributes. 
attributes can be selected similarly to types, clases, and IDs

The most basic syntax is an attribute surrounded by square brackets. like so  [] this would target all elements that have the attribute inside the bracket. 

# pseudo-class
You may have observed how the appearance of certain elements can change, or be in a different state, after certain user interactions.For instance:
** When you click on an input element, and the blue border is added showing that it is in focus

** When you click on a blue a link to visit another page, but when you return to a page the text is purple. 

** When you're filling out a form and the submit button is grayed out and disabled. Buy when all the fields have been filled out, the button has color show that it's active. 

These are all examples of pseudo- class selectors in action! in fact, :focus, : visitied, : disabled, and : active are all pseudo- class. 

A pseudo- class can be attached to any selector. It is always writeen as a colon: followed by a name. For example 
p:hover. {

}

# Classes and ID's 

CSS can select HTML elements by their type, class, and ID. CSS classses and IDs have different purposes, which can affecct which one you use to style HTML elements. 

CSS classes are meant to be reused over many elements. By writing CSS classes, you can style elements in a variety of ways by mixing classes. For instance, imagine a page with two headlines. One headline needs to be bold and blue and the other needs to be green. Instead of writing separate CSS rules for each headline that repeat each other's code, it's better to write a .bold CSS rule, a .green CSS rule, and a .blue CSS rule. Then give one headline the bold green classes and the other bold blue classes. 

While classes are meant to be used many times,an ID is meant to style only one element. As you'll learn in the next exercise, IDs override The styles of types and classes.  Since IDs override these styles, they should be used sparingly and only on  elements that need to always need to appear the same. 


# Specificity
Specificity is the order by which the browser decides which CSS styles will be displayed. A best practice in CSS is to style elements while uding the lowest degree of of specificity so that if a element needs a new style, it is easy to override. 

IDs are the most specific selector in CSS, followed by classes, and finally type. 

Over time as a file grouwsmany elements may have IDs which can make CSS difficult to edit since a new, more specific style must be created to change the style of an element. 

To make styles easy to edit , it's best to style with a type selector, if possible. If not, add a class selector. It that is not specific enough, then consider using an ID selector. 
