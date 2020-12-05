# JAVASCRIPT

>The rules for creating identifire >in JS are

       -The name of the identifire should not be a pre-defined Keyword.(you can't use var in place of num)

       - The first character must be a letter, an (_)underscore or doller sign($),subsequent characters may be an letter or digit or an underscore or doller sign. 

       - Variables are case sensitive.


        **Js is LOOSELY typed.**
		**JS is DYNAMICALLY TYPED.**

```c
<!DOCTYPE html>
<html>
<head>
	<title>my title</title>
	<script type="text/javascript">
		var num = 16;
		document.write(num);
		</script>
		</head> 
<body> 
       <h3>javascript</h3>
</body>
</html>
```
>Output:- 16
>         javascript

```c
<!DOCTYPE html>
<html>
<head>
	<title>my title</title>
	<script type="text/javascript">
		var x;
        x=5;
        alert(x);
        </script>
		</head> 
<body> 
       <h3>javascript</h3>
</body>
</html>
```
> output:- 5
>         javascript


# OPERATORS IN JS

```c
<!DOCTYPE html>
<html>
<head>
	<title>Operators in JS</title>
	<script type="text/javascript">

		//Adittion
		var a = 3; //right-to-left
		var b = 3;
		var c = 6;
		var result = c+b+ "teza"+(a + b) + c;
		//[left-to-right]
		//adding two variables
		var result2 = a+b*c; //it follows BODMAS rule


		document.write("<h1>Result is:"+result2+"</h1>");//here + used to concatinate
	</script>
</head>
<body>

</body>
</html>
```
>Output:- Result is:21

# Switch Case in JS

```c
<!DOCTYPE html>
<html>
<head>
	<title>Switch case in JS</title>
	<script type="text/javascript">
	var day = 4 ;
	switch(day)
    {
    	case 1:
    	document.write("<h2>Sunday</h2>");
    	break;
    	case 2:
    	document.write("<h2>Monday</h2>");
    	break;
    	case 3:
    	document.write("<h2>Tuesday</h2>");
    	break;
    	case 4:
    	document.write("<h2>wednesday</h2>");
    	case 5:
    	document.write("<h2>thrusday</h2>");
    	break;
    	case 6:
    	document.write("<h2>friday</h2>");
    	case 7:
    	document.write("<h2>Saturday</h2>");
    	break;
    	default:
    	document.write("<h2>wrong input</h2>");

   }
    </script>
</head>
<body>

</body>
</html>

```
> Output:- wednesday


# FOR LOOP IN JS
```c
<html>
<head>
<title>for loop in js</title>
<script type="text/javascript">
        /*Q1)print multiplication  table of 5 using for loop*/

        /*Q2)Print first 5 even number*/ //2 4 6 8 10

        // for loop is used when the number or iterations is known in advance

        //for(init;condition;increment/decrement)

        //Code for 1st question
        for(var x=1;x<=10;x++)
        {
            document.write("<h2>"+(5*x)+"</h2>");
        }

        
        //code for 2nd question
      /*  for(var x=2;x<=10;x+=2) //x+=2 equalis to  x=x+2
        {
            document.write("<h2>"+(x)+"</h2>");
        }*/
    </script>
</head>
<body>
</body>
</html>
```
first line is output of first code 
Second line iss output of second code.

> output:- 
>          5    2nd output
>          10      2
>          15      4
>          20      6
>          25      8
>          30      10
>          35    
>          40
>          45
>          50

# While loop in JS

>Print the first 5 odd nubers 
>using while loop
```c
<!DOCTYPE html>
<html>
<head>
    <title>While loop in JS</title>
    <script type="text/javascript">
        /*Q1) Print the first 5 odd nubers using while loop*/

        var x = 1;
        while(x<10)
        {
           document.write("<h1>"+x+"</h1>");
           x=x+2; //x+=2 
           //[writting x=x+2 is compulsory loop will go infinite]
        }
    </script>
</head>
<body>

</body>
</html>
```
> output:-
>1
>3
>5
>7
>9

# Do while loop 
```c
<!DOCTYPE html>
<html>
<head>
    <title>Do-While Loop</title>
    <script type="text/javascript">
        /*Q1) Display usages of do while-loop*/

        var x = 1;
        do{
           document.write("<h2>Anjali</h2>");
        }while(x>5);// here condition is false but still Anjali is printed because of do-while loop.




 

        var y = 9;
        do{
           document.write("<h2>Anjali Tejasvi</h2>");
           y--;
        }while(y>5);


    </script>
</head>
<body>

</body>
</html>
```
>Anjali
>Anjali Tejasvi
>Anjali Tejasvi
>Anjali Tejasvi
>Anjali Tejasvi

# Functions in JS

```c
<!DOCTYPE html>
<html>
<head>
    <title>functions inJS</title>
    <script type="text/javascript">
        /*

        functions are on of the fundamental building bloks in JS.
        A functions is a set of statements that performes a task or calculate a value.
        A javascript function is executed when "something" invokes it (calls it).*/



        /* Q1) write a function to add 2 numbers and print the result*/

        

     //syntax of a function
     function add2Number(a,b)
     {
        
        var total = a+b;

        document.write("<h1> The total is :"+total+"</h1>");
     }

     add2Number("Both are seperated","by comma and written in place of a,b");// Function call
     
    </script>
</head>
<body>

</body>
</html>
```
>output:-The total is :Both are 
>seperatedby comma and written in 
>place of a,b

# Scope of Variable

```c
<!DOCTYPE html>
<html>
<head>
    <title>Scope of Variable</title>
    <script type="text/javascript">
           
           /*In JS we have 2 types of scopes - globle & Local depending upon where you create your variables*/


           var a = 5;// globle value 
           document.write("<h2>"+a+"</h2>"); 

           function myfunction()
           {
            var b = 4;//local variable
            document.write("<h2>"+b+"</h2>"); 

           }


           myfunction();


           //Arrays in JS

           var car1 = "Audi";
           var car2 = "Volvo";
           var car3 = "BMW";

           var cars = ["BMW","Volvo","Audi"];
           cars.push("Mercedes");

           for(var i =0; i<cars.length;i++)
           {

           document.write("<h2>"+cars[i]+"</h2>");
           } 

    </script>
</head>
<body>

</body>
</html>
```
>5
>4
>BMW
>Volvo
>Audi
>Mercedes

# Introduction to Objects
```c
<!DOCTYPE html>
<html>
<head>
    <title>Inroduction to Objects</title>
    <script type="text/javascript">
        /*Objects in JS*/


        var Car = {

            car_brand :"Tesla",
            car_model :"Model ",
            price : 35000,


            teslaAutoPilot : function()
            {
                document.write("<h2>This car has Auto pilot</h2>");
            }
        }
        Car.teslaAutoPilot();
        document.write("<h2>"+Car.car_brand+"</h2>");



        function Cars(car_brand,car_model,price)
        {
            this.car_brand = car_brand;
            this.car_model = car_model;
            this.price = price;
            this.teslaAutoPilot = function()

            {
                document.write("<h2>This car has Auto pilot</h2>");
            }
        }
 
        var c1 = new Cars("Tesla","Model","350000");
        var c2 = new Cars("Tesla","BR3008","4500000")
        c1.teslaAutoPilot();
        document.write("<h2>"+c2.car_model)




        
    </script>
</head>
<body>

</body>
</html>
```
>This car has Auto pilot
>Tesla
>This car has Auto pilot
>BR3008 

# Introduction to Objects[To add or delete the property]

```c
<!DOCTYPE html>
<html>
<head>
    <title>Introduction to Objects[To add or delete the property]</title>
    <script type ="text/javascript">
        //Objects in JS 

        /*
        Booleans can be objects(if defined with the new Keyword)

        Numbers can be objects(if defined with the new keyword)

        strrings can be objcts (if defined with the new keyword)

        Dates are always objects
        Maths are always
        Regular expressions are always objects


        */
        var str1 = new String();
        
        var Car = {

            car_brand :"Tesla",
            car_model :"Model ",
            price : 35000,


            teslaAutoPilot : function()
            {
        document.write("<h2>This car has Auto pilot</h2>");
            }
        }

    Car.fuleType = "Electric";
    Car.teslaAutoPilot();
        document.write("<h2>"+typeof(str1)+"</h2>");
    /*  Output :- Object [If str will be written insted of
    new. String then Output will be String not Object]*/

    document.write("<h2>"+Car.car_brand+"</h2>");
    //      Output :- Tesla
    document.write("<h2>"+Car.fuleType+"</h2>");


/*Suppose we have to delete any property then we can use 
  delete Car.price;  and if we gonna print it it will 
  print Undefined */


    
    delete Car.price; 
    document.write("<h2>"+Car.price+"</h2>");
    //Output  :- Undefined
    </script>
</head>
<body>

</body>
</html>

```
>This car has Auto pilot
>object
>Tesla
>Electric
>undefined

# Introduction to Objects [Dom manpulation & getelementbyId method]

```c
<!DOCTYPE html>
<html>
    <head>
    <title>Introduction to Objects</title>
    <script type = "text/javascript">
    /*Dom manpulation & getelementbyId method
        */

    function buttonClick()
    {
        document.getElementById("heading").innerHTML="After clicking on the button you can see this [txt is changed]";
        alert("Button clicked");

 
       var x = document.getElementById("heading").innerHTML;
    alert(x);
    }

    buttonClick();
    </script>
    
</head>
<body>
    <button onclick = "buttonClick()">Click on Me</button>
    <h2 id = "heading">Some Random Text</h2>
     
</body>
</html>
```
>Output :-
>![first-img](recent:///397813e40d937839b45067a65fcae46a)
>![second img](recent:///c1b26a5d5d12861b58659ca25fcae46a)

# Dom Manipulation [Enter username and password by getElementbyId method]

```c
<!DOCTYPE html>
<html>
<head>
<title>DOM manipulations</title>
<script type = "text/javascript">
    /*DOM maniulation and getelementbyId method*/
    function fun1()
    {
        var str =  document.getElementById("text1").value;
        alert("Value inside the text box is:" +str);
    }

</script>
</head>
<body>

    <input id = "text1" placeholder = "username">
    <br><br>
    <input type = "password" id = "text2" placeholder = "password">
        <br><br>

    <button onclick = "fun1()" id = "button1">Click me</button>
</body>
</html>

```
# DOM manipulations[Use of if-else and else if statement in JS]

```c
<!DOCTYPE html>
<html>
<head>
<title>DOM manipulations</title>
<script type = "text/javascript">
    /* DOM manipulation & getelementbyId method*/

    function fn1()
    {
        var rd1 = document.getElementById("rd1");
        var rd2 = document.getElementById("rd2");
       
        if(rd1.checked == true)
            alert("The channel selected is: "+rd1.value);
        else if(rd2.checked == true)
        alert("The channel selected is: "+rd2.value);

        else
            alert("No channel Selected");
    }
    
</script>
</head>
<body>
    <input id = "rd1" name = "grp1" type = "radio"
    value = "Web Development">Web Development</input><br><br>

    <input id = "rd2" name = "grp1" type = "radio"
        value = "Android Development">Android Development</input><br><br>

    <button onclick = "fn1()" id = "btn1">Click me </button>
</body>
</html>

```
####  DOM manipulations[**select.options[select.selectedIndex].value**]

```c
!DOCTYPE html>
<html>
<head>
    <title>DOM manipulations</title>
<script type = "text/javascript">
/*DOM manipulation & getelementbyId method*/

    function fn1()
    {
        var select = document.getElementById("selectbox");
        alert(select.options[select.selectedIndex].value)
    }
</script>

</head>
<body>
    <select id = "selectbox">
    <option value = "Phython">Phython</option>
    <option value = "R language">R language</option>
    <option value = "core Java">core Java</option>
    <option value = "Javascript">Javascript</option>
    </select>
    <br><br>
    <button onclick = "fn1()">Click Me</button>

</body>
</html>
```
# DOM manipulation[Using CSS and array]

```c
<!DOCTYPE html>
<html>
<head>
    <title>DOM manipulation</title>
    <script type="text/javascript">
        
        function changeStyling() 
        {
            var para = document.getElementsByTagName("p");
        para[0].style.color = "brown";
        para[0].style.fontWeight = "bold";
        para[1].style.color = "tomato";
        para[2].style.fontWeight = "bold";
        para[3].style.fontStyle = "italic";
        para[3].style.color="green";
        para[4].style.color = "blue";
        /*for(var i = 0; i<para.length;i++)
        {
            para[i].style.color = "blue";
        }*/

          }
    </script>
</head>
<body>
        <p>This is paragraph 1</p>
        <p>This is paragraph 2</p>
        <p>This is paragraph 3</p>
        <p>This is paragraph 4</p>
        <p>This is paragraph 5</p>

        <br>
        <button onclick="changeStyling()">Click Me</button>
</body>
</html>
```
# getElementsByClassName

```c
<!DOCTYPE html>
<html>
<head>
    <title>getElementsByClassName</title>
    <script type="text/javascript">
        function fn1() 
        {
            //var tag = document.getElementsByTagName("p");
            var element = document.getElementsByClassName("mypara");
            for(var x =0;x<element.length;x++)
            {
                element[x].style.color = "red";
            }
        }

    </script>
</head>
<body>
       <p class="mypara">This is paragraph 1</p>
       <p>this is paragraph 2</p>
       <p class="mypara">This is parag raph 3</p>
       <p>This is paragraph 4</p>
       <p class="mypara">This is paragraph 5</p>
       <a class = "mypara" href="https://www.google.com/">Google</a>

       <br><br>
       <button onclick="fn1()">Click on me</button>

</body>
</html>

```
# Form Validations

```c
<!DOCTYPE html>
<html>
<head>
    <title>Form Validations</title>
    <script type="text/javascript">
        /* */

        function validate()
        {
            var username = document.getElementById("uname");
            var password = document.getElementById("pass");

            if (username.value.trim() =="" ||password.value =="") //trim is used to neglect spaces(matlab jab bhi koi space dalega tho usko consider nahi karega)
                {
                    alert("No blank value allowed");
                    return false;
                } 
                else {
                    true;
                }
        }
        
    </script>
</head>
<body>
    <form onsubmit = "return validate()" action="https://www.google.com/">
        <input id="uname" placeholder="Username" type="text"/><br><br>

        <input id = "pass" placeholder = "password" type="password"/>
        <br><br>

        <button onclick="validate()" type="submit">Submit</button>
    </form>
</body>
</html>
```
# Form Validations[part 2]
```c
<html>
<head>
    <title>Form Validations</title>
    <script type="text/javascript">
        /* */

        function validate()
        {
            var username = document.getElementById("uname");
            var password = document.getElementById("pass");

            if(uname.value.trim() =="")
            {
                //alert("Blank Username");
                uname.style.border = "solid 3px red";
                document.getElementById("lbluser").style.visibility ="visible";
                return false;
            } 
            else if(password.value.trim() =="")
            {
                alert("Blank password");
                return false;
            }
            else if(password.value.trim().length<5)
            {
                alert("password is too short");
                return false;
            }
            else 
            {
                return true;
            }

        }
        
    </script>
</head>
<body>
    <form  onsubmit = "return validate()" action="message.html">

        <input id="uname" placeholder="Username" type="text"/>
        <label id="lbluser" style="color: red;visibility : hidden">Invalid Username
            
        </label>
        <br><br>

        <input id = "pass" placeholder = "password" type="password"/>
        <br><br>

        <button onclick="validate()" type="submit">Submit</button>
    </form>
</body>
</html>

```
>Output:-![image 3]("recent:///a26c91f4df7d86ee8dad2f825fcb9a4a")

# Password Security codes

```c
<!DOCTYPE html>
<html>
<head>
    <title>Regular Expression in JS</title>
    <script type="text/javascript">

        function validate() 
        {
        var username = document.getElementById("uname").value;
        var regx = /E00/; //regular expression in JS is taken as object[They have method assosiated with them]

        if(regx.test(username))
        {
            alert("Valid Username");
        }
        else
        {
            alert("Invalid Username");
            document.getElementById("lbluser").style.visibility ="visible";
        }
    }
    </script>
</head>
<body>
<form action="message.html">

        <input id="uname" placeholder="Username" type="text"/>
        <label id="lbluser" style="color: red;visibility : hidden">Invalid Username
            
        </label>
        <br><br>
        <button onclick="validate()" type="submit">Submit</button>
    </form>
</body>
</html>
```
```c
<!DOCTYPE html>
<html>
<head>
    <title>Regular Expression in JS</title>
    <script type="text/javascript">

        function validate() 
        {
        var username = document.getElementById("uname").value;
        //regx = new RegExp("E00","i");
        //[Another method for regx]

        var regx = /[sdp]imple/;

        /*input are:-   Outputs
            Simple - [valid username]
            dimple - [valid username]
            pimple - [valid username]
            kimple - [Invalid]
            uhfjfd - [Invalid]
            Any thing which does not start with s or d or p here is invalid.
        */


        //var regx = /E00/; 


        var regx = /[a-x A-x]00/;//Any charater betweeen a-x is valid followed by 00



        if(regx.test(username))
        {
            alert("Valid Username");
        }
        else
        {
            alert("Invalid Username");
            document.getElementById("lbluser").style.visibility ="visible";
        }
    }
    </script>
</head>
<body>
<form>

        <input id="uname" placeholder="Username" type="text"/>
        <label id="lbluser" style="color: red;visibility : hidden">Invalid Username
            
        </label>
        <br><br>
        <button onclick="validate()" type="submit">Submit</button>
    </form>
</body>
</html>
```
```c
<!DOCTYPE html>
<html>
<head>
    <title>Regular expression in js</title>
    <script type="text/javascript">



/*   \d - match any digit 
          (equal to [0-9])

     \w - match any other word character 
           (a-z,A-Z,0-9,_)

     \s - match whitespace character 
             (e.g- spaces & tabs)

     \t - match atab only
        /abc/ - only looks for this pattern abc
        but,

        /^abc/ - accepts only abc. not anything of this pattern
     */



        function validate()
        {
            var text = document.getElementById("text1").value;

            var regx = /[7-9]\d{9}/;

            if(regx.test(text))
            {
                document.getElementById("lbltext").innerHTML= "valid";
                document.getElementById("lbltext").style.visibility= " visible";
                document.getElementById("lbltext").style.color= "green";
            }
            else
            {
                document.getElementById("lbltext").innerHTML= "Invalid";
                document.getElementById("lbltext").style.visibility= "visible";
                document.getElementById("lbltext").style.color= "red";
                
            }
        }
    </script>
</head>
<body>
    <form>
    <input id = "text1" placeholder="Cellphone" type="text"/><br>
    <label id="lbltext" style="color: red;visibility : hidden">Invalid
    </label>
    <br>
    <button onclick="validate()" type="button">Submit</button>
    </form>
</body>
</html>
```
```c
<!DOCTYPE html>
<html>
<head>
    <title>Regulaar expression in Js -4</title>
    <script type="text/javascript">

        /*   \d - match any digit 
          (equal to [0-9])

     \w - match any other word character 
           (a-z,A-Z,0-9,_)

     \s - match whitespace character 
             (e.g- spaces & tabs)

     \t - match atab only
        /abc/ - only looks for this pattern abc
        but,

        /^abc/ - accepts only abc. not anything of this pattern
     */


        function validate()
        {
            var text = document.getElementById("text1"). value;

            //var regx = /a.b/ //dot means anything can be enterd between a to b.

            var regx = /^([a-zA-Z0-9\.-]+)@([a-zA-Z0-9-]+).([a-z-z]{2,20})$/;
            //@([a-zA-Z0-9-]+).([a-z]{2,20})$/;
    //   {2 char min},{20 char max}


            /* + is used to extend the string suppose someone has very large username.
              \.- is used to remove the restriction of any number inbetween.
            1. Email starts from name and numbers.
            2. some special characters (    e.g - @,#,*,_)
            3.string of small letters (     e.g - gmail)
            4.In laast extention 
                (e.g - .com,.in)

            */

            if(regx.test(text))
            {
                document.getElementById("lbltext").innerHTML = "valid";
                document.getElementById("lbltext").style.visibility = " visible";
                document.getElementById("lbltext").style.color ="green";
            }
            else
            {
                document.getElementById("lbltext").innerHTML = "Invalid";
                document.getElementById("lbltext").style.visibility = "visible";
                document.getElementById("lbltext").style.color = "red";
            }
        }
    </script>
    </script>
</head>
<body>
    <form>
        <input id="text1" placeholder="Email" type="text"/><br>
        <label id="lbltext" style="color: red; visibility: hidden">Invalid</label><br>
        <button onclick="validate()" type = "button">Submit</button>
    </form>

</body>
</html>
```
# Code to add or Concatenate
```c
<!DOCTYPE html>
<html>
<head>
    <title>add or concatenate</title>
    <script type="text/javascript">
        
        function addvalues()
        {
            var a = document.getElementById("t1").value;
            var b = document.getElementById("t2").value;
            document.getElementById("op").innerHTML = "Result = "+(a+b);
            console.log(a+b); //to see the output on console
        }
    </script>
</head>
<body>
    <input id="t1" type="text" placeholder="Text 1">
    <br><br>
    <input id="t2" type="text" placeholder="Text 2">
    <br><br>
    <button onclick = "addvalues()" id = "output">Add</button>
    <h2 id="op">Result = </h2>
</body>
</html>
```
# Timer using HTML and JS

##### **1.setTimeout()** *allows you to execute statements ONES after an interval*
##### **2.clearTimout()** *method clears a timer seet with the setTimeout() method*
##### **3.setInterval()** *method clears a timer set with the setIntervl() method.*
##### **4.clearInterval()** *method clears a timer set with the setInterval() method*


```c
<!DOCTYPE html>
<html>
<head>
    <title>Timing functions</title>
    <link rel="stylesheet" type="text/css" href="jQuery.css">
    <script type="text/javascript">

        var ID=0;
        var seconds=0;
        function printMsg() 
        {
            //(1.)document.getElementById("op").innerHTML = "5 seconds have passed";

            document.getElementById("op").innerHTML = seconds+ "sec";
            seconds++;
            document.getElementById("op").style.color = "blue";

        }
        function start()
        {
            //(1.)ID=window.setTimeout(printMsg,5000);//5000 is used for 5 sec.

            ID=window.setInterval(printMsg,1000);
        }
        function stop()
        {
            //(1.)window.clearTimeout(ID);//[used to reset the time again]

            window.clearInterval(ID);
        }
    </script>
</head>
<body>
<div id="btnbar1">
    <button onclick="start()" id = "btnAdd"><b>START</b></button>
    <h2 id="op">Some text </h2>
</div>
<div id="btnbar2">
    <button onclick="stop()" id = "btnStop"><b>STOP</b></button>
    <p>click only once</p>
</div>
</body>
</html>
```
# Fade in & Fade out
```c
<!--PURPOUSE OF THIS CODE
    To fade out the pic by 0.1 &
    To fade in the pic by 0.1
-->
<!DOCTYPE html>
<html>
<head>
    <title>Fade in & Fade out</title>
    <script type="text/javascript">
        var opacity =0;
        var intervalID =0;

        function fadeout() 
        {
            intervalID=setInterval(hide,200);
        }
        function hide()
        {
            var img = document.getElementById("img1");
            opacity = Number(window.getComputedStyle(img).getPropertyValue("opacity"));//window lin will also give opacity but it will give it in a string ,therefore to change in number we have to use Number.

            if(opacity>0)
            {
                opacity = opacity -0.1;
                img.style.opacity= opacity;
                console.log(opacity);
            }
            else
            {
                clearInterval(intervalID);
            }
            
        }
        function fadein()
        {
            intervalID= setInterval(show,200);
        }

        function show()
        {
            var img = document.getElementById("img1");
            opacity = Number(window.getComputedStyle(img/*no ivreted comma*/).getPropertyValue("opacity"));
            if(opacity<1)
            {
                opacity= opacity+0.1;
                img.style.opacity = opacity;
                console.log(opacity);
            }
            else
            {
                clearInterval(intervalID);
            }
        }
    </script>
</head>
<body>
    <button id="btnadd" onclick="fadeout()">Fade Out</button>
    <br><br>
    <img id ="img1" style = "opacity: 1"src="https://images.theconversation.com/files/93616/original/image-20150902-6700-t2axrz.jpg?ixlib=rb-1.1.0&q=45&auto=format&w=1000&fit=clip" width = "398px"/>
    <br><br>
    <button id="btnstop" onclick= "fadein()">Fade In</button>
</body>
</html>
```
# Zoom-In And Zoom-out

```c
<!--DOCTYPE html not used-->
<html>
<head>
    <title>basic animation part 2</title>
    <script type="text/javascript">
        
        var width = 100;
        var difference = 2;
        var intervalID = 0;

        function increase()
        {
            intervalID = setInterval(zoomIn,20);
        }

        function zoomIn()
        {
            if(width<200)
            {
                width = width+difference;
                document.getElementById("img1").style.width =width;
                console.log(width);
            }
            else
            {
                clearInterval(intervalID);
            }
        }


        function decrease()
        {
            clearInterval(intervalID);
            intervalID=setInterval(zoomOut,20);
        }

        function zoomOut()
        {
            if(width>100)
            {
                width=width-difference;
                document.getElementById("img1").style.width= width;
                console.log(width);
            }
            else
            {
                clearInterval(intervalID);
            }
        }
    </script>
</head>
<body>
    <br>
    <br>
    <img onmouseover="increase()" onmouseout="decrease()" id="img1" src="https://cnet3.cbsistatic.com/img/pLwWAw3f1OdjhUWe1-u0jcqhIcI=/1200x630/2019/09/10/d3dc3047-4c7f-499e-8b8c-240b3e27c6d2/google-logo-6.jpg" width="200">
</body>
</html>
```
