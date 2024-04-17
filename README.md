# Ex04 Places Around Me
## Date: 

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
`````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<script>
    function coordinate(event)
    {
        
        let x = event.clientX;
        let y = event.clientY;
    
        document.getElementById("X").value = x;
        document.getElementById("Y").value = y;
    }
</script>
<body>
    <IMG src ="map.png" width="600" height="230" usemap="#MapNew" onmousemove="coordinate(event)">
    <MAP name="MapNew">
        <AREA shape="RECT" coords="140,45,250,75" herf="https://apolloartsandsciencecollege.ac.in/admission.html" Title="Apollo Arts and Science">
        <AREA shape="RECT" coords="335,102,470,130" herf="https://www.saveetha.ac.in/" Title="Saveetha Engineering College">
        <AREA shape="RECT" coords="480,47,575,75" herf="https://paytm.com/movies/chennai/evp-cinemas-chennai-c/1024343" Title="EVP cinemas">
    </MAP> <br>
    X-coordinate <input type="text" id="X"> <br>
    Y-coordinate <input type="text" id="Y"> <br>
</body>
</html>
`````


## OUTPUT

![Screenshot 2024-04-17 142659](https://github.com/iamyadhav/NearMe/assets/147139713/cf5c7dfa-4da3-4e4c-9997-1df0f9c1f87b)






## RESULT
The program for implementing image maps using HTML is executed successfully.
