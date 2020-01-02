# FirstSite
Just playing with HMTL, CSS and JavaScript

## Log of errors:

* The first problem was the width of the table. I wanted it equaled spaced between the cells but also that had a good resizing. The solution that I got was... not good practice I think. I changed the width of every td element in css to be 23%, without messing with the width of the table itself (default: 100%). Somehow everything is working well until now but odd thing happens when I change the percentual. e.g.: When I put 20% the table gets bigger and when I put above 25% somes collumns gets bigger, others gets smaller (I think it's because the total sum gets above 100%). The reason why I still using this messing 23% value because if I put a percentual in the width of the table the smaller version of the page breaks the table, if I put, for example, 290px as the width of the table, it gets a little too big in smaller screens. In the current way the table shrinks in irregular forms, but it still readble in smaller screens. (<a href = "https://stackoverflow.com/questions/59511653/why-percentages-of-width-of-td-in-css-dont-seem-to-work">Question and answers in Stackoverflow</a>)

* The second problem was how to add 15 methods to each cell of the table to make them change the background color of the page when the mouse hovers over them. As I am a beginner in JavaScript I tried this code: 
```
    for(var i = 1; i < 16; i++){
          celula[i].onmouseover= function(){
            document.body.style.backgroundColor = celula[i].getAttribute("bgcolor");
          }
          celula[i].onmouseout = function(){
            document.body.style.backgroundColor = inicial;
          }
        }
```
The problem (that right now I don't understand completely) was that I used the keyword "var" in the declation of the i varible.       The correct way is to use the "let" keyword for reasons of different scope (something like this).

* I commited a type error in the 14º cell's attribute. I didn't put the '#' symbol before the hex code of the bgcolor attribute (I discovered on <a href= "https://stackoverflow.com/questions/59556855/problem-with-interactive-table-in-javascript-html-onmouserover">Stackoverflow</a> that bgcolor is a deprecated attibute. I will put the colors with CSS in the future).
  
