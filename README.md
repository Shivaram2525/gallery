# Ex-7: Interactive Image Gallery
## Date: 12-11-2024

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <link rel="stylesheet" href="gallery.css">
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div id="image">Hover over an image below to display here.</div>
    
    <div class="gallery">
        <img class = "preview" alt = "Sky_1" src = "Sky_1.jpeg" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "Sky_2" src = "Sky_2.jpeg" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "Sky_3.jpeg" alt = "Sky_3" onmouseover = "upDate(this)" onmouseout = "unDo()">
        <img class = "preview" alt = "Sky_4" src = "Sky_4.jpeg" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "Sky_5" src = "Sky_5.jpeg" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "Sky_6.jpeg" alt = "Sky_6" onmouseover = "upDate(this)" onmouseout = "unDo()">
    </div>
    <script src="gallery.js"></script>
</body>
</html>
```

### gallery.css
```
body{
    margin: 2%;
    border: 1px solid black;
    background-color: #b3b3b3;
}
#image{
line-height:650px;
    width: 575px;
height: 650px;
    border:5px solid black;
    margin:0 auto;
background-color: #8e68ff;
background-image: url('');
background-repeat: no-repeat;
color:#FFFFFF;
text-align: center;
background-size: 100%;
margin-bottom:25px;
font-size: 150%;
}
.preview{
    width:10%;
    margin-left:17%;
border: 10px solid black;
}
img{
    width:95%;
}
```

### gallery.js
```
const imageDiv = document.getElementById('image');
const originalImageUrl = '';
const originalText = "Hover over an image below to display here.";

function upDate(previewPic) {
    imageDiv.style.backgroundImage = `url('${previewPic.src}')`;
    
    imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
    imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; 
    
    imageDiv.innerHTML = originalText;
}
```
## WEBSITE URL:
```
https://codepen.io/Shivaram-M/pen/GRVPeyo
```
## OUTPUT:

<img width="1680" alt="Javascript_6" src="https://github.com/user-attachments/assets/5c9e4a06-ce35-4350-b5da-e0e0bea12164">

<img width="1680" alt="Javascript_4" src="https://github.com/user-attachments/assets/cd7f8428-4be4-4944-bc16-54414da2ce0f">

<img width="1680" alt="Javascript_5" src="https://github.com/user-attachments/assets/b736c3c8-93f6-4dc0-bd06-26955a9b79d5">

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
