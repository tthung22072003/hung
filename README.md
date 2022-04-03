# code chữ chạy html

// html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css.css">
    <title>Document</title>
</head>
<body>
    <div class="text">T</div>
    <div class="text">R</div>
    <div class="text">O</div>
    <div class="text">N</div>
    <div class="text">G</div>
    <div class="text">H</div>
    <div class="text">U</div>
    <div class="text">N</div>
    <div class="text">G</div>
    <script src="js.js"></script>
</body>
</html>

// css
*{
    padding: 0;
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
body{
    width: 100%;
    height: 800px;
    background-color: #000;
    display: flex;
    justify-content: center;
    align-items: center;
}
.animation{
    color: rgb(0, 0, 0) !important;
    border-radius: 5px;
    text-shadow: 0px 0px 30px #fff,0px 0px 30px #fff,0px 0px 30px #fff,0px 0px 30px #fff;
    box-shadow: 0px 0px 10px #fff,0px 0px 10px #fff,0px 0px 10px #fff;
}
.text{
    font-size: 100px;
    font-weight: 700;
    color: rgb(51, 48, 48);
    margin: 0 20px;
    transition: .5s;
}


// js
var a = 0
var divElement = document.querySelectorAll('.text')
var b = divElement.length
setInterval(function(tthung){
    divElement.forEach(function(tthung){
        tthung.classList.remove('animation')
    })
    divElement[a].classList.add('animation')
    a++
    if(a == b){
        a = 0
    }
}, 350)

