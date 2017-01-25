---
title: "Alternate Classes in a For Loop"
layout: post
---
There may come a situation where you need to display content that has similar
components so you decide to use a for loop but you need to use different
classes.

Here is an example of displaying a list of posts with their corresponding
images.

Insert images here.

The issue here is that the content is identical and is not the look we are
attempting to achieve. How about instead of having the second image below on
the left, we move it to the right leaving the text to float left.

Insert images here.

We will be using the classes Capture and Cycle inside of a for loop to
create the layout above.

Capture stores the result of block into a variable.
{% raw %}
~~~html
  {% capture text %}
    This is some text!
  {% endcapture %}
~~~
{% endraw %}

If we want to output the content in the variable text we can simply use:
{{ text }} which will display "This is some text!"
