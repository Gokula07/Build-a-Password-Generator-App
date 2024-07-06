# Build-a-Password-Generator-App
<!-- index.html  -->
<!DOCTYPE html> 

<html lang="en"> 

  

<head> 

    <meta charset="UTF-8" /> 

    <meta name="viewport" 

          content="width=device-width,  

                   initial-scale=1.0" /> 

    <link rel="stylesheet" href="style.css" /> 

    <title>Password Generator</title> 

</head> 

  

<body> 

    <h1>Password Generator</h1> 

    <div class="generator"> 

        <div class="password"> 

            <input type="text" value="test" /> 

            <button>copy</button> 

        </div> 

        <div class="range"> 

            <input type="range" min="4" 

                   max="24" value="8" /> 

            <span>8</span> 

        </div> 

        <div class="options"> 

            <div class="option"> 

                <label> 

                    <input type="checkbox" 

                           id="lowercaseCb" checked /> 

                    <span>a-z</span> 

                </label> 

            </div> 

            <div class="option"> 

                <label> 

                    <input type="checkbox" 

                           id="uppercaseCb" /> 

                    <span>A-Z</span> 

                </label> 

            </div> 

            <div class="option"> 

                <label> 

                    <input type="checkbox" 

                           id="digitsCb" /> 

                    <span>0-9</span> 

                </label> 

            </div> 

            <div class="option"> 

                <label> 

                    <input type="checkbox" 

                           id="specialsCb" /> 

                    <span>!@$#%^</span> 

                </label> 

            </div> 

        </div> 

        <button class="generate"> 

            generate 

        </button> 

    </div> 

    <script src="script.js"></script> 

</body> 

  

</html>
/* style.css */

@import url( 

"https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap"); 

  
body { 

    background-color: #f8f8f8; 

    color: #333; 

    font-family: "Roboto Mono", monospace; 
} 

  
.generator { 

    background-color: #f5f5f5; 

    width: 250px; 

    margin: 150px auto; 

    padding: 20px; 

    border-radius: 10px; 
} 

  
div.password { 

    display: grid; 

    grid-template-columns: auto min-content; 

    border-radius: 10px; 

    overflow: hidden; 
} 

  
div.password input { 

    padding: 7px 10px; 

    background-color: #ddd; 

    border: 0; 

    color: #333; 
} 

  
button { 

    background-color: #4caf50; 

    color: #fff; 

    text-transform: uppercase; 

    padding: 5px 15px; 

    border: 0; 

    border-radius: 10px; 
} 

  
div.password button { 

    border-radius: 0; 
} 

  
div.range { 

    margin: 10px 0; 

    display: grid; 

    grid-template-columns: 1fr min-content; 
} 

  
div.range span { 

    background-color: #ddd; 

    padding: 10px; 

    margin-left: 20px; 

    min-width: 30px; 

    text-align: center; 

    border-radius: 10px; 
} 

  
div.options { 

    display: grid; 

    grid-template-columns: 1fr 1fr; 

    gap: 10px; 
} 

  
div.options label { 

    display: block; 

    background-color: #ddd; 

    padding: 10px; 

    border-radius: 10px; 

    cursor: pointer; 

    font-family: sans-serif; 
} 

  
button.generate { 

    width: 100%; 

    margin-top: 10px; 

    padding: 10px; 
} 

  

h1 { 

    text-align: center; 

    color: #4caf50; 
}
