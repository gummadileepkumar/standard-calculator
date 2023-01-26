# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.


### Step 2:
Change settings.py file to allow request from all hosts.


### Step 3:
Use CSS for creating attractive colors


### Step 4:
Write JavaScript program for implementing five different operations.



### Step 5:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```html
<!DOCTYPE html>
<HTML lang="en">
    <head>
        <title>Calculator</title>
        
        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>

        <style>
            h1{
                color: white;
            }



            
            .calculator-container {
                width: 400px;
                background-color: white;
                margin: 0 auto; 
                text-align: center;
                
            }

           
            button {
                width: 50px;
                height: 50px;
                margin: 10px; 
                font-size: 20px; 
                
                background-color: white; 
                color: black; 
                border: none;
            }

          
            #result {
                
       background-color:#ABFFBA;
    text-align: right;
    padding-right: 50px;
    font-size: 20px;
    margin-bottom: 20px; 
    border: solid black 0.5px;
    color: black;
    width: 348px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 5px;
                color: black;
            }
            .redd {
                background-color: brown;
            }
            .bluee {
                
                background-color: cornflowerblue;
            }
            body {
                background-color: black;
            }
        </style>

    </head>
<body>
    <div class="calculator-container">
        <h1>CALCULATOR</h1>
        <div id="result">0</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">√ </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </body>
    </HTML>
```
## OUTPUT:
![calc1_output](https://user-images.githubusercontent.com/118707761/214777500-c03417be-8b62-4d0d-b054-a93ce243cfbd.png)
![calc2_output](https://user-images.githubusercontent.com/118707761/214777532-1fe00aee-c13b-4821-818e-59bcccc6c9b0.png)
![calc3_output](https://user-images.githubusercontent.com/118707761/214777588-b9feef58-666d-4d2e-be70-a80025e54359.png)
## HTML VALIDATION:




![Screenshot (56)](https://user-images.githubusercontent.com/118707761/214778203-f50400b8-2734-4b14-9532-bfbfa85ef506.png)


## Result:
The program for designing a simple calculator using JavaScript css and html is executed successfully.

