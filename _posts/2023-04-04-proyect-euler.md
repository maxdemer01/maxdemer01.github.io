---
layout: post
title: Project Euler
subtitle: A web page to improve your mathematical problem solving using programming.
tags: [maths,programming]
thumbnail-img: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/Leonhard_Euler_2.jpg/200px-Leonhard_Euler_2.jpg"
comments: true
---

Today I am going to talk about [Project Euler](https://projecteuler.net), a website where we will find hundreds of mathematical problems of varying difficulty that we will have to solve by designing algorithms and programs in our favorite programming language. 

According to the official Project Euler (or PE) website, the problems we will encounter will require logic and knowledge of computers and programming to be solved, rather than mathematical knowledge. However, it will lead to more precise and elegant answers.

{: .box-note}
*"Project Euler exists to encourage, challenge, and develop the skills and enjoyment of anyone with an interest in the fascinating world of mathematics."*

With over a million users who have solved at least one problem, PE is aimed at anyone who wants to maintain and improve their problem solving skills.

Any reader of this blog should, at a variable rate, be able to solve all the problems, as each problem uncovers a concept needed to solve subsequent problems.






This is a demo post to show you how to write blog posts with markdown.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/headings/tables/etc.

**Here is some bold text**

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


How about a yummy crepe?

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

It can also be centered!
h
![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.