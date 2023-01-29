# DOM_ASSIGNMENTS
## 28th Jan Dom Assignments

# Question 1
### Task_01
![Screenshot (69)](https://user-images.githubusercontent.com/97464092/215342223-dc2f11fb-56c3-4bed-85ac-4b86a970637b.png)

```
// Adding Hire Me

let list = document.createElement("li");
let text = document.createTextNode("Hire Me");
list.appendChild(text);

let element = document.querySelector("ul");
element.appendChild(list);

// Changing Contact to Project

let thirdchild = document.querySelector("header nav ul li:nth-child(3)")
thirdchild.innerText = "Project";

// Removing social icon

let removesocialicons = document.querySelector("footer ul")
removesocialicons.remove();
```

### Task_02
