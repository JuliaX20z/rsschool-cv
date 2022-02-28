# Julia Frill

 
**Contacts:** <br />
Email: juliafrill2000@gmail.com <br />
Discord: @juliafrill#1708<br />
Telegram: @astyOOO



### Intro
Hello, my name is Julia, I am just a girl who lives in the south of Chile.<br />
My main goal for 2021-2022 is to become a web developer, create a good portfolio and prove to myself that I can achieve this thanks to my perseverance. From birth, I have a tendency to calm mental work, so I tried myself in various areas of programming. I love to learn and usually understand on the fly any new information, therefore, at the moment I am going through the initial stage of the course on web development – in which I'm interested in.<br />
When I am not interested in something, it is very difficult for me to force myself to learn something, but when there is interest and a wish to do,  I will keep trying until I understand.

### Knowledge and skills
**Programming languages**
*	C – basics
*	JavaScript<br />

**Additionally**
*	Responsive website layout, HTML5, CSS3, as well as basic knowledge of JavaScript/JQuery
*	Git
*	Bootstrap
*	EJS

**Languages:**<br />
Russian - native speaker<br />
Spanish - native speaker<br />
English - level B1-B2

__Education__ - Incomplete secondary general education. “Examenes Libres” (state correspondence examinations). Independent education.

### Code time

__Eratosthenes task in C__

```
  #include <stdio.h>
  int main () {  
      int i, h, c;
      for (i = 2; c < 100; i = i+1){
          int a = 1;
          for (h = 2; h * h <= i; h = h+1){
              if (i % h == 0){
                  a = 0;
                  break; }}
          if (a != 0) {
              c = c+1;
              printf("%d\n",i);
          }
      }
  }
```

__Kata. The Western Suburbs Croquet Club solution in JS__<br />
[Categorize New Member Kata](https://www.codewars.com/kata/5502c9e7b3216ec63c0001aa)

```javascript
function openOrSenior(data){
  var haskellMembers = [];

  for(var i = 0; i < data.length; i++){
      var oneMember = data[i];
    
      if(oneMember[0] >= 55 && oneMember[1] > 7){
        haskellMembers.push("Senior");
      }
      else {
        haskellMembers.push("Open");
      }
  }
  return haskellMembers;
}
```

__Basics of NodeJS, Express and EJS package. My server__
```
const express = require("express");
const bodyParser = require("body-parser");
const date = require(__dirname + "/date.js")

const app = express();

let items = ["Buy Food", "Eat Food", "Cook Food"];
let workItems = [];

app.set('view engine', "ejs");

app.use(bodyParser.urlencoded({ extended: true }));

app.use(express.static("public"))

app.get("/", function (req, res) {

let day = date.getDate();

  res.render("list", {listTitle: day, newListItems: items });
});

app.post("/", function (req, res) {
  let item = req.body.newItem;
  if (req.body.button === "Work"){
    workItems.push(item);
    res.redirect("/work");
  } else {
    items.push(item);
    res.redirect("/");
  }
});

app.get("/work", function(req, res){
  res.render("list", {listTitle: "Work list", newListItems: workItems});
});

app.post("/work", function(req, res){
  let item = req.body.newItem;
  workItems.push(item);
  res.redirect("/work");
});

app.get("/about", function(req, res){
  res.render("about");
});

app.listen(3000, function () {
  console.log("Server started on port 3000.");
});
```

### Education and Projects

Before the course in RS school i have passed [The Complete Web Development Bootcamp](https://www.udemy.com/course/the-complete-web-development-bootcamp/) course on Udemy.<br />

And also a year ago I was studying about C by completing [this course (Основы программирования на C)](https://stepik.org/course/3078/syllabus) on [Stepik](https://welcome.stepik.org/en), after which I solved problems and watched videos on YouTube.<br />

You can see my other works in my [Portfio on Google Drive](https://drive.google.com/drive/folders/1w43h4gGjeHzQq87v4BO6In5JNgMoHpnb?usp=sharing).<br /><br />


![Thanks!](https://www.araioflight.com/wp-content/uploads/2019/05/Thank-You-different-world-languages-world.jpg)







