# Ex04 Places Around Me
# Date:04/12/2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
```
MAIN.PAGE:
<html>
    <head>
        <title>
            UNITED KINGDOM
        </title>
    </head>
    <style>
     .img{
       margin-left: 15%;
       width: 70%;
       height: 65%;
      
     }
    
     .tit1{
        font-size: 100px;
        text-align: center;
       

     }
     .tit2{
        font-size: 40px;
        text-align: center;
       
     }
     .tit1:hover{
        cursor: default;
     }.tit2:hover{
        cursor: default;
     } 
     body{
      color: grey;
     }

    </style>
    <body  >
        <div class="tit1">UNITED KINGDOM</div>
        <div class="tit2"> POPULAR PLACES</div><br><br>
        {% load static %}
        <img src={% static 'images/Imagemap.png' %} style="margin-left: 30%;"  usemap="#imagemap"  >
        <map name="imagemap">
         <area shape="poly" coords="171,75,388,71,412,168,155,171" title="Manchester" href="C:\Users\admin\Desktop\HTML\manchester.html">
         <area shape="poly" coords="80,220,258,258,199,389,7,357" title="Wales" href="C:\Users\admin\Desktop\HTML\wales.html">
         <area shape="poly" coords="539,259,300,287,269,413,476,409" title="london" href="C:\Users\admin\Desktop\HTML\london.html">
      </map>  



   
</body>
</html>

1ST PAGE:

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>London</title>
</head>

    
    <style>
       
        img{
            height: 450px;
            
        }
       
        DIV{
          
            color:orange;
           
            font-size: 70px;
            
        }
        p{
           color: orange;
        }
        
        footer{
          color: orange;
        margin-left:75%;
        margin-top: 30px;
    }
  
   
    </style>
    <body style="background-color:blue">

    <center>

    <div>LONDON:TOWER BRIDGE</div><br>
    <hr>
    {% load static%}
    <img src={% static 'images/tower-bridge.jpg' %} width="1300px" ><br>
    <hr>
    <p>

           
         Tower Bridge is one of London's most iconic landmarks, combining elements of both a bascule and suspension bridge. Completed in 1894, it was 
         designed to ease road traffic while still allowing ships to pass along the Thames. Its Victorian Gothic architecture, featuring two majestic 
         towers connected by walkways, has made it a beloved symbol of the city. The bridge's bascule sections, which can be raised to permit river
          traffic, are powered by a combination of hydraulic mechanisms that originally used steam engines, later modernized to use electricity and oil.
           Visitors can explore the bridge's history and engineering marvels through its exhibition, which includes a glass-floored walkway offering 
           stunning views of London from above. Whether you're admiring its architecture, 
         walking across it, or exploring its exhibition, Tower Bridge offers a fascinating glimpse into both London's past and its engineering prowess.
    <br>
  
The London Eye, also known as the Millennium Wheel, is a massive Ferris wheel on the South Bank of the River Thames in London. Standing at 135 meters tall, it was the world's tallest Ferris wheel when it opened in 2000. Each of its 32 capsules can hold up to 25 people, offering breathtaking panoramic views of the city's skyline. The London Eye has become an iconic symbol of modern London and is one of the most popular tourist attractions in the United Kingdom. Whether day or night, a ride on the London Eye provides an unforgettable perspective of the city's landmarks.


    
    
    <hr></p></center>
</body>
<footer>
    @COPYRIGHT by Tower_bridge-2024.
</footer>
</html>
2ND PAGE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manchester</title>
</head>

    
    <style>
        DIV{
          
            color:brown;
           
            font-size: 70px;
            
        }
        img{
            height: 450px;
            width: 1300px;
        }
        footer{
            margin-left: 75%;
            margin-top: 10px;
        }
        p{
            color: brown;
        }
       
    </style>
    <body style="background-color:blanchedalmond;">

    <center>

    <div> MANCHESTER : BISHOP'S MOVE</div><br>
    <hr>
    <br>
    {% load static %}
    <img src={% static 'images/manchester.png' %} alt="Bishop move"><br>
    <br><hr><p >
           
        The bishop is a versatile piece in chess, known for its ability to move diagonally across the board. Unlike some other pieces, the bishop is unrestricted by the number of squares it can travel in a single move. As long as its path isn't obstructed by another piece, the bishop can cover a great distance, making it a powerful tool for controlling long diagonals. Each bishop starts on a specific color, either light or dark, and remains on that color throughout the game, which often shapes its strategic importance. Bishops work particularly well in pairs, complementing each other by covering both sets of diagonals. This dynamic often makes them valuable assets in endgames and open positions. Effective use of bishops involves leveraging their range and mobility to exert pressure on the opponent's position.
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat cupiditate ab molestiae expedita labore pariatur, vel libero provident officia perspiciatis, nemo aliquam dolore ipsum commodi consequatur laudantium corporis fugit tempora.
    <hr></p>

    </center>
</body>
<footer>
    @COPYRIGHT by Bishop's_move-2024.
</footer>
</html>
3RD PAGE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wales</title>
</head>

    
    <style>
       
        div{
            color: cyan;
           display: inline;
            font-size: 70px;
            
        }
        img{
            height: 450px;
            width: 1300px;
        }
        footer{
            margin-left: 75%;
            margin-top: 20px;
        }
        body{
            overflow: hidden;
        }
       
    </style>
    <body style="background-color:crimson;">

    <center>

    <div >WALES:</div> 
    <div>CADRIFF CASTLE</div><br>
    <hr><br>
  {% load static%}
    <img src={%static 'images/walescastle.jpg' %} alt="cadriff castle image" ><br>
    <br><hr>
    <p>
        <center>
            Cardiff Castle, located in the heart of Cardiff, Wales, is a striking example of medieval architecture with an extensive history that spans over 2,000 years. Originally built as a Roman fort, the site has seen numerous transformations, most notably under the ownership of the Norman invaders in the 11th century and the Bute family in the 19th century. The Bute family's influence led to the castle's Victorian Gothic revival, designed by architect William Burges, resulting in the stunningly ornate interiors and impressive clock tower that visitors see today. Cardiff Castle not only serves as a historical monument but also as a cultural hub, hosting a variety of events, exhibitions, and tours, making it a must-visit landmark rich with stories of the past.<br>

    
         Lorem ipsum dolor sit amet consectetur, adipisicing elit. Molestias fugiat esse natus nihil blanditiis sed sunt ab voluptatum labore itaque maiores nulla repellendus optio, eveniet ratione odio? Architecto, fuga beatae. From the legendary fields of the FIFA World Cup to local street games, football is a mix of talent, strategy, and pure passion. The sport boasts iconic players like Pelé, Diego Maradona, Lionel Messi, and Cristiano Ronaldo, whose careers have inspired generations.
       Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum dolor nesciunt libero ullam voluptas doloremque numquam quam, hic soluta! Error? 
    <br>

        
        
       <hr>
    </center>
    
</body>
<footer>
    @COPYRIGHT by cadriff_castle-2024.
</footer>
</html>
```
# OUTPUT
![output04(web)i](https://github.com/user-attachments/assets/91ed1c94-73e9-4153-b3ad-f8dd676b1e28)
![output04(web)ii](https://github.com/user-attachments/assets/a8d35444-b7c6-43ce-88a0-5969f09209cf)
![output04(web)iii](https://github.com/user-attachments/assets/066046e6-0d6f-4d69-82a8-2455b8f83ba7)
![output04(web)iv](https://github.com/user-attachments/assets/55249133-d630-4196-abad-9c0a81f7897c)

# RESULT
The program for implementing image maps using HTML is executed successfully.
