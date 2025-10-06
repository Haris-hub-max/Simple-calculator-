<!DOCTYPE html>
<html>
<head>
  <title>Simple Calculator</title>
  <style>
    #calculator {
      width: 300px;
      margin: 50px auto;
      padding: 20px;
      border: 1px solid #ccc;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    #display {
      width: 100%;
      height: 40px;
      margin-bottom: 20px;
      padding: 10px;
      border: none;
      border-radius: 10px;
      font-size: 24px;
      text-align: right;
    }
    .button {
      width: 60px;
      height: 40px;
      margin: 5px;
      padding: 10px;
      border: none;
      border-radius: 10px;
      background-color: #f0f0f0;
      cursor: pointer;
    }
    .button:hover {
      background-color: #e0e0e0;
    }
  </style>
</head>
<body>
  <div id="calculator">
    <input type="text" id="display" disabled>
    <div>
      <button class="button" onclick="document.getElementById('display').value=''">C</button>
      <button class="button" onclick="document.getElementById('display').value = document.getElementById('display').value.slice(0, -1)">DEL</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '7'">7</button>
      <button class="button" onclick="document.getElementById('display').value += '8'">8</button>
      <button class="button" onclick="document.getElementById('display').value += '9'">9</button>
      <button class="button" onclick="document.getElementById('display').value += '/'">/</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '4'">4</button>
      <button class="button" onclick="document.getElementById('display').value += '5'">5</button>
      <button class="button" onclick="document.getElementById('display').value += '6'">6</button>
      <button class="button" onclick="document.getElementById('display').value += '*'">*</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '1'">1</button>
      <button class="button" onclick="document.getElementById('display').value += '2'">2</button>
      <button class="button" onclick="document.getElementById('display').value += '3'">3</button>
      <button class="button" onclick="document.getElementById('display').value += '-'">-</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '0'">0</button>
      <button class="button" onclick="document.getElementById('display').value += '.'">.</button>
      <button class="button" onclick="document.getElementById('display').value = eval(document.getElementById('display').value)">=</button>
      <button class="button" onclick="document.getElementById('display').value += '+'">+</button>
    </div>
  </div>
</body>
</html>

