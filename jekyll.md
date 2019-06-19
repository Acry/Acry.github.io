##Media
https://github.com/etianen/html5media/wiki/embedding-video

https://dev-notes.eu/2016/01/images-in-kramdown-jekyll/
![image-title-here](/path/to/image.jpg){:class="img-responsive"}
{:height="700px" width="400px"}

##Buttons
https://github.com/hashedin/jekyll-template/blob/master/_assets/libs/bootstrap-4.0.0-alpha.6/docs/components/buttons.md

https://stackoverflow.com/questions/40688633/how-can-i-add-a-button-in-a-md-file-with-jekyll

Option 1. Shortcode + javascript

The first is using shortcodes WordPress style and replacing them with jQuery. You will need some clever regex in javascript to achieve this. In that case your markdown can look like this:

Lorem ipsum dolor sit amet.

[button url="http://www.google.com"]
Option 2. Include Jekyll file

Another option is to use a Jekyll include:

Lorem ipsum dolor sit amet.

{% include button.html url="http://www.google.com" %}
Option 3. Plain HTML

The third option is to write plain HTML:

Lorem ipsum dolor sit amet.

<button name="button" onclick="http://www.google.com">Click me</button>
Option 4. The markdown way

The last option is to use markdown to add a class and use CSS to style the link as a button.

Lorem ipsum dolor sit amet.

[Option 4](http://www.google.com){: .btn}  

**Conclusion**

What you choose will depend on your preferences. The first solution is the simplest if you want to port from or to WordPress. The second one is the true Jekyll way. The third (HTML) just makes sense too. The last one, the markdown way, is the most beautiful (in my opinion), but does not generate a true button.