# iNeuron-JavaScript-DOM-Assignment


1.Website Name: [Dev To](https://dev.to/)

## Topic

```
Query Selctory, Inner HTML
```

## Sample Image
![](JS-DOM/1.png)

## Task

```
Target the Top description div and change the DEV Community to <Your_Name> and description to your passion
```    

## Solution
![](JS-DOM/2.png)


2.Website Name: [Apple](https://support.apple.com/en-in)

## Task

![](JS-DOM/3.png)

## Solution
```
const listNsmr = document.querySelectorAll(".as-imagegrid-item");
//console.log(listNsmr)
const storeValHouse =  [];
listNsmr.forEach((item)=>{
let x = item.innerText.replace("\nSupport", "");
storeValHouse.push(x);
})
console.log(storeValHouse)
```
['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']


3.Website Name: [Youtube Support](https://support.google.com/youtube/#topic=9257498)

## Topic

```
Get Element By Id, Create Element, Create Text Node, Append Child
```

## Sample Image
![](JS-DOM/4.png)

## Task
```
Add another FAQ 'My New FAQ' to the list
```

## Solution
![](JS-DOM/5.png)
```
const targetMain = document.querySelector(".accordion-homepage");
const addSection = document.createElement("section");
addSection.className = "parent";
const addTag = document.createElement("h3");
addTag.textContent = "My New FAQ"
targetMain.appendChild(addSection)
addSection.appendChild(addTag);
```


4.Website Name:[OnePlus](https://service.oneplus.com/in)

## Topic
```
Query Selector, InnerText
```
## Sample Image
![](JS-DOM/6.png)

## Task

```
Change the contact number
```
## Solution

```
document.querySelector(".customer-support a").innerText = '+919962929448'
```


5.Website Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

## Topic

```
getElementById, createElement, InnerText, append, setAttribute
```
## Task
```
Target the main div of card and change the Button text to Check out
```
## Solution

![](JS-DOM/8.png)


6.Website Name:[Adidas](https://www.adidas.co.in/)


## Topic

```
Query Selector, Event listeners, Changing Styles
```

## Task

```
Target the search box and on hover change thebackground color to red.
```

## Solution

```
  const find = document.querySelector(".searchinput___19uW0")
  find.addEventListener("mouseover", changbg)
  function changbg(){
  find.style.backgroundColor = "red"
  };

  /*or*/
             document.querySelector(".searchinput___zXLAR").addEventListener("mouseover", function() {
 document.querySelector(".searchinput___zXLAR").style.   backgroundColor = "red";
 });
 ```
 
 7.Website Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)
 
 ## Topic
 
 ```
 Form, Value, Submit
```

## Task

```
To Search a topic in the MDN Search bar.
First add a text to search in the search bar and then hit the submit search button to search the docs using DOM
```

## Solution

![](JS-DOM/9.png)

```
let form = document.getElementById("hp-search-form");

form.querySelector("input").value = "CSS Selector";

form.submit();
```


8.Website Name: [Google](https://www.google.com/)

## Topic

```
Remove Elements
```

## Task

```
 Remove alternate languages from the home page languages listed
```

## Solution

![](JS-DOM/10.png)

```
let x = document.querySelectorAll('.z4hgWe a')
x.forEach((a,index)=>{
index % 2 == 0 && a.remove()
})
```

9.Website Name: [Code Wars](https://www.codewars.com/)

## Topic

```
   Change Font Family, Color of Text.
```   

## Task

```
Change the font family of the text to monospace and text color to the logo’s background color.
```

## Solution

![](JS-DOM/11.png)

```
document.querySelector(".text-align-center").style.fontFamily="monospace";
document.querySelector(".text-align-center").style.fontFamily="orange";
```

10.Website Name: [Freecodecamp](https://www.freecodecamp.org/)

## Topic

```
querySelector, mouseover, click eventListener,  callback function, style
```

## Task

```
Target the button and change background colour on mouseover
```

## Solution

![](JS-DOM/12.png)

```
  document.querySelector(".btn-cta-big .login-btn-text ").addEventListener("mouseover",function(){

  document.querySelector(".btn-cta-big .login-btn-text ").style.backgroundColor="red"
```  
 



