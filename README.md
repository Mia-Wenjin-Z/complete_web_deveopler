# Complete-Web-Developer-Manual

All resources and notes from the Complete Web Developer in 2018: Zero to Mastery course

## 1.	__Introduction__

![roadmap](https://udemy-images.s3.amazonaws.com/redactor/raw/2019-03-08_11-40-49-4f1a261d70c1fa39427df0ba41b85a81.jpg)

## 2.	__How The Internet Works__

## 3.	__History Of The Web__

![full-stack-framework-new](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190303094556925.png)

## 4. __HTML 5__

### Bacis Tags

<!DOCTYPE html>
<html>
    <head>
        <title>This is the web page title</title>
    </head>
    <body>
        <a href="https://www.google.com"><h1>Go to Google</h1></a>
        This is the body
        This is the body
        <p>This is a paragraph</p>
        <p>This is a paragraph</p>
        <h1>This is the 1st title</h1>
        <h6>This is the 6th title</h6>
        <p><strong>This is the strong, evolving from bold</strong></p>
        <em><p>This is the emphasis, evolving from italicized</p></em>
        <ul>This is an unordered list
            <li>apple</li>
            <ol>This is a nested ordered list
                <li>Shandong Big Apple</li>
                <!alt is for screen readers>
                <img src = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTGIdjYe17cbMptGm_087hNFMs0oQDlbvCiZ607rscrYI2WMzXz" alt = “Shandong_Big_Apples” width = “60” height="60">
                <li>Royal Gala that you can't afford</li>
            </ol>
            <li>banana with break</li><br> <!--br is for break, this is a self-closing tag-->
            <li>peach with horizontal line</li><hr><!--hr is for horiozontal line, this is also a self-closing tag-->
        </ul>
        </body>
    </html>

### Reference

Install  a text editor (Select one):

*	[sublime](https://www.sublimetext.com/) 
*	[VS](https://code.visualstudio.com/)
*	Atomic

Reference websites:
*	[MDN](https://developer.mozilla.org/en-US/)

## 5.	Advanced HTML 5

### Write a Form

<!DOCTYPE html>
<html>
<head>
    <title>register</title>
</head>
<body>
    <form method = "GET">
        Firstname:<input required type = "text" name ="firstname" required><br>
        Lastname: <input type="text" name = "lastname" required><br>
        Birthday: <input type="date" name ="bod" min="1900-01-01" max="2019-01-01" required><br>
        <!-- In unsupported browsers, the control degrades gracefully to a simple <input type="text"-->
        Email: <input type="email" name="email" required><br>
        Password: <input type="password" name="password" min = "5"required><br>
        Gender:<br>
        <!--you need to add name and value for each input, sharing the same name(such as Gender) means only one value can be selected-->
        <input type="radio" name="Gender" value = "Male">Male<br>
        <input type="radio" name="Gender" value = "Female">Female<br>
        <input type="radio" name="Gender" value = "Other">Other<br>
        Pets:<br>
        <input type="checkbox" name="Puppy">Puppy<br>
        <input type="checkbox" name="Kitten">Kitten<br>
        <input type="checkbox" name="Rubber_duck">Rubber Duck<br>
        <input type="checkbox" name="Hyper_Rubber_duck">Hyper Rubber Duck<br>
        Cars:<br>
        <SELECT name="Car">
            <OPTION value ="Volvo" >volv0</OPTION>
            <OPTION value ="Maserati" >maserati</OPTION>
        </SELECT><br>
        <input type="submit" value="Register">
        <input type="reset">
    </form>
</body>
</html>



### Submit a Form

It's one way for us, to send our information to the backend or the servers

This was automatically generated in HTML5, with a form. But **form** was using an attribute called

**"GET"** and this "GET" will attach the form information to the URL and send it to the server.

```
file:///Users/miawenjinzhang/CS_basics/Web_application/register.html
?firstname=Mia
&lastname=Z
&bod=1996-01-07
&email=mia%40gmail.com
&password=1234
&Gender=Female
&Rubber_duck=on
&Hyper_Rubber_duck=on
&Car=Maserati
```

### Extras

* Form in html 
* 非常重要的两个tag, 利于CSS
  * `<div>` 用于页面分区
  * `<span>` in-line division
* html vs html5
  * 最主要的变化是加了new semantics（比如 header），有利于SEO爬页面的时候获取更多信息



## 6.	__CSS__

### Basic CSS

CSS = **Cascading** style sheets

* <u>Cascading意味着后定义的style会覆盖前面的style</u>

Ways to add CSS files

* use `link` in section `title`
* use `style` in section `title`
* add `style` in the section directly

<!DOCTYPE html>
<html>
<head>
	<title>My first website!</title>
	<!-- this is the first method to add CSS: use link in section title-->
	<link rel="stylesheet" type="text/css" href="style.css">
	<!-- this is the second method to add CSS: use style in section title -->
	<style type="text/css">
		h1{
			background-color: pink;
		}
	</style>
</head>
<body>
	<!-- this is the third method to add CSS: add in the section directly -->
	<header style="background-color: pink ; color: blue">
		<nav>
			<ul>
				<li><a href="index.html">Home</a></li>
				<li><a href="about.html">About</a></li>
				<li>Login</li>
			</ul>
		</nav>
	</header>
	<section>
		<h5>Login</h5>
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
		quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
		cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
		proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
	</section>
</body>
</html>

### `Div` and `Span`

[read this link](https://www.1keydata.com/css-tutorial/div-span.php)

### Add Color

![AddColor](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190306121419147.png)

### CSS Selection cheatsheet

[CSS Selector Reference](https://www.w3schools.com/cssref/css_selectors.asp)

Cascading Style Sheets at the most basic level it indicates that the order of CSS rules matter. 

* `.class`： 用于选取一组元素赋予他们同样的style
* `#id` : 和class类似，和`<div>`一起使用，但是只能使用一次（id不能重复）`<div id = "#idnum">`

* `*` : 表示所有元素

* | Selector          | Example    | Example description                                          |
  | ----------------- | ---------- | ------------------------------------------------------------ |
  | `.class`          | .intro     | Selects **all elements with class**="intro"                  |
  | `#id`             | #firstname | Selects **the element with id**="firstname"                  |
  | `*`               | *          | Selects **all elements**                                     |
  | `element`         | p          | Selects all <p> elements                                     |
  | element,element   | div, p     | Selects all <div> elements **and** all <p> elements          |
  | element element   | div p      | Selects all <p> elements **inside** <div> elements           |
  | element>element   | div > p    | Selects all <p> elements where the **<u>direct parent</u>** is a <div> element |
  | element+element   | div + p    | Selects all <p> elements that are **<u>placed immediately after</u>** <div> elements |
  | element1~element2 | p ~ ul     | Selects every <ul> element that are <u>**preceded by**</u> a <p> element |

  `:hover` 鼠标移动到该区域后应用

* `:last-child` 同class中的最后一个
  `:first-child` 同classs中的第一个
* `!important `(not recommended) Overrides all other styles

###  Cascade depends on:

[Cascade_and_inheritance](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Cascade_and_inheritance)

* Specificity [specificity calculator](https://specificity.keegan.st/)
  * `element` < `Class` <`ID`<`in-line selector `<`!important`.
  * **Thousands**: Score one in this column if the declaration is inside a `style` attribute, aka <u>*inline styles*</u>. Such declarations don't have selectors, so their specificity is always simply 1000.
  * **Hundreds**: Score one in this column for each <u>*ID selector*</u> contained inside the overall selector.
  * **Tens**: Score one in this column for each <u>*class selector, attribute selector, or pseudo-class*</u> contained inside the overall selector.
  * **Ones**: Score one in this column for <u>*each element selector or pseudo-element*</u> contained inside the overall selector.
* Importance
* Source Code Order

### Box Model

- **Content** - The content of the box, where text and images appear
- **Padding** - Clears an area around the content. The padding is transparent
- **Border** - A border that goes around the padding and content
- **Margin** - Clears an area outside the border. The margin is transparent

`div {
  width: 300px;
  border: 25px solid green;
  padding: 25px;
  margin: 25px;
}`

### Em & Rem

和`span`一起用

* Xem ： 将值设为element对应值的X倍
* Xrem：将值设为root element对应值的X倍

### Reference 

* websites:
  * https://css-tricks.com/
  * https://www.supremo.co.uk/typeterms/
  * https://css-tricks.com/snippets/css/a-guide-to-flexbox/
  * https://waitbutwhy.com/
  * https://unsplash.com/
  * https://developer.mozilla.org/es/docs/Learn/CSS/Introduction_to_CSS/Cascada_y_herencia
  * https://specificity.keegan.st/

* website for color check:
  * http://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF
  * https://coolors.co/

* website for fonts download:
  * https://fonts.google.com/

## 7.	__Advanced CSS__ - TBC

### Efficiency of your page

CSS， Font等东西都需要加载，会减缓page render的速度。

有一个专门mininize CSS 和Javascript语句的网站。[MinifyCSS](https://www.cleancss.com/css-minify/)

### FlexBox

是一种flexible的container，课上的例子是一个显示image的网页，并给了一个装Robot的练习

核心思想是不同的区块`<div>` 到不同的class中

**<u>在父类中定义`  display: flex;`，则各个子类按照`flex`的方式排列。</u>**

[flexbox tutorial](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

[flexbox cheatsheet](https://darekkay.com/dev/flexbox-cheatsheet.html)

[flexboxfroggy](http://flexboxfroggy.com/)

### 检查不同浏览器的支持情况

*  [CSS Browser Support Reference](https://www.w3schools.com/cssref/css3_browsersupport.asp)
* [Can I use](https://caniuse.com/)
* **加不加前缀** [ShouldIPrefix](http://shouldiprefix.com/)

### Responsive UI



## 8.	__Bootstrap 4, Templates, And Building Your Startup Landing Page__

### Basics

是一个提供了很多模板的网站。

使用CDN，可以在文件`<head>`里add link bootstrap，在`<body>`里add javascript

直接copy所需源码到html的`<body>`即可。

### CDN

CDN主要功能是在不同的地点缓存内容，通过负载均衡技术，将用户的请求定向到最合适的缓存服务器上去获取内容，比如说，是北京的用户，我们让他访问北京的节点，深圳的用户，我们让他访问深圳的节点。通过就近访问，加速用户对网站的访问。解决Internet网络拥堵状况，提高用户访问网络的响应速度。

CDN是什么？使用CDN有什么优势？ - Xigang的回答 - 知乎
https://www.zhihu.com/question/36514327/answer/121026637

不适用CDN的情形：

 ![不适用CDN的情形](https://pic1.zhimg.com/80/v2-3cb264b4b37a79bdcd27afcbdf34b0e8_hd.jpg)

### Bootstrap 4 

Allows the web page to fit different screen size

### Reference

[Sample startup page](https://github.com/zero-to-mastery/Coding_Challenge-8)

* [Mailchimp](https://mailchimp.com)
  * App for creating users list: up to 2000 users for free

*	[Animate.css](https://daneden.github.io/animate.css)

* Website for patterns:
  * 这个评价高[Cruip: Free landing page templates for startups.](https://cruip.com/)
  * Creative Tim
    * https://www.creative-tim.com/bootstrap-themes/ui-kit?direction=asc&sort=price
    * https://www.creative-tim.com/
  * 这个有很多图标的template https://mdbootstrap.com/freebies/
  * 这个超好看 http://mashup-template.com/templates.html
  * 这个也不错https://startbootstrap.com/template-categories/all/

## 9.	__Career Of A Web Developer_

### How to make UI responsive to Screen size

* Bootstrap 4
* CSS Flexbox

* CSS grid

![CSS GIRDS VS FLEXBOX](https://qph.fs.quoracdn.net/main-qimg-273858213285396edb57d9bb175825d6)

### CSS grid

* Give the parent css grid and all the children will be under the grid system

* The best way is to use `fr`

  * *1fr* is for 1 part of the available space

  * you can mix *fr* values with fixed and percentage values. The *fr* values will be divided between the space that’s left after what’s taken by the other values.

  `.container{
      display:grid;
      grid-gap:20px;
      /*300 px 2 columns*/
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  }`

  * *minmax* allows to create grid tracks that **<u>flex to the available space, but that don’t shrink narrower than 200px size.</u>**
  * **<u>这里的1fr表示当页面宽度超过200px时，用每个单位长度为1fr（不小于200px）的格子autofill整行</u>**
    * width = 300, auto-fill 1* 200px
    * width = 400, auto-fill 2*200px
    * <u>width = 500, auto-fill 2*250px</u>
    * width = 600, auto-fill 3*200px
  *  After as many 100 pixel tracks are assigned, we then have the remaining space to distribute. **<u>Our tracks are allowed to be greater than 100 pixels wide so the remaining space is equally distributed.</u>** The result **as many equal width, flexible sized columns as can fit inside the container**.

  `repeat(times, xfr)`

  Use `auto` to fit the content in the grid

  `justify-items`元素上下

  `align-items`元素左右

  `justify-self`格子上下

  `align-self`格子左右

  * default value = `stretch`, value = `start, end, ...`

* For any individual grid:

  `    grid-column : 1/3;
      grid-row: span 2;`

### Media Query

[MDN: Media query](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

只有media之后的语句整体为真时，`{..}`的语句才得以执行。

```css
@media type/feature $logical_operator type/feature { ... }
```

`$logical_operator`: 

* `and` 且
* `only `只有
* `,` 或
* `not` 非
  * `not`覆盖到下一个`, `之前

```css
@media not screen and (color), print and (color) { ... }
=@media not (screen and (color)), print and (color) { ... }
```

课上的例子解决了content bar过窄无法全部显示的问题。

```css
@media only screen and (max-width: 600px){
    .main-nav{
        font:size:0.5em;
        padding: 0;
    }
}
```

### Reference

[Noshit.xyz](https://interfacer.xyz/)  各种免费设计元素

[Media query cheatsheet](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/) 不同尺寸显示器快速customize

[CSS grid cheatsheet](http://grid.malven.co/)

[CSS grid game](http://cssgridgarden.com/)

## 10.	__Javascript__

### 在html里使用script

在`<body>`末尾添加`<script>`关键字

### JAVASCRIPT TYPES

1. Number 
2. String
3. Boolean
4. Undefined
5. Null
  <!-- 6. Symbol (new in ECMAScript 6) -->
6. Object

### JAVASCRIPT COMPARISONS

`===` : check type and value

`==`: check value

 转义字符`\`

> !==
>

>=
><=
>
><

```javascript
5 + "34" // "534"
5 - "4" // 1
10 % 5 // 0
5 % 10 // 5
"Java" + "Script" // "JavaScript"
" " + " " //  "  "
" " + 0 //  " 0"
true + true // 2
true + false // 1
false + true //  1
false - true //  -1
3 - 4 //  -1
"Bob" - "bill" // NAN - not a number


5 >= 1 // true
0 === 1 //  false
4 <= 1 //  false
1 != 1 //  false
"A" > "B" //  false
"B" < "C" //  true
"a" > "A" //  true
"b" < "A" //  false
true === false //  false
true != true // false


// Make the string: "HI There! It's sunny out" by using the + sign.
"Hi There! " + "It\'s \"sunny\" out"
```

### JAVASCRIPT VARIABLES

var

* 在被assign前都是undefined

<!-- let (new in ECMAScript 6)-->  
<!-- const (new in ECMAScript 6)-->

* start with `$`/`_`/letters
* Use `prompt()`

```javascript
var first = prompt("enter the first number");
var second = prompt("enter the second number");
var sum = Number(first) + Number(second);
alert(sum);
// sum undefined
```

### JAVASCRIPT CONDITIONALS

[MDN: Javascript control flows](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)

*  [Falsy](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)  values

  - `false`
  - `undefined`
  - `null`
  - `0`
  - `NaN`
  - the empty string (`""`)

* block scope

  * Javascript does not have block scope except for [`let`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let) and [`const`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const) 

  * ```javascript
    var x = 1;
    {
      var x = 2;
    }
    console.log(x); // outputs 2
    ```

  * Starting with ECMAScript2015, the `let` and `const` variable declarations are block scoped. See the [`let`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let) and [`const`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const) reference pages for more information.

```javascript
if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
} 
```

<!-- ternary operator -->
<!-- switch -->

```javascript
switch (expression) {
  case label_1:
    statements_1
    [break;]
  case label_2:
    statements_2
    [break;]
    ...
  default:
    statements_def
    [break;]
}
```


### JAVASCRIPT LOGICAL OPERATORS
&&

||
!

### JAVASCRIPT FUNCTIONS

[MDN: javasript functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

* Define a function

  ```javascript
  var a = function name() {}
  function name() {}
  return
  ```

  <!-- () => (new in ECMAScript 6) -->

* Function scope

  * Nested functions

    ```javascript
    function outside(x) {
      function inside(y) {
        return x + y;
      }
      return inside;
    }
    fn_inside = outside(3); // Think of it like: give me a function that adds 3 to whatever you give
                            // it
    result = fn_inside(5); // returns 8
    
    result1 = outside(3)(5); // returns 8
    ```

#### Function hoisting

- functions are *hoisted*: independently of where a function declaration is mentioned in its scope, **it is always created at the beginning of the scope.**

  #### { // Enter a new scope


    console.log(foo()); // OK, due to hoisting
    
    function foo() {
    
        return 'hello';
    
    }

}

### JAVASCRIPT DATA STRUCTURES

#### Array

[Indexed collections](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Indexed_collections)

类似于arraylist

```javascript
var number = [1,2,3,4]
> undefined
var mix = [1,'c']
> undefined
number.shift();
> 1
number
> (3) [2, 3, 4]
number.pop();
> 4
number
> (2) [2, 3]

for(var i in number){
	console.log(i);

} // print the index
> VM719:2 0
> VM719:2 1
> undefined

for(var i in number){
	console.log(number[i]);

} // print the value
> VM751:2 2
> VM751:2 3
> undefined
```

##### Common APIs

* push()/pop()

* unShift()/shift()
* sort()
* concat() - not in-place, returns a new array
* slice(start, end)

```javascript
// using this array, 
var array = ["Banana", "Apples", "Oranges", "Blueberries"];

// 1. Remove the Banana from the array.
array.shift();

// 2. Sort the array in order. 
array.sort();

// 3. Put "Kiwi" at the end of the array.
array.push("Kiwi");

// 4. Remove "Apples" from the array.
array.splice(0, 1);

// 5. Sort the array in reverse order. 
array.reverse();

// using this array, 
// var array2 = ["Banana", ["Apples", ["Oranges"], "Blueberries"]];
// access "Oranges".
array2[1][1][0];
```

#### Object

[MDN: working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

Each `property_i` is an identifier (either a <u>name, a number, or a string literal</u>)

```javascript
objectName.methodname = functionName;

var myObj = {
    
    property_1:   value_1,   // property_# may be an identifier...
             2:   value_2,  // or a Number
       // ...,
            'property n’: value_n ; // or a string
    
  myMethod: function(params) {
    // ...do something
  }

  // OR THIS WORKS TOO

  myOtherMethod(params) {
    // ...do something else
  }
};
```

##### Methods

Methods are defined the way normal functions are defined, except that they have to be assigned as the property of an object. 

* Only comparing the same object reference with itself yields true.

![image-20190314193451221](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190314193451221.png)

### JAVASCRIPT LOOPING

[MDN: Loops and Iterations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

#### for

```javascript
for ([initialExpression]; [condition]; [incrementExpression])
  statement
```

#### while

```javascript
do
  statement
while (condition);
```

#### do 

```javascript
while (condition)
  statement
```

#### forEach (new in ECMAScript 5) 

[MDN: forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

```javascript
array1.forEach(function(element, index) {
  console.log(element, index);
});
// expected output: "a 0"
// expected output: "b 1"
// expected output: "c 2"

function iterFunc(element, index){
      console.log(element, index);
}// iterFunc can be used for any array
anyArray.forEach(iterFunc);
```

#### label-break/continue

```javascript
break [label]; continue [label];
```

- When you use `break` with a label, it terminates the specified labeled statement.
- When you use `continue` with a label, it applies to the looping statement identified with that label.
- When you use `break` without a label, it terminates the innermost enclosing `while`, `do-while`, `for`, or `switch` immediately and transfers control to the following statement

### `for...in`  statement vs `for...of` statement

iterates a specified variable over all the enumerable properties of **<u>an object</u>**

While `for...in` iterates over property names, `for...of` iterates over property values:

```javascript
var arr = [3, 5, 7];
arr.foo = 'hello';

for (var i in arr) {
   console.log(i); // logs "0", "1", "2", "foo"
}

for (var i of arr) {
   console.log(i); // logs 3, 5, 7
}
```

### JAVASCRIPT KEYWORDS

break

case
catch
class
const
continue
debugger
default
delete
do
else
export
extends
finally
for
function
if
import
in
instanceof
new
return
super
switch
this
throw
try
typeof
var
void
while
with
yield

### Terminologies

```javascript
// function declaration
function newFunc(){
	...
}

// function expression
var newFunc = function(){
	...
}

var newFunc = function funcName(){
	...
};

//calling a function
alert();
new function(para1, para2);

//function vs method
function thisIsAFunction(){}
   

// creating an object    
var object = {
	thisIsAMethod: function(){}
}

//clone an object

//shallow clone, clone primitives and object references
let clone = Object.assign({},object);
let clone2 = {...object};
    
// deep clone, clone primitives and objects
let superClone = JSON.parse(JSON.stringify(object));

//calling a method
object.thisIsAMethod(paralist);
```

### Bonus

[JavaScript数据结构：树](https://segmentfault.com/a/1190000010095344)

## 11.	__DOM Manipulation__

### Basic Logic

A web browser has a window object that has a property 'document' that specifies what should get displayed.

The the document object model reads the HTML and CSS

JavaScript is read line by line by  JavaScript engine -In Google Chrome that's the V-8 engine.

And if it ever needs to change anything, JavaScript can speak with the document object (DOM) and modify the HTML and CSS. 

![image-20190314212215415](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190314212215415.png)

### DOM Selectors

```bash
DOM Selectors
--------------
getElementsByTagName
getElementsByClassName
getElementById

querySelector
querySelectorAll

getAttribute
setAttribute

##Changing Styles
style.{property} //ok

className //best
classList //best

classList.add
classList.remove
classList.toggle

##Bonus
innerHTML //DANGEROUS

parentElement
children

##It is important to CACHE selectors in variables
```

### Events

[event delegation](https://stackoverflow.com/a/33015903)

![image-20190316142311508](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190316142311508.png)

* [Callback Functions](https://www.udemy.com/the-complete-web-developer-zero-to-mastery/learn/v4/t/lecture/10807448?start=0)

  In the previous video you saw something interesting:

  Event listener syntax : 

  ```
  button.addEventListener("click", addListAfterClick);input.addEventListener("keypress", addListAfterKeypress);
  ```

  You didn't see the function being called like this as you may have expected: 

  ```
  button.addEventListener("click", addListAfterClick());input.addEventListener("keypress", addListAfterKeypress(event));
  ```

  This is something called a callback function. When that line of javascript runs, we don't want the addLisAfterClick function to run because we are just adding the event listener now to wait for click or keypress. We want to let it know though that we want this action to happen when a click happens. So the function now automatically gets run (gets added the ()) every time the click happens. So we are passing a reference to the function without running it.

### Shopping List Excercise

 

### BackGround Generator

![image-20190316184818365](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190316184818365.png)

### Reference websites:

*	[MDN: event reference](https://developer.mozilla.org/en-US/docs/web/Events)
*	[Key Codes](https://www.cambiaresearch.com/articles/15/javascript-char-codes-key-codes)
*	https://jquery.com/
*	http://youmightnotneedjquery.com/
*	https://babeljs.io/

## 12.	__Advanced Javascript__

### !!!How javascript works!!!

[js的面向对象,js是面向对象语言吗](https://www.jianshu.com/p/018d22baeb4e)

Javascript is a single-threaded language that can be non-blocking.

J<u>avascript is asychronous: use a callback() function to check callback queue everytime the stack is empty</u>

![image-20190321001557058](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190321001557058.png)

### !!!Modules!!!

[ES modules: A cartoon deep-dive](https://hacks.mozilla.org/2018/03/es-modules-a-cartoon-deep-dive/)

![image-20190322131038105](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322131038105.png)

### Scope

* 只有function能产生scope
* function内的var外部不可见
* function内可见全局变量
* 对于`let` 和`const` { }可见

### Advanced Control Flow

* tenary operator

* switch

  * Switch cases use **strict** comparison (===)

  ```javascript
  switch(expression) {
    case x:
      // code block
      break;
    case y:
      // code block
      break;
    default:
      // code block
  }
  ```

#### Advanced Loops

```js
const basket = {'apple','orange','stawberry' };
const fruit = {
    apple: 1;
    orange: 1;
    strawberry: 5;
}

// for .. of array, string
// iterate

for (item of basket){
   console.log(item);
}	// apple, orange, strawtberry

for (item in fruit){
    console.log(item)
}	// error: object not iterable

// for .. in objects
//enumerate

for (item in basket){
   console.log(item);
}	// 0, 1, 2

for (item in fruit){
    console.log(item)
}	// apple, orange, strawberry



const basket = ['apples', 'oranges', 'grapes'];
const detailedBasket = {
  apples: 5,
  oranges: 10,
  grapes: 1000
}

//1
for (let i = 0; i < basket.length; i++) {
  console.log(basket[i]);
}

//2
basket.forEach(item => {
  console.log(item);
})

for (item in detailedBasket) {
  console.log(item);
}

for (item of basket) {
  console.log(item);
}
---------
// Question #1:
// create a function called biggestNumberInArray() that takes
// an array as a parameter and returns the biggest number.
// biggestNumberInArray([-1,0,3,100, 99, 2, 99]) should return 100;
// Use at least 3 different types of javascript loops to write this:
const array = [-1,0,3,100, 99, 2, 99] // should return 100
const array2 = ['a', 3, 4, 2] // should return 4
const array3 = [] // should return 0

function biggestNumberInArray(arr) {
  let highest = 0;
  for (let i = 0; i < arr.length; i++) {
    if (highest < arr[i]) {
      highest = arr[i];
    }
  }
  return highest
}

function biggestNumberInArray2(arr) {
  let highest = 0;
  arr.forEach(item => {
    if (highest < item) {
      highest = item;
    }
  })
  return highest;
}

function biggestNumberInArray3(arr) {
  let highest = 0;
  for (item of arr) {
    if (highest < item) {
      highest = item;
    }
  }
  return highest;
}


biggestNumberInArray3(array3)


// Question #2:
// Write a function checkBasket() that lets you know if the item is in the basket or not
amazonBasket = {
  glasses: 1,
  books: 2,
  floss: 100
}

function checkBasket(basket, lookingFor) {
  for (item in basket) {
    if (item === lookingFor) {
      return `${lookingFor} is in your basket`
    }
  }
  return 'that does not exist in your basket'
}

```

### ES5 & ES6

ES7 = ecmaScript version6

use BABEL to transform it into universal version

#### `let`and`const`

* <u>**block-scoped variables (`let` and `const`) do not hoist as `undefined` to the top of their block scope.**</u>

* **var** and **let** are both used for function declaration in javascript but the difference between them is that **var** is <u>function scoped</u> and **let** is <u>block scoped.</u> 

* **const** value cannot be changed, either variable or a modifier of <u>function, or an object</u>

  * constant object: cannot reassign reference, can change properties

    ```javascript
    const personality = "puppy";
    const obj = {
        name: "guy";
        age:"26";
        relation: "boo-boo";
    }
    
    obj = 5;//error : assignment to constant vairable
    
    obj.relation = "breakup"; // this is fine
    
    //destructuring
    const {name: newname, age: newage} = obj;
    let {relation} = obj;
    
    // identical to
    const newname = obj.name;
    const newage = obj.age;
    let relation = obj.relation;
    ```

##### 特别小心: [Variables and scoping in ECMAScript 6](http://2ality.com/2015/02/es6-scoping.html)

[https://stackoverflow.com/a/33040926]

A function expression, that is:

```js
[const | let | var] = function () {} (or () =>
```

Is the creation of an anonymous function (`function () {}`) and the creation of a variable, and then the assignment of that anonymous function to that variable.

So the usual rules around variable hoisting within a scope -- **block-scoped variables (`let` and `const`) do not hoist as `undefined` to the top of their block scope.**

This means:

```js
if (true) {
    doSomething() // will fail
    const doSomething = function () {}
}
```

Will fail since `doSomething` is not defined. (It will throw a `ReferenceError`)

* Example

* ```javascript
  if(true){
   greet();
   const greet = function(){console.log("hi");};
  }
  > VM1378:2 Uncaught ReferenceError: greet is not defined
      at <anonymous>:2:2
  ```

#### Template String

Use back tiks ``;

```javascript
const name = "Mia";
const age = "22";
const feature = "pretty";

const greeting = `Hi ${name}! You seem to be ${age-5}. You are so ${feature}.`;

// default arg
function greet(name = "Miss", age = 18, feature = "smart"){
   return `Hi ${name}! You seem to be ${age-5}. You are so ${feature}.`;
}
```



![image-20190316200001113](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190316200001113.png)

![image-20190316200207694](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190316200207694.png)

#### Arrow Functions `=>`

[Arrow function examples](https://www.sitepoint.com/es6-arrow-functions-new-fat-concise-syntax-javascript/) : compare to ES5

```javascript
const add = (a,b) => a+b;
add(2,4); // returns 6

//array filter
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15];

// ES5
var divisibleByThrreeES5 = array.filter(function (v){
  return v % 3 === 0;
});

// ES6
const divisibleByThrreeES6 = array.filter(v => v % 3 === 0);
console.log(divisibleByThrreeES6); // [3, 6, 9, 12, 15]
```

### Advanced Function

Closure

* 保证函数调用的ref都保存着

Curried Function

* pass multiple arg

Compose

* 函数嵌套

```js
//Solve these problems:

//#1 Create a one line function that adds adds two parameters
const sum = (a, b) => a + b

//Closure: What does the last line return?
const addTo = x => y => x + y
var addToTen = addTo(10)
addToTen(3) // returns 13

//Currying: What does the last line return?
const sum = (a, b) => a + b
const curriedSum = (a) => (b) => a + b
curriedSum(30)(1) // 31


//Currying: What does the last line return?
const sum = (a, b) => a + b
const curriedSum = (a) => (b) => a + b
const add5 = curriedSum(5)
add5(12) // 17

//Composing: What does the last line return?
const compose = (f, g) => (a) => f(g(a));
const add1 = (num) => num + 1;
const add5 = (num) => num + 5;
compose(add1, add5)(10) // 16

//What are the two elements of a pure function?
1. Deterministic --> always produces the same results given the same inputs
2. No Side Effects -->  It does not depend on any state, or data, change during a program’s execution. It must only depend on its input elements.
```

### Array

[JS Array explorer](https://sdras.github.io/array-explorer/)

```js
// Complete the below questions using this array:
const array = [
	{
		username: "john",
		team: "red",
		score: 5,
		items: ["ball", "book", "pen"]
	},
	{
		username: "becky",
		team: "blue",
		score: 10,
		items: ["tape", "backpack", "pen"]
	},
	{
		username: "susy",
		team: "red",
		score: 55,
		items: ["ball", "eraser", "pen"]
	},
	{
		username: "tyson",
		team: "green",
		score: 1,
		items: ["book", "pen"]
	},

];

//Create an array using forEach that has all the usernames with a "!" to each of the usernames
let newArray = []
array.forEach(user => {
	let { username } = user;
	username = username + "!";
	newArray.push(username);
})
console.log(newArray);

//Create an array using map that has all the usernames with a "?" at the end of usernames
const mapArray = array.map(user => {
	let { username } = user;
	return username + "?";
})
console.log(mapArray);

//Filter the array to only include users who are on team: red
const filterArray = array.filter(user => {
	return user.team === "red";
})
console.log(filterArray);

//Find out the total score of all users using reduce
const total = array.reduce((acc, user) => {
	return acc + user.score
}, 0);
console.log(total);


// (1), what is the value of i? INDEX of the array.
// (2), Make this map function pure:
const arrayNum = [1, 2, 4, 5, 8, 9];
const newArray = arrayNum.map((num, i) => {
	return num * 2;
})



//BONUS: create a new list with all user information, but add "!" to the end of each items they own.
const answer = array.map(user => {
	user.items = user.items.map(item => {
		return item + "!"
	});
	return user;
})
console.log(answer);

```

### Type Coercion

== see 

https://dorey.github.io/JavaScript-Equality-Table/

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness

`NAN === NAN` - false

`Object.is(+0, -0)` -false

- double equals (`==`) will perform a type conversion when comparing two things, and will handle `NaN`, `-0`, and `+0` specially to conform to IEEE 754 (so `NaN != NaN`, and `-0 == +0`);
- triple equals (`===`) will do the same comparison as double equals (including the special handling for `NaN`, `-0`, and `+0`) but without type conversion; if the types differ, `false` is returned.
- `Object.is` does no type conversion and no special handling for `NaN`, `-0`, and `+0`(giving it the same behavior as `===` except on those special numeric values).

### Advanced Objects

```js
//Evaluate these:
//#1
[2] === [2] // false - array 
{} === {} // false - object

//#2 what is the value of property a for each object.
const object1 = { a: 5 }; // 4
const object2 = object1; // 4
const object3 = object2; // 4
const object4 = { a: 5}; // 5
object1.a = 4;


//#3 create two classes: an Animal class and a Mamal class. 
// create a cow that accepts a name, type and color and has a sound method that moo's her name, type and color. 
class Animal {
	constructor(name, type, color) {
		this.name = name;
		this.color = color;
		this.type = type;
	}
}

class Mamal extends Animal {
	constructor(name, type, color) {
		super(name, type, color)
	}
	sound() {
		console.log(`Moooo I'm ${this.name} and I'm a ${this.color} ${this.type}`);
	}
}

const cow = new Mamal('Shelly', 'cow', 'brown');

```

### ES7

`.includes()` - used in string and array

`a**b` - a^b

```js
// #1) Check if this array includes the name "John".
const dragons = ['Tim', 'Johnathan', 'Sandy', 'Sarah'];

dragons.includes('John') // false

// #2) Check if this array includes any name that has "John" inside of it. If it does, return that
// name or names in an array.
const dragons = ['Tim', 'Johnathan', 'Sandy', 'Sarah'];

dragons.filter(F) // ['Johnathan']

// #3) Create a function that calulates the power of 100 of a number entered as a parameter
const power100 = (num) => num**100;

// #4) Useing your function from #3, put in the paramter 10000. What is the result?
// Research for yourself why you get this result.

power100(10000) // Infinity
```

### ES8

```js
// Solve the below problems:

// #1) Line up the Turtle and the Rabbit at the start line:
const startLine = '     ||<- Start line';
let turtle = '🐢';
let rabbit = '🐇';

// it should look like this:
'     ||<- Start line'
'       🐢'
'       🐇'

// when you do:
console.log(startLine);
console.log(turtle);
console.log(rabbit);


turtle = turtle.padStart(8);
rabbit = rabbit.padStart(8);


// #2) What happens when you run turtle.trim().padEnd(9, '=') on the turtle variable
// Read about what the second parameter does in padEnd and padStart
turtle = turtle.trim().padEnd(9, '=');

'     ||<- Start line'
'🐢======='
'       🐇'


// #3) Get the below object to go from:
let obj = {
  my: 'name',
  is: 'Rudolf',
  the: 'raindeer'
}
// to this:
'my name is Rudolf the raindeer'
Object.entries(obj).map(value => value.join(" ")).join(' ')
```

#### Coding Example

#### New Usage

```js
// change everything below to the newer Javascript!

// let + const
let a = 'test';
const b = true;
const c = 789;
a = 'test2';


// Destructuring
const person = {
    firstName : "John",
    lastName  : "Doe",
    age       : 50,
    eyeColor  : "blue"
};

const { firstName, lastName, age, eyeColor } = person;


// Object properties
const a = 'test';
const b = true;
const c = 789;

const okObj = {a, b, c};

/* identical to
const okObj = {
    a: a;
    b: b;
    c: c;
}*/

// Template strings
const message = `Hello ${firstName} have I met you before? I think we met in ${city}. last summer no???`;


// default arguments
// default age to 10;
const isValidAge = (age = 10) => age;

// Symbol
// Create a symbol: "This is my first Symbol"
const sym = Symbol('This is my first Symbol');

// Arrow functions
const whereAmI = (username, location) => {
    if (username && location) {
        return "I am not lost";
    } else {
        return "I am totally lost!";
    }
}

```

## 13. __Command Line__

FOR MAC OR LINUX:


```bash
ls
Pwd
cd 
cd ..
Clear
Cd / —> root director
Cd ~
Cd folder/folder/test
Mkdir name
Open folder
Touch index.html
Open index.html
Open -a “Sublime Text”
Open .
Mv index.html about.html
Up and down arrow.
Rm file
Rm -r folder
Say hello (only on Mac).
```


FOR WINDOWS:


```cmd
dir - list files
cd {directory name} - change directory
cd / - go to root (top) directory
cd .. - go up a level
mkdir {file name} - make a directory
echo > {filename} - create an empty file
del {filename} - remove a file
rmdir {directory name} - remove a directory and all files within
rename {filename} {new filename} - rename a file or folder
start {filename} - open file in default program
start . - open current directory
cls - clear the terminal screen 
```

******************************************************************************************
## 14.	__Developer Environment__

哭了哭了这个好详细： [Mac OS setup guide](http://sourabhbajaj.com/mac-setup/)

## 15.	__Git + Github + Open Source Projects__

### Basic Command Walk through

Install Git:

*	https://www.atlassian.com/git/tutorials/install-git#windows
*	https://www.atlassian.com/git/tutorials/install-git


```bash
git clone “https:……”
git status
git add “filename”
git add .
git commit –m”message”
git push

// update 
git pull

//new branch
git branch
git branch “branchname1”

// go to branch 1
git checkout “branchname1”

// upadate with master to branch 1
git merge “master”
```

### Keeping Your Fork Up To Date

Once you are in your forked project directory in your command prompt....

1.	Type `git remote -v` and press Enter. You'll see the current configured remote repository for your fork.​

```bash
git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
```


2.	Type `git remote add upstream`, and then paste the URL you would copy from the original repository if you were to do a git clone. Press Enter. It will look like this:


```bash

git remote add upstream https://github.com/zero-to-mastery/PROJECT_NAME.git

```


3.	To verify the new upstream repository you've specified for your fork, type ```git remote -v``` again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.


4.	Now, you can keep your fork synced with the upstream repository with a few Git commands. 
  One simple way is to do the below command from the master of your forked repository: 
  ```git pull upstream master```

Or you can follow along another method here: "[Syncing a fork](https://help.github.com/articles/syncing-a-fork)."

### [Conribute to Open Source: walk through](https://github.com/firstcontributions/first-contributions)

* on how to participate in github projects

### [Student Generated Resources]( <https://zero-to-mastery.github.io/resources/>)

## 16.	__A Day In The Life Of A Developer__

## 17.	__NPM + NPM Scripts__

### How npm works

![image-20190322104927837](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322104927837.png)


```bash
npm init // creates package.json of the metadata
```

```bash
npm install –g browserify// install globally browserify
```

### ！Install and use package- Walkthrough

```bash
npm install lodash
```

locally创建 node_modules文件夹。并且package.json文件里会加入lodash的dependency。安装lodash后如下图。

![image-20190322130325352](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322130325352.png)

用import方法调用lodash中的js文件。

![image-20190322130711741](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322130711741.png)

chrome浏览器目前不支持import功能。

![image-20190322130815787](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322130815787.png)

使用browserify。

```bash
npm -g install browserify
```

bundle the modules.

```bash
browserify scripts.js > bundle.js
```

![image-20190322131555726](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322131555726.png)

#### ！[how browserify works](https://github.com/browserify/browserify-handbook#how-browserify-works)

初衷是让Node.js的syntax可以在browser上执行。

browserify 会根据`scripts.js`里的`require()`方法在`node_modules`(之前`npm install`产生的)里搜索所需最精简的source code，生成`bundle.js` 。

In this case, it searches the `node_modules` and include `lodash` in `bundle.js`. Now `bundle.js` contains all the javascript that `script.js` needs to work. 

在html文件里引用`bundle.js`即可。Just plop it into a single script tag in some html: [bundling for the browser](https://github.com/browserify/browserify-handbook#bundling-for-the-browser)

```javascript
<html>
  <body>
    <script src="bundle.js"></script>
  </body>
</html>
```

(Browserify starts at the entry point files that you give it and searches for any `require()` calls it finds using [static analysis](http://npmjs.org/package/detective)of the source code's [abstract syntax tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree). 

This means that the bundle you generate is completely self-contained and has everything your application needs to work with a pretty negligible overhead.)

![image-20190322132158419](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322132158419.png)

例： 调用lodash里的without函数

![image-20190322133146129](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322133146129.png)

### ！How NPM works！

```bash
npm install
```

自动安装package.json里dependency所需的模块（default as `nodes_modules`）git上传只需要上传pakcage.json即可。

删去node_module文件夹，调用以上语句，根据denpendcy再次自动安装lodash模块。

![image-20190322140512320](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322140512320.png)

#### 统一调用

直接在build下写入需要bundle和安装的语句。

```json
"build" : "browserify script.js > bundle.js && live-server" 
```

Then in command line,

```bash
npm run build
```

![image-20190322141555260](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322141555260.png)

![image-20190322141322273](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322141322273.png)

### Reference websites:

* Install node and npm	
  * https://www.npmjs.com/get-npm
  * https://nodejs.org/es/

*	https://www.npmjs.com/
*	https://www.npmjs.com/package/react
*	https://lodash.com/

## 18.	__React.js + Redux__

### React的特点

[React.js的特点](https://www.jianshu.com/p/aaf4e14c4e4b)

[谈谈React.js的核心入门知识](https://www.imooc.com/article/1389)

* By components, rather than by language
* Data flow : single direction, top to bottom

### Create a React App

```bash
sudo npm install –g create-react-app
create-react-app robotfriend
npm start
```

![image-20190322160549800](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322160549800.png)

![image-20190322160506472](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322160506472.png)

### Upgrade to newer version

![image-20190322161701784](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322161701784.png)

![image-20190322161820306](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322161820306.png)



* 不理解的部分： 各个包的作用

  ![image-20190322163110743](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322163110743.png)

```
npm install tachyons
```

![image-20190322164723268](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322164723268.png)

### First Component example - Hello

![image-20190322191333418](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322191333418.png)

When we need immutable data in our component, we can just add props to **reactDOM.render()** function in **main.js** and use it inside our component. [more about props](https://www.tutorialspoint.com/reactjs/reactjs_props_overview.htm)

To call the properties:

 Can write a function

![image-20190322191249535](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322191249535.png)

Or you can write an object

```jsx
import React, { Component } from 'react';
import './Hello.css';
class Hello extends Component{
    render(){

        return (

            //use 'className' instead of 'class' as it is reserved for JavaScript
           <div className = 'f1 tc'>
           <h1>Hello World</h1>
           <p>this.props.greeting</p>
           </div>

            )

    }
}

export default Hello;
```

![image-20190322191419360](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322191419360.png)

Output:

![image-20190322191452028](/Users/miawenjinzhang/Library/Application Support/typora-user-images/image-20190322191452028.png)

### Card/Cardlist/Index.js

​		 		 display 		map		info from

​		Index <-------- Cardlist.js <--------Card.js <--------------Robot.js

Import  		↑_ _ _ _ _ _ _ _	_↑ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _| 

​						↑_ _	_ _ _ _ _ _ _| 

* 所有的return后面跟(..), (..)里面默认是html syntax
* 想使用 javascript，必须外面添加{ };
* 每个js文件（component）末尾都要export，非default时要加{ }（？？？为什么）
  * 变量名和文件名须一致？（case-insensitive however）

### Service Worker

* Invoked by default in create-react-app

* Essentially a seperate javascript file runs from main thread (asynchronized)

* Can process requests, and push messages <u>offline</u>, which improves application performance

* Two APIs: 

   [Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)(a standard way to retrieve content from the network) and [Cache](https://developer.mozilla.org/en-US/docs/Web/API/Cache) (a persistent content storage for application data). This cache is persistent and independent from the browser cache or network status.

Complete information in: [Service Worker Introduction](https://developers.google.com/web/ilt/pwa/introduction-to-service-worker)

### References

website for fonts download:

*	http://www.cufonfonts.com/en


Reference websites:
*	https://reactjs.org/docs/react-component.html
*	https://jsonplaceholder.typicode.com/
*	http://atomicdesign.bradfrost.com/
*	https://robohash.org

Action --> Reducer --> Store --> Make changes

```
npm install redux
npm install react-redux
npm install redux-logger 
npm install redux-thunk
```


*	https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en
*	https://reacttraining.com/react-router/
*	https://ramdajs.com/
*	https://lodash.com
*	https://glamorous.rocks
*	https://www.styled-components.com
*	https://github.com/css-modules/css-modules
*	https://www.gatsbyjs.org
*	https://zeit.co/blog/next5
*	www.material-ui.com/#/components/app-bar
*	https://react.semantic-ui.com/elements/button
*	https://github.com/reactjs/reselect
*	https://redux-saga.js.org
*	https://facebook.github.io/immutable-js/

## 19.	__HTTP/JSON/AJAX + Asynchronous Javascript__
## 20.	__Backend Basics__
## 21. __APIs__
* https://stripe.com/docs/api

*	https://www.twilio.com/docs/api/messaging/send-messages
*	https://apilist.fun

## 22.	__FINAL PROJECT: SmartBrain Front-End__


Animated objects library:
*	https://www.npmjs.com/package/react-tilt
	```
	npm install –save react-tilt
	```

background patterns:
*	http://lea.verou.me/css3patterns/


animated background library:
*	https://vincentgarreau.com/particles.js/

	```
	npm install react-particles-js
	```

image and video recognition:
*	https://clarifai.com/developer/guide/
	```
	npm install clarifai
	```
icons library:
*	https://icons8.com/icon
	
## 23.	__Node.js + Express.js__

Install Postman:
*	https://www.getpostman.com/apps

Express.js
*	https://expressjs.com/en/api.html

(Getting start guide)

```
npm install body-parser
npm install express --save
npm install --save-dev nodemon
```

Reference webs:
*	https://nodejs.org/en/
*	https://nodejs.org/api/modules.html

storing passwords securely:
```
npm install bcrypt-nodejs
```
*	https://www.npmjs.com/package/bcrypt-nodejs
*	https://www.npmjs.com/package/argon2


```
$ npm install bcrypt
```

```jsx
1.	/*
2.	* You can copy and run the code below to play around with bcrypt
3.	* However this is for demonstration purposes only. Use these concepts
4.	* to adapt to your own project needs.
5.	*/
6.	 
7.	import bcrypt from'bcrypt'
8.	const saltRounds = 10 // increase this if you want more iterations  
9.	const userPassword = 'supersecretpassword'  
10.	const randomPassword = 'fakepassword'
11.	 
12.	const storeUserPassword = (password, salt) =>  
13.	  bcrypt.hash(password, salt).then(storeHashInDatabase)
14.	 
15.	const storeHashInDatabase = (hash) => {  
16.	   // Store the hash in your password DB
17.	   return hash // For now we are returning the hash for testing at the bottom
18.	}
19.	 
20.	// Returns true if user password is correct, returns false otherwise
21.	const checkUserPassword = (enteredPassword, storedPasswordHash) =>  
22.	  bcrypt.compare(enteredPassword, storedPasswordHash)
23.	 
24.	 
25.	// This is for demonstration purposes only.
26.	storeUserPassword(userPassword, saltRounds)  
27.	  .then(hash =>
28.	    // change param userPassword to randomPassword to get false
29.	    checkUserPassword(userPassword, hash)
30.	  )
31.	  .then(console.log)
32.	  .catch(console.error)
```

## 24.	__FINAL PROJECT: SmartBrain Back-End -- Server__


Change localhost:
*	https://stackoverflow.com/questions/40714583/how-to-specify-a-port-to-run-a-create-react-app-based-project

If you don't want set environment variable, other option - modify scripts part of package.json from:

```"start": "react-scripts start"```

Linux (tested on Ubuntu 14.04/16.04) and MacOS (tested by @aswin-s on MacOS Sierra 10.12.4) to:

```"start": "PORT=3006 react-scripts start"```

or (may be) more general solution by @IsaacPak to:

```"start": "export PORT=3006 react-scripts start"```

Windows @JacobEnsor solution to:

```"start": "set PORT=3006 && react-scripts start"```


Front-end and back-end connection:
*	https://www.npmjs.com/package/cors
	```
	npm install cors
	```

front-end:  

```Javascript
fetch('http://localhost:3000/image', {
	method: 'put',
	headers: {'Content-Type': 'application/json'},
	body: JSON.stringify({
		id: this.state.user.id
	})
})
.then(response => response.json())
.then(count => {
	this.setState(Object.assign(this.state.user, { entries:count}))
})
```
Back-end:

```Javascript
const cors = require('cors')
app.use(cors());
```

## 25.	__Databases__


Install PostgreSQL:

*	http://www.psequel.com/

	en el terminal:
	```zsh
	brew update
	brew doctor
	brew install postgresql
	brew services start postgresql
	brew services stop postgresql
	createdb ‘test’
	psql ‘test’
	```

	for windows:

*	https://www.pgadmin.org/download/pgadmin-4-windows/
*	http://www.postgresqltutorial.com/install-postgresql/

	```cmd
	@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('https://s3.amazonaws.com/pgcentral/install.ps1'))"

	cd bigsql
	pgc install pg10
	pgc start pg10
	```
*	http://dc-apuntes.blogspot.com/2016/04/comandos-postgres-desde-cmd-windows.html
*	https://www.w3resource.com/PostgreSQL/connect-to-postgresql-database.php
*	https://www.youtube.com/watch?v=fD7x8hd9yE4

data types
*	https://www.techonthenet.com/postgresql/datatypes.php

terminal commands for windows

login: (-U usuario)

	psql -h localhost -U postgres

create database	

	create database database_name;

show all datatables:

	\l

Create a user:

	create user moni with password ‘moni’;

delete database

	drop database database_name;

connect to a database:

	\c database_name;

Create a squema:

	create schema friends;

Create a table

	create table Friends.test( firstname CHAR(15), lastname CHAR(20)); 
	
	create table Friends.login(id serial not null primary key, secret varchar (100) not null, name text unique not null, entries bigint default 0, joined timestamp not null);

show all information of a table

	select * from friends.test;
describe database

	\d friends.test

Insert data

	insert into friends.test values( ‘Mike’, ‘Smith’); 
	
	insert into friends.test (firstname, lastname )values( ‘Sally’, ‘Jones’);

add a column to an existing table

	alter table Friends.test add age smallint;

update data from the table

	update friends.test set age = 25 where firstname= ‘Mike’;

delete data from the table

	delete from friends.test where firstname = ‘Mike’;

delete column from a tableinae

	alter table friends.test drop column age;

delete a table

	drop table friends.test;

functions

	select avg(age) from friends.test;

join tables

	select * from friends.test join friends.login on friends.test.firstname = friends.login.name;

exit

	\q

List users in postgres: 

	\du
List all tables in a squeme: 

	\d+ nombre_Esquema.*

List all tables in a database : 

	\dt *.* 

List a table in a squeme: 

	\d+ nombre_Esquema . nombre_Tabla

Show description of a tavle, columns, type, modifications,....: 

	\d+ nombre_Tabla

Create a backup of a database: 

	pg_dum -h localhost -U postgres nombre_Base > nombre_Base.sql

Restore a database: 1. Create a new database where the restore file is going to be placed

	psql -U postgres -d nombre_nuevaBase -f respaldo.sql
	
	*Note:  it is important to create the restore in the same root where the database copy is saved. 

Enter to postgres with a user different to postgres: 

	psql -h localhost -d postgres -U usuario

Enter to a database with a different user: 

	psql -h localhost -d nombre_base -U nombre_usuario

## 26.	__FINAL PROJECT: SmartBrain Back-End – Database__


Tool for db connection with back-end
*	https://knexjs.org/
*	https://knexjs.org/#Installation-node
*	https://github.com/vitaly-t/pg-promise

## 27.	__Production + Deployment__


Environmental variables 
*	http://www.dowdandassociates.com/blog/content/howto-set-an-environment-variable-in-windows-command-line-and-registry/

### PORT

on terminal

	bash
	-->PORT-3000 node server.js

On server.js
```JSX
	const PORT = process.env.PORT
	app.listen(PORT, ()=>{
		console.log(`app is running on port ${PORT}`);
	})
```

### DATABASE

on terminal

	bash
	-->DATABASE_URL-123  node server.js

On server.js

```jsx
	const DATABASE_URL = process.env. DATABASE_URL
	app.listen(3000, ()=>{
		console.log(`app is running on port ${ DATABASE_URL }`);
	})
```

### OTHER OPTION

On terminal

	fish
	-->env DATABASE_URL-‘hello’ node server.js

Deploy apps:

Heroku:

*	https://www.heroku.com/
*	https://devcenter.heroku.com/articles/git

Not the best one:
*	https://www.hostgator.com/promo/snappy60?utm_source=google&utm_medium=brandsearch&kclickid=cfe89874-3c6a-404e-b321-fc3e56f9ec2b&gclid=CjwKCAjwsJ3ZBRBJEiwAtuvtlIkFb-qOw3HN_JpH3AAkmYwKhk_L0y0stl7J1CFRR8FRltvmvhwXPBoCATIQAvD_BwE



commands for heroku on backend folder:
install heroku:
```
npm install -g heroku
heroku login
heroku create
```
In the terminal there will be an URL : ” https://limitless-bastion-10041.herokuapp.com/”
```
git remote –v
git push origin master
heroku git: remote –a limitless-bastion-10041
```

changes required in:

*	BACKEND: PORT in server.js needs to be changed by an environment variable
*	FRONT: fetch URL needs to be changed by the URL of HEROKU + “:3000”

```
git push heroku master
for checking errors:
heroku logs --tail
heroku open
```


connect to pg database:
*	https://devcenter.heroku.com/articles/heroku-postgresql
*	https://docs.aws.amazon.com/es_es/AmazonRDS/latest/UserGuide/USER_ConnectToPostgreSQLInstance.html
*	https://msdn.microsoft.com/en-us/library/ms175043(v=sql.120).aspx#SSMSProcedure
	

create on heroku app a new postgress:

Data: Heroku postgres: create new: install heroku postgres: select the app created
```
heroku addons
heroku info
heroku pg:psql
```

## 28.	__Where To Go From Here?__
The Complete Junior to Senior Web Developer Roadmap (2019):
*	https://www.udemy.com/the-complete-junior-to-senior-web-developer-roadmap/

## 29.	__Bonus: AMA + Developer Morning Routine__


