
 <html>
     <head>
    <title>Ascending Numbers</title> 
    <style>
        body {
            background-image: url("https://img.freepik.com/free-vector/beige-leafy-watercolor-background-vector_53876-136491.jpg?size=626&ext=jpg&ga=GA1.1.735520172.1710892800&semt=ais");
            background-repeat: no-repeat;
            background-size: cover;
            background-attachment: fixed;
            text-align: center;
            font-family: 'Times New Roman', Times, serif;
            font-size: 2.4rem;
            border-style: groove;
            border-width: 5px;
            padding: 5%;
            cursor: pointer;
            position: relative;
            outline: none;
        }
    
        
        
    
        
        h1 {
            font-style: italic;
            font-size: 5rem;
            color: rgb(59, 7, 37);
            text-indent: 10%;
            word-spacing: 2rem;
            transition: 2ms;
        }
        
        
        p {
            word-spacing: 2px;
           font-weight: bold;
           
           font-size: 1.5rem;
        }
        

        </style> 

     </head> 

    <body>
    
    <h1>Ascending Numbers</h1>

    <p>Enter an integer greater than 0:</p>

    <input type="number" id="inputNumber"> 
  
    <button onclick="displayAscendingNumbers()">Display Ascending Numbers</button> 

    <div class="output" id="output">

    </div>
   
     <script> 

     function displayAscendingNumbers()

     { var inputNumber = document.getElementById("inputNumber").value;

      var output = document.getElementById("output"); output.innerHTML = "";

    if (inputNumber > 0) 

    { for (var i = 1; i <= inputNumber; i++)

    { var span = document.createElement("span"); span.textContent = i + " "; 

    output.appendChild(span); } } 

    else { output.textContent = "Please enter a valid integer greater than 0."; } } 

    </script>

     </body> 

     </html>
