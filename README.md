# FirstSite
Just playing with HMTL, CSS and JavaScript

## Log of errors:

* The first problem was the width of the table. I wanted it equaled spaced between the cells but also that had a good resizing. The solution that I got was... not good practice I think. I changed the width of every td element in css to be 23%, without messing with the width of the table itself (default: 100%). Somehow everything is working well until now but odd thing happens when I change the percentual. e.g.: When I put 20% the table gets bigger and when I put above 25% somes collumns gets bigger, others gets smaller (I think it's because the total sum gets above 100%). The reason why I still using this messing 23% value because if I put a percentual in the width of the table the smaller version of the page breaks the table, if I put, for example, 290px as the width of the table, it gets a little too big in smaller screens. In the current way the table shrinks in irregular forms, but it still readble in smaller screens.

*
