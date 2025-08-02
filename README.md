## Fun facts about javascript and CSS

1. you can multiply a null variable with any number and get 0 - without any error!
2. dont ever assign svg-attributes such as rx in <rect rx="20" ...> in CSS, even if it looks like the change was applied - if you try grabbing the rx (or other svg-attribute) in javascript, say via `element.rx.baseVal.value` or `element.getAttribute('rx')`, you will also get 0 ..
3. always define the `position` property of a div in css; ordering layers through the `z-index` is f.e. not possible if `position: relative;` is not specified.
4. Assigning a class to an element will NOT give an error in the javscript console if the class to be assigned through `element.classList.add('class-to-assign')` is not defined or not spelled correctly in any CSS file or `style` tag.