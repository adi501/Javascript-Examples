**Reverse of a string**
```
<!DOCTYPE html>
<html>
<head>
    <script>
  function reverse(){
    let input=document.getElementById("inputData").value;
    let output="";
    for(let i=input.length-1;i>=0;i--)
  {
    output+=input[i];
  }
    document.getElementById("output").innerHTML=output;
  }
    </script>
</head>
<body>

<h1>Reverse of a string</h1>
<input type="text" id="inputData" />
<button type="button" onclick="reverse()">Reverse</button>
<h3><U>Output</U></h3>
<p id="output"></p>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/fa233419-1502-450b-a348-8c8d860c48aa)
