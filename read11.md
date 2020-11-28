# EJS 

### What is EJS?
_What is the "E" for? "Embedded?" Could be. How about "Effective," "Elegant," or just "Easy"? EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript._

![html](https://www.tutomena.com/static/9057d03a46e7cb23b1bc026fcd30db21/9522a/ejs-templating.jpg)


 ### Docs

 **Example**
 ```
 <% if (user) { %>
  <h2><%= user.name %></h2>
 <% } %>
```

### Usage

```
let template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
}); 

``` 
![ejs](https://miro.medium.com/max/3144/1*gnkTUgkWeTgvRX12sv8F1A.png)

### Tags

**<%** 'Scriptlet' tag, for control-flow, no output
**<%_** ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
**<%=** Outputs the value into the template (HTML escaped)
**<%-** Outputs the unescaped value into the template
**<%#** Comment tag, no execution, no output
**<%%** Outputs a literal '<%'
**%>** Plain ending tag
**-%>** Trim-mode ('newline slurp') tag, trims following newline
**_%>** ‘Whitespace Slurping’ ending tag, removes all whitespace after 

 ### Includes

_Includes are relative to the template with the include call. (This requires the 'filename' option.) For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use <%- include('user/show'); %>._

You'll likely want to use the raw output tag (<%-) with your include to avoid double-escaping the HTML output.

```
<ul>
  <% users.forEach(function(user){ %>
    <%- include('user/show', {user: user}); %>
  <% }); %>
</ul>
```

