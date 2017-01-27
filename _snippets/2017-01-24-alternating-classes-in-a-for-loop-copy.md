---
title: "Alternate Classes in a For Loop"
layout: post
---
When using a for loop in Liquid, you may not want all of the content's
styling to be identical. For example, here is a layout that displays two
image with a text description to the right.

![alt text](/assets/img/cupcake_ipsum_2.png){:height="429.50px" width="915px"}

But what if we wanted to alternate the position of the image so that it
is rotates from left to right as we proceed to the next image.

The second image inside the div is positioned on the left similarly to the
first image above. The desired look is to have the second image positioned to
the right with the text to the left.

![alt text](/assets/img/cupcake_ipsum_1.png){:height="429.50px" width="915px"}

The classes Capture and Cycle inside of a for loop to can create the layout
above.

Capture stores the result of a block into a variable.
{% raw %}
~~~html
  {% capture text %}
    This is some text!
  {% endcapture %}
~~~
{% endraw %}

If we want to output the content in the variable text we can simply use:
{{ text }} which will display "This is some text!"
