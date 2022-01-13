# Notes on: php, html, css, etc.

## Elements

- elements are designators that define the structure and content of objects within a page
- Elements are identified by the use of less-than and greater-than angle brackets surrounding the element name.

## Tags

- Tags are elements enclosed within 
- There must be an opening tag and a closing tag 
- Some tags are self-closing. They are called void-elements.

<p class="code-label">Tags</p>

```html
<Title>This is text within a title element</Title>

<!-- This is a comment, which is not visible on the page, but remains in the source code and visible from the developer tools within the browser. -->
<br/> <!-- these are self closing tags -->
<input/> <!-- these are self closing tags -->
<br/> <!-- these are self closing tags -->
<span> This is text within a span </span>
```

## Attributes

Attributes are properties used to provide additional info about an element.

<p class="code-label">Attributes</p>

```html
<div id="attribute-example"> </div>
```

## CSS

### Cascading Style Sheet

Style information can be embeded within the html, with properties applied to attributes on the elements themselves, or they can be within a separate .css file which is linked to in the .html document.

The link should be at the top of the html page, just before the title, as it will be read and applied first.

Css is broken down into three main terms
1. selectors, the way in which the element is referenced
2. properties
3. values

<p class="code-label">Inline styles</p>

```html
<div style="color:blue; text-align:center">This is a blue container</div>
```

<p class="code-label">seperate file link</p>

```html
     <!-- the link to the css file -->
    <link rel="stylesheet" href="styles.css">
    <title>Document</title>

    <p class="code-label">Inline styles</p>
    <div class="code-container">
        <code class="code-block">
            <!-- showcased code example goes here --> 
            <!-- this is how you can show example code instead of executing it -->
        </code>
    </div>
```

<p class="code-label">seperate css file</p>

```css
.code-label {
    display: inline-block;
    border-top-left-radius: 0.5rem;
    border-top-right-radius: 0.5rem;
    --bg-opacity: 1;
    background-color: #e1e7ef;
    background-color: rgba(224.70600000000002,231.07080000000002,239.394,var(--bg-opacity));
    padding: 0.25rem 0.75rem;
    border-top-width: 1px;
    border-left-width: 1px;
    border-right-width: 1px;
    --border-opacity: 1;
    border-color: #ccd6e0;
    border-color: rgba(204,213.85999999999999,224.39999999999998,var(--border-opacity));
    margin-bottom: 0;
    color: #141416;
}
.code-container {}
.code-block {
    background-color: black;
}
```

- css can also be injected as a block within a style element.
- The last element within the css block may override the prior rules.
- The inline styling, overrides the css file styling if there are conflicts.

<p class="code-label">Selectors, Properties and Values</p>

```html
<!-- in this example, "span", "text-thingy" and "container" are potential selectors -->
<style>
    .container { /* selector: classes are referenced with a preceding . */
        background-color:HoneyDew; /* property:value pair */
    }
    span { /* selector */
        font-size: 10px; /* property:value pair */
    }
    #text-thingy { /*selector: Id's are refferenced with a preceding # */
        font-size: 12px
    }    
</style>

<span id="text-thingy" class="container" style="color:green"> Text will be rendered from here </span>
<!-- "color:green" is a property:value pair -->
```

## PHP

- Php is an object oriented language for developing and rendering web pages
- Php is run on the server, not on the client
- Pages are rendered, then delivered to the client.

### Objects and Classes

- Object 
    - Objects have states and behaviors
    - Objects are instances of a class

- Class
    - Classes are templates that describe the behavior and states of an object of its type.


<style>
.code-label {
    display: inline-block;
    border-top-left-radius: 0.5rem;
    border-top-right-radius: 0.5rem;
    --bg-opacity: 1;
    background-color: #e1e7ef;
    background-color: rgba(224.70600000000002,231.07080000000002,239.394,var(--bg-opacity));
    padding: 0.25rem 0.75rem;
    border-top-width: 1px;
    border-left-width: 1px;
    border-right-width: 1px;
    --border-opacity: 1;
    border-color: #ccd6e0;
    border-color: rgba(204,213.85999999999999,224.39999999999998,var(--border-opacity));
    margin-bottom: 0;
    color: #141416;
}
</style>