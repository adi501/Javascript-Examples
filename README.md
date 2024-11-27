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

**Longest word in the sentence**
```
<!DOCTYPE html>
<html>
<head>
    <script>
  function Find(){
    let input=document.getElementById("inputData").value;
    let output="";
    let outputlength=0;
    const words=input.split(" ");
    for(let i=0;i<words.length;i++)
  {
    if(outputlength<words[i].length)
  {
    outputlength=words[i].length;
    output=words[i];
  }
  }
    document.getElementById("output").innerHTML=output;
  }
    </script>
</head>
<body>

<h1>Longest word in the sentence</h1>
<input type="text" id="inputData" />
<button type="button" onclick="Find()">Find</button>
<h3><U>Output</U></h3>
<p id="output"></p>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/5ae73b5c-c24b-4bfb-ba90-a17868dcf1b8)

**Palindrome or not**
```
<!DOCTYPE html>
<html>
<head>
    <script>
  function Find(){
    let input=document.getElementById("inputData").value;
    let output="";
    for(let i=input.length-1;i>=0;i--)
  {
    output+=input[i];
  }
if(input==output)
{
    document.getElementById("output").innerHTML="given string is Palindrome";
}
else
{
    document.getElementById("output").innerHTML="given string is Not Palindrome";
}
  }
    </script>
</head>
<body>

<h1>Palindrome or not</h1>
<input type="text" id="inputData" />
<button type="button" onclick="Find()">Find</button>
<h3><U>Output</U></h3>
<p id="output"></p>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/935075a2-bcdb-403b-a15e-f4209bb1df9f)

**Remove Duplicate elements from an array**
```
<!DOCTYPE html>
<html>
<head>
    <script>
  function Find(){
    let arr=[1,2,2,3,4,4,4,5,6];
    const newarr=[];
    console.log(arr);
    for(let i=0;i<arr.length;i++)
    {
        if(newarr.indexOf(arr[i])==-1)
    {
        newarr.push(arr[i]);
    }
    }
    console.log(newarr);
   }
    </script>
</head>
<body>

<h1>Remove Duplicate elements from an array</h1>
<button type="button" onclick="Find()">run</button>
</body>
</html>

```
![image](https://github.com/user-attachments/assets/8f3ea8f8-6ae1-44d1-855d-3a50831de63d)

**Map() Vs filter()**
```
 <script>
  function Find(){
    const arr=[1,2,3,4];
    const mapArr=arr.map(a=>(a*a));  // [1, 4, 9, 16]
    console.log(mapArr);  
    const filterArr=arr.filter(a=>(a%2)==0); // [2, 4]
    console.log(filterArr); 
   }
    </script>
```
**Promise Example**
```
<!DOCTYPE html>
<html>
<head>
    <script>
  let promiseExp=new Promise(function (resolve1,reject1){
    const a=10;
    const b=10;
    if(a==b){
        resolve1();
    }
    else{
        reject1();
    }
  })
  function Find(){
    promiseExp.then(function(){
        console.log("Equal...Promise fulfilled");
    }).catch(function(){
        console.log("Not Equal...Promise Rejected");
    })
   }
    </script>
</head>
<body>
<h1>Promise Exp</h1>
<button type="button" onclick="Find()">run</button>
</body>
</html>
```
