# Ex.08 Design of Interactive Image Gallery
## Date: 16.10.2024

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
    <head>
        <style>
            .container{
                background-image:url(bg2.png);
                background-repeat: no-repeat;
                background-size: cover;
                background-image: center;
                width:100%;
                height:100%;
                position: relative;

            }
            .font-color{
                color:rgba(0, 255, 255, 0.684);
                font-size:45px;
                font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
            }
            .soft{
                background-image: url(soft.png);
                align-items: center;
                background-repeat: no-repeat;
                margin-left: 750px; 
                position: relative; 
            }
            .women{
                background-image: url(women.png);
                background-repeat: no-repeat;
                margin-left: 905px;
                position: relative;
               
            }
            .flower{
                background-image: url(flower.png);
                background-repeat: no-repeat;
                margin-left: 1030px;
                position: relative;

            }
            .pic{
                background-image: url(pic1.png);
                align-items: right;
                background-repeat: no-repeat;
                margin-left: 750px; 
                
                bottom: 890px;
                position: relative;
                left: 500px;
                
            }
            .eye{
                background-image: url(eye.png);
                position: relative;
                background-repeat: no-repeat;
                bottom: 910px;
                left: 1415px;
            }
            .tile{
                background-image: url(tile.png);
                position: relative;
                background-repeat: no-repeat;
                bottom: 2500px;
                left: 1325px;
            }
            .background{
                background-image: url(bg.png);
                position: relative;
                background-repeat: no-repeat;
                bottom: 3000px;
                left: 1485px;
                top: -2505px;
                
            }
            .soft:hover, .women:hover, .flower:hover, .pic:hover, .eye:hover, .tile:hover, .background:hover {
                transform: scale(1.1);}
        </style>
        <body>
            <main>
                <div class="container">
                    <div class="font-color">
                        <h1 align=center>Interactive Image Gallery</h1>
                        <hr>
                        <h4 align="center">Designed and Developed by Indhu Priya.T</h4>
                        <div>
                            <div class="soft" onclick="toggleVisibility('soft')">
                                <img src="soft.png" alt="soft image" width="600px" height="700px"/>
                            </div>
                            <div class="women" onclick="toggleVisibility('women')">
                                <img src="women.png" alt="women image" width="500px" height="400px"/>
                            </div>
                           <div class="flower" onclick="toggleVisibility('flower')">
                            <img src="flower.png" alt="flower image" width="600px" height="400px" />
                           </div>
                           <div class="pic" onclick="toggleVisibility('pic')">
                            <img src="pic1.png" alt="pic image" width="300px" height="300px" />
                           </div>
                           <div class="eye" onclick="toggleVisibility('eye')">
                            <img src="eye.png" alt="eye image" width="500px" height="700px" />
                           </div>
                           <div class="tile" onclick="toggleVisibility('tile')">
                            <img src="tile.png" alt="tile image" width="600px" height="600px" />
                           </div>
                           <div class="background" onclick="toggleVisibility('background')">
                            <img src="bg.png" alt="background image" width="900px" height="460px" />
                           </div>
                        </div>
                    </div>
                    
                   
                </div>

            </main>
           <script>
             function toggleVisibility(imageClass) {
            const imageElement = document.querySelector(`.${imageClass}`);
            const isHidden = imageElement.style.opacity === '0';
            imageElement.style.transition = 'opacity 0.3s ease';
            imageElement.style.opacity = isHidden ? '1' : '0'; 
        }

        
        function changeBackgroundColor() {
            const container = document.getElementById('container');
            const currentColor = container.style.backgroundColor;

            
            if (currentColor === 'rgb(255, 255, 255)') {
                container.style.backgroundColor = 'rgba(0, 0, 0, 0.6)';
            } else {
                container.style.backgroundColor = 'rgba(255, 255, 255, 0.7)';
            }
        }
           </script>
        </body>
    </head>
</html>
```

## OUTPUT:
![alt text](<images/imageapp/static/Screenshot (51).png>)
![alt text](<images/imageapp/static/Screenshot (52).png>)
![alt text](<images/imageapp/static/Screenshot (53).png>)
![alt text](<images/imageapp/static/Screenshot (54).png>)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
