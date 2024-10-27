# Ex.05 Design a Website for Server Side Processing
## Date: 27-10-24

## AIM:
To design a website to find surface area of a Right Cylinder in server side.

## FORMULA:
Surface Area = 2Πrh + 2Πr<sup>2</sup>
<br>r --> Radius of Right Cylinder
<br>h --> Height of Right Cylinder

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
    <head>
        <style>
            .box{
                border: 5px solid black;
                border-radius: 20px;
                width: 500px;
                height: 500px;
                background-color: #cacaa4;
                padding: 10px;
                flex-direction: column;
                font-style: inherit;
                
            }
            input[type="text"]{
                font-size: larger;
                font-weight: 300;
                color: black;
                font-style: italic;
                
            }
            input[type="button"]{
                font-size: larger;
                font-weight: 200;
                color: blue;
                font-style: inherit;
            }
            body{
                display: flex;
                align-items: center;
                justify-content: center;
            }


        </style>
        <script>
            function calculatearea(){
                var a=Number(document.getElementById("RADIUS").value);
                var b=Number(document.getElementById("HEIGHT").value);
                if(isNaN(a)||isNaN(b)||a<=0||b<=0){
                    document.getElementById("result").textContent="please enter a valid number!!";
                    return ;
                }
                var surfacearea=2*Math.PI*a*(a+b);
                document.getElementById("result").textContent = "Surface Area =" +surfacearea.
toFixed(2)+"square units";

            }
        </script>

    </head>
    <body background="https://st2.depositphotos.com/2124221/46809/i/450/depositphotos_468095768-
stock-photo-abstract-multicolored-background-poly-pattern.jpg">
        <div class="box">
        <h1 align="center">Surface Area Of a Cylinder</h1>
        <h2 align="center">(M.MANI SRI LATHA - 21222311025)</h2>
        <br><br><br>
        <label><strong>Radius</strong></label><br><br>
        <input type="text" id="RADIUS" placeholder="Radius in units"><br><br>
        <label><strong>Height</strong></label><br><br>
        <input type="text" id="HEIGHT" placeholder="Height in units"><br><br>
        <input type="button" value="Calculate Surfacce Area" onclick="calculatearea()"><br><br>
        <p id="result"></p>
        </div>

    </body>
</html>
```
## HOMEPAGE:
![Screenshot 2024-10-27 233549](https://github.com/user-attachments/assets/04f17465-b8d8-4352-925a-6ef21655e948)


## RESULT:
The program for performing server side processing is completed successfully.
