HyperText Markup Language (HTML) provides the foundational content structure that all web applications build on.
<p>style (CSS)</p>
make pages interactive (JavaScript)

## HTML
HTML elements are represented with enclosing tags that may enclose other elements or text.
> \<p>Hello world\</p>
- The html element represents the top level page structure. 
- The head element contains metadata about the page and the page title. 
- The body element represents the content structure. The main element represents the main content structure
> \<html><br>
   &emsp;\<head><br>
    &emsp;&emsp;<title>My First Page</title><br>
  &emsp;\</head><br>
  &emsp;\<body><br>
    &emsp;&emsp;\<main><br>
      &emsp;&emsp;&emsp;\<p>Hello world\</p><br>
    &emsp;&emsp;\</main><br>
  &emsp;\</body><br>
\</html>

## CSS
There are three ways that you can associate CSS with HTML.
- The first way is to use the style attribute of an HTML element and explicitly assign one or more declarations.
- The next way to associate CSS is to use the HTML style element to define CSS rules within the HTML document. The style element should appear in the head element of the document so that the rules apply to all elements of the document.
- The final way to associate CSS is to use the HTML link element to create a hyperlink reference to an external file containing CSS rules. The link element must appear in the head element of the document.
