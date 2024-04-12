# Ex04 Places Around Me
## Date: 12-04-2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    *{
        margin:0
    }
</style>
<script>
    function coordinate(event){
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("text1").value = x;
        document.getElementById("text2").value = y;

    }
</script>
<center>
<body style="padding-top: 090px;">
    <img  src="map.png" width="1000" height="500" usemap="#MapNew" onmousemove="coordinate(event)">
    <map name="MapNew">
        <area shape="RECT" coords="223,33,310,55" href="https://apolloartsandsciencecollege.ac.in/admission.html" title="Apollo Arts and Science ">
        <area shape="RECT" coords="314,224,430,250" href="https://rajalakshmi.org/" title="RAJALAKSHMI Engineering College">
        <area shape="RECT" coords="300,105,420,120" href="https://saveetha.ac.in/300,105,420,120" title="Saveetha Engineering College">
        <area shape="RECT" coords="575,475,675,495" href="https://www.citchennai.edu.in/" title="Chennai Institute of Technology ">
        <area shape="RECT" coords="512,120,604,131" href="https://www.lit.edu.in/" title="Loyola Institute of Technology">
        <area shape="RECT" coords="593,20,708,43" href="https://ritchennai.org/" title="RAJALAKSHMI Institute of Technology">

    </map>
    <br>
    X-coordinate
    <input type="text" id="text1">
    <br>
    Y-coordinate
    <input type="text" id="text2">
</body>
</center>
</html>
```


## OUTPUT

![Screenshot 2024-04-12 093949](https://github.com/gururaghav2925/NearMe/assets/151489500/063123d0-32c5-4558-a73e-1545c52e8a8f)





## RESULT
The program for implementing image maps using HTML is executed successfully.
