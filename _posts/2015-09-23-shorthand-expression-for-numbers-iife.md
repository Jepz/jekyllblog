---
layout: post
title:  "Shorthand expression for numbers (IIFE)"
date:   2015-09-23 17:00
categories: quickpost
---
I just came across to check if a variable is a number without using Number(). It's the shorthand way to make sure that variables in a function are Numbers and not a string is to add an expression to it. 
 Exampel:
{% highlight ruby %}
 +value <= numb && +value[+i + 1] > numb)
{% endhighlight %}

"+" before a variable will ensure it is a Number instead of a String. So basically...
{% highlight ruby %}
+"1" -> 1 
+"Hello" -> NaN
{% endhighlight %}
A string that is a number will den be 1, but if its not it will be NaN. This could also crash you application so good practice is to check if the +value = true then to fucntion.

[Ben Alman](http://benalman.com/news/2010/11/immediately-invoked-function-expression/ "Ben Alman - Immediately-Invoked Function Expression (IIFE)") deep dives into the topic so read his take on it. Also check out [Stackoverflow - JavaScript plus sign in front of function name](http://stackoverflow.com/questions/13341698/javascript-plus-sign-in-front-of-function-name "Stackoverflow - JavaScript plus sign in front of function name"), it helped me out.





