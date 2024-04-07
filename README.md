# Ex04 Places Around Me
## Date: 07.04.2024

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
### index.html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Map</title>
</head>
<body>
    <img src="assets/css/images/image.png" width="1000px" usemap="#MapNew" onmousemove="coord(event)">
    <Map name="#MapNew">
        <AREA shape="RECT" coords="600,150,700,190" href="https://www.svrcc.in/" title="Swami Vivekanda Rural Community ">
        <AREA shape="RECT" coords="500,290,600,300" href="http://www.smasc.edu.in/index.php"  title="Sri Muthukumaran Arts and Science College">
        <AREA shape="RECT" coords="750,100,650,100" href="http://www.saintthomascollege.com/" title="St.Thomas College of Arts and Science">
        <AREA shape="RECT" coords="800,70,950,70" href="https://donboscocollege.ac.in/" title="Don Bosco College">
        <AREA shape="RECT" coords="750,300,890,330" href="https://hcaschennai.edu.in/" title="Hindustan College of Arts and Science College">
    </Map>
    <br>
    x Coord : <input type="text" name="" id="txt1"><br>
    y Coord : <input type="text" name="" id="txt2">
</body>
<script>
    function coord(event)
    {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById('txt1').value=x;
        document.getElementById('txt2').value=y;
    }
</script>
</html>
```


## OUTPUT
![output](https://github.com/Aishwarya-TM/Web-EX4/assets/127846109/f89a1b88-334a-4ee5-b602-c586cfccaab0)



## RESULT
The program for implementing image maps using HTML is executed successfully.
