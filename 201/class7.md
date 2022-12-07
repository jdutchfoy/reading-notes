# README.MD

## Read Assignment 7

1.The main reason for using DOM is to create or modify an XML document programmatically. You can use DOM just to read an XML document, but as you will see in the next chapter, SAX is often a better candidate for the read-only case. If you want to create a document, you start by creating a root element and then add attributes, content, sub-ele-ments, and so on. Once you are finished, you can write the document out to disk or send it over a network. The output looks just like an XML document prepared in a text editor or XML tool.

Learning to use DOM saves you considerable time by leveraging existing parsers. Additionally, a standard interface makes it easy to change parsers in the event that an improved implementation becomes available.


2.In short, using tables for layout rather than CSS layout techniques is a bad idea. The main reasons are as follows:
Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.

Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.

Tables are not automatically responsive: When you use proper layout containers (such as <header>, <section>, <article>, or <div>), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.

3.HTML was originally created as a markup language to describe documents on the early internet. As the internet grew and was adopted by more people, its needs changed.
<article>
<aside>
<details>
It is much easier to read, greater accessibility,Overall, semantic elements also lead to more consistent code. 
This works fine but is a bit long-winded: we have to create an empty object, initialize it, and return it. A better way is to use a constructor. A constructor is just a function called using the new keyword. When you call a constructor, it will:
create a new object
bind this to the new object, so you can refer to this in your constructor code
run the code in the constructor
return the new object.
Constructors, by convention, start with a capital letter and are named for the type of object they create. 

4.You are probably wondering what "this" is. The this keyword refers to the current object the code is being written inside — so in this case this is equivalent to person. So why not just write person instead?
Well, when you only have to create a single object literal, it's not so useful. But if you create more than one, this enables you to use the same method definition for every object you create.

5.Regardless of whichever pattern you used to create an object, getting that object's prototype can be accomplished using the Object.getPrototypeOf method. *Fingerprint

## Things I want to know more 

Inheritance
