# Calculator
Simple calculator using html,css,javascript . User can add,subtract,multiply,divide and find the reminder in this calculator.  

CODE:
### HTML,JavaScript
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
    <div class="container">
        <div class="Calculator">
            <form >
                <div class="display">
                    <input type="text" name="display">
                </div>
                <div>
                    <input type="button" value="AC" onclick="display.value=''">
                    <input type="button" value="DC "  onclick="display.value=display.value.toString().slice(0,-1)">
                    <input type="button" value="." onclick="display.value+='.' ">
                    <input type="button" value="/"  onclick="display.value+='/' ">
                </div>
                <div>
                    <input type="button" value="7"  onclick="display.value+='7' ">
                    <input type="button" value="8"  onclick="display.value+='8' ">
                    <input type="button" value="9"  onclick="display.value+='9' ">
                    <input type="button" value="*"  onclick="display.value+='*' ">
                </div>
                <div>
                    <input type="button" value="4"  onclick="display.value+='4' ">
                    <input type="button" value="5"  onclick="display.value+='5' ">
                    <input type="button" value="6"  onclick="display.value+='6' ">
                    <input type="button" value="-"  onclick="display.value+='-' ">
                </div>
                <div>
                    <input type="button" value="1"  onclick="display.value+='1' ">
                    <input type="button" value="2"  onclick="display.value+='2' ">
                    <input type="button" value="3"  onclick="display.value+='4' ">
                    <input type="button" value="+"  onclick="display.value+='+' ">
                </div>
                <div>
                    <input type="button" value="00"  onclick="display.value+='00' ">
                    <input type="button" value="0"  onclick="display.value+='0' ">
                    <input type="button" value="="  onclick="display.value = eval(display.value)">
                    <input type="button" value="%" onclick="display.value+='%' ">
                </div>
            </form>
        </div>
    </div>
    
</body>
</html>
```
### CSS
```
*{
    margin: 0;
    padding: 0;
    font-family: 'Poppins',sans-serif;
    box-sizing: border-box;
}

.container{
    width: 100%;
    height: 100vh;
    background: #81daf2;
    display: flex;
    align-items: center;
    justify-content: center;
}
.Calculator {
    background: #3a4452;
    padding: 20px;
    border-radius: 10px;
}
.Calculator form input{
    border: 0;
    width: 69px;
    height: 69px;
    box-shadow: -8px -8px 15px rgba(255,255,255,0.1),5px 5px 15px rgba(0,0,0,0.2);
    background: transparent;
    font-size: 22px;
    color: #fff;
    cursor: pointer;
    margin: 10px;
}
form .display{
    display: flex;  
    justify-content: flex-end;
    margin  :20px  0;   
}
form .display input{
    text-align: right;
    flex: 1;
    font-size: 45px;
}
```
### Output
![image](https://github.com/VisHinu24/Calculator/assets/144244396/131dd520-c57f-49d0-982c-fd2571a2744d)

