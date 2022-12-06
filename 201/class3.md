# README.md 

## Read Assignment 3 Notes

Read Assignment 3

1.The <ul> element is for grouping a collection of items that do not have a numerical ordering, and their order in the list is meaningless. Typically, unordered-list items are displayed with a bullet, which can be of several forms, like a dot, a circle, or a square. The bullet style is not defined in the HTML description of the page, but in its associated CSS, using the list-style-type property.The <ul> and <ol> elements may be nested as deeply as desired. Moreover, the nested lists may alternate between <ol> and <ul> without restriction.The <ol> and <ul> elements both represent a list of items. They differ in that, with the <ol> element, the order is meaningful. To determine which one to use, try changing the order of the list items; if the meaning is changed, the <ol> element should be used, otherwise you can use <ul>.

2.CSS list-style-type 

3.The <ol> and <ul> elements both represent a list of items. They differ in that, with the <ol> element, the order is meaningful. To determine which one to use, try changing the order of the list items; if the meaning is changed, the <ol> element should be used, otherwise you can use <ul>.

4.The CSS for styling lists is here, but is basically:
li {
    list-style-type: decimal;
    list-style-position: inside;
}
                OR
However, the specific layout you're after can probably only be achieved by delving into the innards of the layout with something like this (note that I haven't actually tried it):
ol { counter-reset: item }
li { display: block }
li:before { content: counter(item) ") "; counter-increment

5.In the standard box model, if you give a box an inline-size and a block-size (or width and a height) attributes, this defines the inline-size and block-size (width and height in horizontal languages) of the content box. Any padding and border is then added to those dimensions to get the total size taken up by the box (see image below).
element_name{
height:<value>;
width:<value>;
border:<value>;
padding: <value>;
margin:<value>;

6Content: This is the main content of the element. It can be text, links, images, videos or any other content.Padding: This is the gap between the content and the border (which is another element) of the content.Border: This can be visualized as a solid boundary of the content of the element.Margin: This is the space that is maintained between various boxes on a particular page i.e. the space between two borders.


7. String, Integer, Double, Boolean

8.NO

9. Assignment operators
An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

Assignments	Shorthand	Meaning

Addition 	   a+=b		a=a+b

Subtraction	    a-=b		 a=a-b

Multiplication       a*=b		 a=a*b

Division	    a/=b		 a=a/b

Remainder	   a%=b	a=a%b

10. Loops offer a quick and easy way to do something repeatedly in javascript

## Things I need to know

I dont understand how to operate loops, I ma not strong with arrays
