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

        /* Rotations to create petal layers */
        .p1 { transform: rotate(0deg); }
        .p2 { transform: rotate(45deg); }
        .p3 { transform: rotate(90deg); }
        .p4 { transform: rotate(135deg): }
        .p5 { transform: rotate(180deg); }
        .p6 { transform: rotate(225deg); }
        .p7 { transform: rotate(270deg); }
        .p8 { transform: rotate(315deg); }   

        @keyframes spin {
          100% { transform: rotate(360deg); 
        }
      </style>
      </head>
      <body>

      <div class="flower">
        <div class="core"></div>
        <!-- 8 Petals -->
        <div class="petal p1"></div>
        <div class="petal p2"></div>
        <div class="petal p3"></div>
        <div class="petal p4"></div>
        <div class="petal p5"></div>
        <div class="petal p6"></div>
        <div class="petal p7"></div>
        <div class="petal p8"></div>
      </div>

      </body>
      </html>
