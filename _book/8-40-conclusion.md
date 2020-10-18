# (PART) Closing Remarks {-}

# Conclusion {#conclusion}

The book covered a few topics and introduced a lot of concepts probably new to many, these are sometimes difficult to fully understand at first and will likely require some more exploring. So here, we wrap up with some heartening thoughts to encourage the reader to persevere as much of what was covered in the book requires practice to be fully comprehended.

## Performances {#conclusion-performances}

As mentioned in the opening of this book some of the code presented is not entirely optimal as we need to make use of R as much as possible to limit any confusion caused by the fresh-to-the-eyes JavaScript code. In places, this involves making use of R where it is in fact not needed, namely within shiny applications where sometimes data is sent from the front end to R, only to be sent back to JavaScript again. For instance, when the click of a button triggers something in the shiny UI but uses the server as an intermediary, oftentimes it is not necessary to involve the server.

This, though has little impact on performances in most cases, can be improved upon by not involving R in the process, handling everything in the front-end with JavaScript but this was judged outside the scope of the book as it focuses on interactions between the two languages. Nonetheless, somewhat interestingly, the book covered all the code necessary to do so, only not in the same section or chapter. It might therefore take some practice to make the connection.

```js
// toggle an input at the click of a button
$('#button').on('click', function(){
  $('#input').toggle();
});
```

## Road Ahead {#conclusion-ahead}

Practice makes perfect: the best way to become at ease with the learnings of the book is probably to attempt to put them into practice. In addition to finishing the projects used as examples in this book, below are some ideas of great JavaScript library that are yet to be integrated with R, make for great practice and would great benefit the community.

### Computation {#compute}

- [chance.js](https://github.com/chancejs/chancejs) - random generator
- [currency.js](https://github.com/scurker/currency.js) - helpers to work with currencies

### Shiny {#shiny}

- [micromodal.js](https://github.com/Ghosh/micromodal) - tiny, dependency-free javascript library for creating accessible modal dialogs
- [hotkeys](https://github.com/jaywcjlove/hotkeys) - capture keyboard inputs
- [handtrack.js](https://github.com/victordibia/handtrack.js) - realtime hand detection
- [annyang](https://github.com/TalAter/annyang) - speech Recognition library 

### htmlwidgets {#widgets}

- [chart.js](https://www.chartjs.org/) - simple yet flexible JavaScript charting
- [cytoscape.js](https://js.cytoscape.org/) - network theory library for visualisation and analysis
- [Toast UI charts](https://ui.toast.com/tui-chart/) - easy way to draw various and essential charts
- [amcharts](https://www.amcharts.com/) - library for all your data visualization needs

Moreover, the book did obviously not cover everything that can be done with JavaScript, much more is possible. Perhaps this book entices the reader to go a step further and become more familiar with JavaScript.