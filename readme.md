# a11y-slides-math
HTML template to write accessibility-oriented slides with symbolic mathematical content 
rendered using [MathJax](https://www.mathjax.org/). 

## usage/getting started
Download the file `a11y-slides-math-template.html` and edit it as you see fit. You'll find the 
necessary Javascript and CSS at the bottom of the file. 

You can navigate through the slides using the LEFT and RIGHT arrow keys.

## version
V0.1, 2024-11-14

## testing with NVDA
To test `a11y-slides-math-template.html` with [NVDA](https://www.nvaccess.org/download/), use the following steps:

1. open `a11y-slides-math-template.html` in your web browser (I recommend Chrome or Firefox, but others should work also);
2. launch NVDA, note that the default NVDA key is the INSERT key, and that this can be changed;
3. navigate through the first slide using the UP and DOWN arrow keys; on each slide, you should hear the text from the `<h1>` announced;
4. press NVDA+SPACE to exit <i>focus</i> mode, and you can now navigate through the slides by using the RIGHT and LEFT arrows;
5. when you want to interrogate a slide, press NVDA+SPACE to enter <i>focus</i> mode, and then use the UP and DOWN arrows to interrogate the details of the slide;
6. on slide 3 of `a11y-slides-math-template.html` you will encounter some symbolic mathematical content:
    * when you reach the mathematical content, press ENTER;
    * now press SHIFT+SPACE which should allow you to interrogate this mathematical content at different levels using the arrow keys via the MathJax explorer extention; press SPACE to have NVDA announce your current level;
    * when you're done interrogating the mathematical content, press ESC, and then NVDA+CTRL+SPACE, which should 
      return you to the next part of the slide;
7. if you want to exit/quit NVDA, press NVDA+Q.

For reference, see the [NVDA keyboard shortcuts](https://www.nvaccess.org/files/nvdaTracAttachments/455/keycommands%20with%20laptop%20keyboard%20layout.html).

## assumptions about users of this
I assume the following two assumptions about users of this template:

1. they wish to prioritise accessibility;
2. they only wish to do the work of creating their slides once.

## anticipated questions, and responses
<details>
<summary>I'm happy with the way I produce my slides, why should I use this?</summary>

If you're happy with your method, keep using your method, and don't use this template. 
</details>

<details>
<summary>why not LaTeX?</summary>

Before I answer, please understand that I am a supporter of `LaTeX`; see my tex stackexchange profile at [cmhughes](https://tex.stackexchange.com/users/6621/cmhughes), and [latexindent.pl](https://github.com/cmhughes/latexindent.pl/) which I have authored and maintained since 2012.

`LaTeX` produces `pdf` files by default. Such `pdf` files that contain mathematical content will, in general, not be accessible to assistive technology. Authors that choose
to use `LaTeX` (with classes such as `beamer`) will have to do the work of creating their slides more than once if they wish to create an accessible version. If you have
a method that you're happy with, stick with it. 
</details>

<details>
<summary>why not PowerPoint?</summary>

I have been unable to produce a PowerPoint slide deck containing mathematical content that allows me to interrogate mathematical content. If you have instructions 
on how this can be done, please do link me to them.
</details>

<details>
<summary>why not reveal js?</summary>

I have been unable to create [reveal.js](https://revealjs.com) slides that I can navigate with 
assistive technology. If you have an example that works, please do link me to them.
</details>

<details>
<summary>why not dzslides?</summary>

I have been unable to create [dzslides](https://github.com/paulrouget/dzslides) slides that I can navigate with 
assistive technology. If you have an example that works, please do link me to them.
</details>

<details>
<summary>how can I get my LaTeX/PowerPoint/whatever into a11y-slides-math format?</summary>

I have no idea, and that's not what this project is about. I only want to do work once (see assumption 2 in the above), so I *produce* my slides in `a11y-slides-math` format. 
</details>

<details>
<summary>what about fancy transitions and visual effects?</summary>

`a11y-slides-math` is not about fancy transitions and visual effects. If you want something 
more visually appealing, you can edit the `CSS` and `Javascript` as you see fit, or use 
something like [reveal.js](https://revealjs.com) or [dzslides](https://github.com/paulrouget/dzslides). 

`a11y-slides-math` is deliberately simple HTML with minimal Javascript and CSS, designed to be navigated
with assistive technology.  I intend to keep it that way, prioritising accessibility and screen reader navigability above everything else.

</details>

## acknowledgements
This project is based on the work of Utibe Udoma posted at [How to build a slideshow using HTML, CSS, and JavaScript](https://medium.com/illumination/how-to-build-a-slideshow-using-html-css-and-javascript-977ecbdbf48c)