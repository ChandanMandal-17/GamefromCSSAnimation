# GamefromCSSAnimation
GamefromCSSAnimation: A mini game of sliding window with center ball moving.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AnimationGame</title>
    <style>
        *{
            margin: 0;
            padding: 0;
            box-sizing:border-box;
        }
        .container{
            background-color: rgb(255, 255, 255);
            padding: 10px;
            height: 100vh;
            width: 100vw;
            
        }
        #Box1{

            height: 100px;
            width: 400px;
            background-color: palevioletred;
            margin: 15px;
            padding: 5px;
            position: relative;
            box-shadow: 2px 2px 25px white;
            border-radius: 5px;
            animation-name: box1animate;
            animation-duration: 5s;
            animation-iteration-count: infinite;
            animation-timing-function: ease-in-out;
            animation-delay: 0s;
            animation-direction: alternate;
        }
        #Box2{
            height: 100px;
            width: 400px;
            background-color: palevioletred;
            margin: 15px;
            padding: 5px;
            position: relative;
            box-shadow: 2px 2px 25px white;
            border-radius: 5px;
            animation-name: box2animate;
            animation-duration: 5s;
            animation-iteration-count: infinite;
            animation-timing-function: ease-in-out;
            animation-delay: 0s;
            animation-direction: alternate;
        }
    
        #circle{
            height: 80px;
            width: 80px;
            background-color: palevioletred;
            border-radius: 55px;
            box-shadow: 2px 2px 25px rgb(255, 255, 255);
            animation-name: circleanimate;
            position: relative;
            animation-duration: 10s;
            animation-timing-function: ease-in-out;
            animation-direction: alternate;
            animation-iteration-count: infinite;
            
        }
        @keyframes box1animate {
            from{
                top: 0px;
                left: 0px;

            }
            to{
                top: 0px;
                left: 1450px;

            }
        }
        @keyframes box2animate {
             from{
                top: 680px;
                left: 1450px;

            }
            to{
                top: 680px;
                left:0px  
            }   
        }
        @keyframes circleanimate {
            0%{
                top:-90px;
                left:50px;

            }
            20% {
                top:-90px;
                left:1750px;

            }
            40%{
                top:450px;
                left:150px;
            }
            60%{
                top:450px;
                left:1750px;
            }
            80%{
                top:0px;
                left:1300px;
            }
            100%{
                top:-90px;
                left:50px;
            }
        }
           
    </style>
</head>
<body>
    <div class="container">
        <div id="Box1"></div>
        <div id="Box2"></div>
        <div id="circle"></div>
    </div>
</body>
</html>
