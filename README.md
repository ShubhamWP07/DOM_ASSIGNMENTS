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
![Screenshot (71)](https://user-images.githubusercontent.com/97464092/215344033-2c14b78a-a735-465c-8c96-9deb58ab2974.png)

```
// Removing Hire Me

let removelistitem = document.querySelector("ul");
removelistitem.removeChild(removelistitem.children[3]);


// Removing social icon

let removesocialicons = document.querySelector("footer ul")
removesocialicons.remove();

// Changing Inputtext 

let Inputtext = document.querySelector("header nav .search-field input");
Inputtext.placeholder = "Search My Project";
```

### Task_03
![Screenshot (72)](https://user-images.githubusercontent.com/97464092/215723203-ee9cf77e-848c-4a51-b705-c56c483554bb.png)

```
"use strict"

// Changing Inputtext 

let textbox = document.querySelector("header nav .search-field input");
textbox.placeholder = "Search";

// Chaniging Paragragph a freelancer to an Employee

let para = document.querySelector(".hero-left-section p span:nth-child(3) ")
// console.log(para.innerHTML)
para.innerText = "an Employee";

// Chaniging Paragragph National and International Client to iNeuron Intelligence Pvt Ltd

let para2 = document.querySelector(".hero-left-section p span:nth-child(5) ")
// console.log(para2.innerHTML)
para2.innerText = "iNeuron Intelligence Pvt Ltd";
```

### Task_04
![Screenshot (73)](https://user-images.githubusercontent.com/97464092/215728505-26d71652-f45c-42f9-aadf-ac87e385404a.png)

```
// Chaniging Paragragph an Employee to a freelancer 

let para3 = document.querySelector(".hero-left-section p span:nth-child(3) ")
// console.log(para.innerHTML)
para3.innerText = "a freelancer";

// Chaniging Paragragph iNeuron Intelligence Pvt Ltd to National and International Client

let para4 = document.querySelector(".hero-left-section p span:nth-child(5) ")
// console.log(para2.innerHTML)
para4.innerText = "National and International Client";

// Changing Image

let img = document.querySelector(".hero-section .hero-right-section img")
console.log(img);
img.src = "https://hiteshchoudhary.com/static/a8d73d1aac4c79e9bb689640e6090367/2eaab/person-image.jpg"
```

### Task_05
![Screenshot (74)](https://user-images.githubusercontent.com/97464092/215735350-158b39b9-a168-4fdf-84e6-297160f3efc6.png)

```
// Changing img to Default

let img2 = document.querySelector(".hero-section .hero-right-section img")
console.log(img);
img2.src = "avtar.png"

// Creating Button

let addbtn = document.createElement("button");
let btntext = document.createTextNode("Support Me");
addbtn.appendChild(btntext);

let btn_path = document.querySelector(".hero-right-section-btns");
console.log(btn_path.innerHTML)
btn_path.appendChild(addbtn);
```

# Question 2
### Task_01
![Screenshot (75)](https://user-images.githubusercontent.com/97464092/215744978-3e11bed7-6a16-4247-a22e-160283670fe8.png)

```
// Changing BG Color

let bgc = document.querySelectorAll(".accordian h3")
for(let i = 0; i<bgc.length; i++){
  bgc[i].style.backgroundColor = "#dadaf8";
}
// console.log(bgc);
```

### Task_02
![Screenshot (76)](https://user-images.githubusercontent.com/97464092/215759917-e51cafd1-f519-45e2-9e99-ea6aef09e287.png)

```
// Adding new accordian div

let accdiv = document.createElement("div");
let div_path = document.querySelector(".accordian-wrapper");
div_path.appendChild(accdiv);
accdiv.classList.add("accordian");



// Adding new accordian Heading

let acc_last_div = document.querySelector(".accordian-wrapper div:last-child");
console.log(acc_last_div)

let createacc = document.createElement("h3");
let accheadingtext = document.createTextNode("Skills")
createacc.appendChild(accheadingtext);
createacc.style.backgroundColor = "#dadaf8";


let acc_path = document.querySelector(".accordian-wrapper:last-child");
acc_last_div.appendChild(createacc);


// Adding new accordian paragraph

let accpara = document.createElement("p");
let accparatext = document.createTextNode("I posses a very good command over the Full Stack Development technologies like MERN which can be seen in my work over the Github.")
accpara.appendChild(accparatext);

let acc_para_path = document.querySelector(".accordian-wrapper")
acc_last_div.appendChild(accpara);


// Adding Styles and functions

let accordian2 = document.querySelectorAll(".accordian:last-child h3");
accordian2.forEach((element) => {
  element.addEventListener("click", () => {
    let para = element.nextElementSibling;
    if (para.style.display === "block") {
      para.style.display = "none";
    } else {
      para.style.display = "block";
    }
  });
});

let newvar = document.querySelector(".accordian-wrapper")
console.log(newvar)

```

# Question 4
![Screenshot_20230201_101834](https://user-images.githubusercontent.com/97464092/216108181-dd03f256-778c-48b7-b1d2-2ac3769d57fa.png)

```
// Changing color of all scores

let Paracolor = document.querySelectorAll(".stat,.stat-value");
console.log(Paracolor)
for (let i = 0; i < Paracolor.length; i++) {
  Paracolor[i].style.color = "#fff";
};


// Changing bgc of Barbarian

let Barbarian = document.querySelector(".clash-card__unit-stats--barbarian");
Barbarian.style.backgroundColor = "#ec9b3b";


// Changing bgc of Archer

let Archer = document.querySelector(".clash-card__unit-stats--archer")
Archer.style.backgroundColor = "#ee5487"

// Changing heading text of cr-2

let cr2 = document.querySelectorAll(".clash-card__level--archer+div")
console.log(cr2)
for (let i=0; i<cr2.length; i++) {
  if(cr2[i].innerText = "Character 2"){
    cr2[i].innerText = "The Archer";
  }
}



// Changing bgc of Giant

let Giant = document.querySelector(".clash-card__unit-stats--giant");
Giant.style.backgroundColor = "#f6901a";

// Changing heading text of goblin

let cr4 = document.querySelectorAll(".clash-card__level--goblin+div")
console.log(cr4)
for (let i=0; i<cr4.length; i++) {
  if(cr4[i].innerText = "Character 2"){
    cr4[i].innerText = "The Goblin";
  }
}

// Changing bgc of goblin

let goblin = document.querySelector(".clash-card__unit-stats--goblin")
goblin.style.backgroundColor = "#82bb30"

// Changing bgc of wizard

let wizard  = document.querySelector(".clash-card__unit-stats--wizard")
wizard.style.backgroundColor = "#4facff"
```

# Question 5
![Screenshot (79)](https://user-images.githubusercontent.com/97464092/217028307-050c22e8-3286-4866-8542-d0b4106d8bb9.png)

```
// Adding Button

let btn = document.createElement("button");
let btntxt = document.createTextNode("Pro Subscription");
btn.appendChild(btntxt);
btn.classList.add("btn")
btn.style.border = "none"
btn.style.fontFamily = "none";

let contact_btn = document.querySelector(".btn")
// console.log(contact_btn)
contact_btn.style.marginLeft = "350px"

let btn_loaction = document.querySelector(".nav-center");
// console.log(btn_loaction)
btn_loaction.appendChild(btn);


// Adding Recipes

let chinise = document.createElement("h3");
let ch_txt = document.createTextNode("Chinese (7)")
chinise.appendChild(ch_txt)
chinise.style.fontSize = "24px"
chinise.style.color = "brown"
chinise.style.fontWeight = "300"

let ch_location = document.querySelector(".tags-container");
console.log(ch_location);
ch_location.appendChild(chinise)

// Adding card

let card_div = document.createElement("div");
card_div.classList.add("card")

let card_div_location = document.querySelector(".recipe-gallery")
console.log(card_div)
card_div_location.appendChild(card_div)

// Adding img

let pizza_img = document.createElement("img")
pizza_img.src = "https://www.google.com/url?sa=i&url=https%3A%2F%2Fpixabay.com%2Fimages%2Fsearch%2Fpizza%2F&psig=AOvVaw3ilqaF5xn8LJFei-6Q3Iuk&ust=1675600469823000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCLiFm6jw-_wCFQAAAAAdAAAAABAE"
pizza_img.src.appendChild(pizza_img);
pizza_img.classList.add("recipe-img")

let pizza_img_location = document.querySelector(".recipe-gallery card_div ")
pizza_img_location.appendChild(card_div)
```

# Question 6
### Task_01
![Screenshot (77)](https://user-images.githubusercontent.com/97464092/217029430-16e4b84f-b321-4406-8c24-d36467c68289.png)

```
// Changing Logo

let logo = document.querySelector(".logo");
// console.log(logo);
logo.src = "https://ineuron.ai/images/ineuron-logo.png";
```

### Task_02
![Screenshot (78)](https://user-images.githubusercontent.com/97464092/217029780-226721a3-d603-440f-bdc8-330524182852.png)

```
// Changing Price

let price = document.querySelector(".app_price span");
console.log(price);
price.innerText = "$10"
```
