---
marp: true
size: 4:3
theme: default
paginate: true
---


<!-- slide settings -->
<style>
    /* more readable text */
    p {text-align:justify;}

    /* fixing footer position */
    footer {bottom:-9px;left:0;z-index:99;}
    
    /* editing pagination */
    section:after{
        /* position */
        /* content:attr(data-marpit-pagination)" of "attr(data-marpit-pagination-total); */
        bottom:4%;left:50%;z-index:199;

        /* color and text style */
        /* background:none; */
        color:white;font-size:0.6em;font-weight: bold;
    }

    /* one column slide style */
    twocolumn,onecolumn,ti,it {height:100%;}

    /* text-img slide style */
    ti p {float:left;width:50%;}
    ti img {width:90%;float:right;}

    /* img-text slide style */
    it p {float:right;width:50%;}
    it img {width:90%;float:left;}
    
    /* fixing footers in customized slides */
    ti footer{left:-107px;bottom:-2.7px}
    it footer{right:-107px;bottom:-2.7px}

    twocolumn column1 {width:48%;float:left;}
    twocolumn column2 {width:48%;float:right;}
    

</style>

<!-- --------------------------------------- -->
<!-- TITLE OF THE PRESENTATION -->
<!-- --------------------------------------- -->
<!-- paginate: skip -->
<!-- footer: "" -->
![bg](img/portada.jpg)
<br/>


# UG Slides using MARP <!-- fit -->
* **Autor✍:** Francisco Javier Moreno Vazquez
* **Email✉:** **fj.morenovazquez@ugto.mx**

---

<!-- --------------------------------------- -->
<!-- BODY OF PRESENTATION -->
<!-- --------------------------------------- -->
<!-- paginate: true -->
<!-- footer: "![](img/interior.jpg)" -->

<!-- PUT TEXT DOWN HERE -->
# What is MARP?

> Create beautiful slide decks using an intuitive Markdown experience

MARP (also known as the *Markdown Presentation Ecosystem*) provides an intuitive experience for creating beautiful slide decks. You only have to focus on writing your story in a Markdown document.

---

<!-- PUT TEXT DOWN HERE -->
# Some Features

* **Based on CommonMark**
* **Directives and extended syntax**
* **Built-in themes and CSS theming**
* **Export to HTML, PDF, and PowerPoint**
* **Marp family: The official toolset**
* **Pluggable architecture**
* **Fully open-source❤**

---

<!-- PUT TEXT DOWN HERE -->
# Normal/Simple Mode<!-- fit -->

Marp creates slides with the next format:
```html
<section>
  <header>Header content</header>
  <h1>Page 1</h1>
  <footer>Footer content</footer>
</section>
```
Where each slide is a section, so this can be changed with CSS styles. In the default style, the content starts at the vertical center of the slide.

---

<!-- PUT TEXT DOWN HERE -->
<onecolumn>

# Custom `onecolumn` slide style<!-- fit -->

By using css styles we can configurate the slide to produce a Powerpoint like layout.
* In this layout the content begins at the top of the slide.
* Each paragraph `<p>` is justify to be a more readable text.

</onecolumn>

---

<!-- PUT TEXT DOWN HERE -->
<twocolumn>

# Custom `twocolumn` slide style<!-- fit -->

<column1>

This slide is styled to be a doble columns slide, this is produced by using to html elements inside the `<twocolumn>` element.
* In this case, this is the first column or the `<column1>` element.

</column1>

<column2>

This slide is styled to be a doble columns slide, this is produced by using to html elements inside the `<twocolumn>` element.

* And this is the second column or the `<column2>` element.

</column2>

</twocolumn>

---

<!-- PUT TEXT DOWN HERE -->
<ti>

# Custom `ti` slide style<!-- fit -->

This slide is called `ti` that stands for *Text and Image* slide. We can see the image floating at the right of the slide.

![](https://picsum.photos/720?image=1)

</ti>

---

<!-- PUT TEXT DOWN HERE -->
<it>


# Custom `it` slide style<!-- fit -->

Conversely, this slide is called `it` that stands for *Image and Text* slide. We can see the image floating at the left of the slide.

![](https://picsum.photos/720?image=3)

</it>

---


<!-- --------------------------------------- -->
<!-- END OF PRESENTATION -->
<!-- --------------------------------------- -->

<!-- footer: "" -->
<!-- paginate: false -->
![bg](img/contraportada.jpg)
