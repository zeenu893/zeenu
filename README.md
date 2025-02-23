<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="card">
            <div class="outside">
                <h1>Happy m</h1>
                <h3>My dear best friend,may god bless you with abundant joy on your birthday and always!<br>
                    Thank you for always being by my side and having my back.</h3>
            </div>
            <div class="inside">
                <img src="cakegif.gif"/>
                <h3>Sending you an infinite amount of love, joy, and happiness on your birthday!
                </h3>
            </div>
        </div>

        <div class="block">
            <div class="frames frame1">
                <img src="img1.png" alt="">
                <p>Keep smiling,Keep shining</p>
            </div>
            <div class="frames frame2">
                <img src="img2.png" alt="">
                <p>On this occasion bring you lot of happiness and success
                </p>
            </div>
            <div class="frames frame3">
                <img src="img3.png" alt="">
                <p>May God bless you on your birthday, and always</p>
            </div>
        </div>

    </div>
</body>
</html> 
@import url('https://fonts.googleapis.com/css2?family=Bodoni+Moda:ital@1&display=swap');
*{
    padding: 0;
    margin: 0;
    font-family: 'Bodoni Moda', serif;
}
body{
    height: 100vh;
    background: linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.5)),url(bday.gif);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.container{
    perspective: 1000px;
}
.card{
    width: 280px;
    height: 360px;
    position: absolute;
    top: 100px;
    left: 230px;
    transition: 2s;
    transform-style: preserve-3d;
}
.card:hover{
    transform: rotateY(180deg);
}
.block{
    position: absolute;
    top:200px;
    right: 600px;
    perspective: 800px;
}
.outside,.inside{
    width: 100%;
    height: 100%;
    border-radius: 20px;
    text-align: center;
    padding: 1.5rem;
}
.outside{
    background-color: blanchedalmond;
    box-shadow: inset 0 5px 10px rgba(0,0,0,0.5);
    position: absolute;
    backface-visibility: hidden;
}
.outside h1{
    font-size: 3rem;
    font-weight: bold;
    color: salmon;
    margin-bottom: 30px;
}
.inside{
    background-color: rgb(255, 244, 79);
    box-shadow: inset 0 5px 10px rgba(0,0,0,0.5);
    transform: rotateY(180deg);
}
.inside h3{
    font-size: 1.2rem;
    font-weight: bold;
    margin-top: 20px;
}
.frames{
    width: 400px;
    height: 150px;
    box-shadow: 0 5px 10px rgba(255, 255, 255, 0.5);
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 0 0.8rem;

    transform: rotateY(-230deg) rotateX(20deg);
    position: absolute;
}
.frames img{
    width: 125px;
    height: 125px;
    border-radius: 50%;
    box-shadow: 0 5px 10px rgba(0,0,0,0.5);
}
.frames p{
   font-size: 20px;
   font-weight: bold;
   transform: rotateY(180deg);
}
.frames:nth-child(1)
{
    top:-110px;
    z-index: -1;
    background-color: coral;
}
.frames:nth-child(2){
    background-color: goldenrod;
}
.frames:nth-child(3)
{
    top:100px;
    background-color: burlywood;
}
