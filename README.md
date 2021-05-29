# sortNumber
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Number sorter</title>
  </head>
  <style>
   input[type=number], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid rgb(216, 43, 43);
  border-radius: 4px;
  box-sizing: border-box;
}
button {
  width: 100%;
  background-color: green;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
div {
  border-radius: 5px;
  background-color: lightgray;
  padding: 20px;
}
  </style>
  <body>
    <h1>Number Sorter Website</h1>
    <form id="form" action="/homepage.html" method="GET" >
      <div>
        <label for="fInput"> Input first Number</label>
        <input type="number" id="fInput" name="fInput" />
      </div>
      <div>
        <label for="sInput"> Input second Number</label>
        <input type="number" id="sInput" name="sInput" />
      </div>
      <div>
        <label for="tInput"> Input third Number</label>
        <input type="number" id="tInput" name="tInput" />
      </div>
      <label for="foInput"> Input fourth Number</label>
      <input type="number" id="foInput" name="foInput" />
      </div>
      <div>
        <button onclick="myFunction()"> Submit to sort </button>
      </div>
      
    </form>
  </body>
  <script>
    function myFunction() {
    var value = [document.getElementById("fInput").value, document.getElementById("sInput").value, document.getElementById("tInput").value, document.getElementById("foInput").value];
    value.sort(function(a, b) {
     return a - b;
   }); 
     alert(value);
   }


  </script>


</html>
