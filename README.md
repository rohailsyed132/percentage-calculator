   <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Document</title>
   <style>
      html, body {
         display: flex;
         flex-direction: column;
         align-items: center;
         text-align: center;
         justify-content: center;
         height: 100vh;

      }
   </style>
   

 </head>
 <body>
   <h1>Percentages</h1>
   <h2>what is <input class="x"> % of <input class="y"> <button class="one">calculate</button> = <input class="z"readonly> </h2>
     
   <h2><input class="f"> is what percent of <input class="g"> <button class="two">calculate</button> = <input class="h"readonly>  </h2>
      
   <h2>what is the percentage increase/decrease from <input class="v"> to <input class="b"> <button class="three">calculate</button> = <input class="n" readonly> </h2>
      
       <script>
         document.querySelector(".one").addEventListener("click",waitforclick);
         function waitforclick(){
            var x=parseFloat(document.querySelector('.x').value);
            var y=parseFloat(document.querySelector('.y').value);
            document.querySelector('.z').value=(x*y)/100
         };
      </script>
      <script>
         document.querySelector(".two").addEventListener("click",wait);
         function wait(){
            var f=parseFloat(document.querySelector('.f').value);
            var g=parseFloat(document.querySelector('.g').value);
            document.querySelector('.h').value=(f/g)*100
         };
   
      </script>
       <script>
         document.querySelector(".three").addEventListener("click",wait2);
         function wait2(){
            var v=parseFloat(document.querySelector('.v').value);
            var b=parseFloat(document.querySelector('.b').value);
            document.querySelector('.n').value=(b-v)/v*100
         };
   
      </script>
 </body>
 </html>
