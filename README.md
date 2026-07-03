<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Flower Design</title>
    <style>
      body {
         display: flex;
         justify-content: center;
         align-items: center;
         height: 100vh;
         margin: 0;
         background-color: #f7f9fc;
       }

        .flower {
          position: relative;
          width: 100px;
          height: 100px;
          animation: spin 20s linear infinite;
       }

       .core {
         position: absolute;
         top: 25px;
         left: 25px;
         width: 50px;
         height: 50px;
         background: radial-gradient(circle, #8a1a46 30%, #520926 100%);
         border-radius: 50%;
         z-index: 10;
         box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
       }

       .petal {
         position: absolute;
         top: 0;
         left: 25px;
         width: 50px;
         height: 100px;
         background: linear-gradient(to top, #ff75a0, #ffb3c6);
         border-radius: 50% 50% 50% 50% / 40% 40% 60% 60%;
         transform-origin: center 50px;
         box-shadow: 0 0 10px rgba(225,117,160,0.5);
     }
         </style>
</head>
