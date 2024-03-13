
## Code I Figured Out: 

.dropdownmenu1 { 

&nbsp;&nbsp;&nbsp;&nbsp;display: flex;

&nbsp;&nbsp;&nbsp;&nbsp;padding: 0;

&nbsp;&nbsp;&nbsp;&nbsp;position: absolute;

&nbsp;&nbsp;&nbsp;&nbsp;transition: all 0.75s ease-out, top 0s 0.75s;

&nbsp;&nbsp;&nbsp;&nbsp;top: -50px;

&nbsp;&nbsp;&nbsp;&nbsp;left:0;

&nbsp;&nbsp;&nbsp;&nbsp;min-width: 5rem;

&nbsp;&nbsp;&nbsp;&nbsp;width: 100%;

&nbsp;&nbsp;&nbsp;&nbsp;box-shadow: none;

&nbsp;&nbsp;&nbsp;&nbsp;max-height: 0;  

&nbsp;&nbsp;&nbsp;&nbsp;z-index: -10;

&nbsp;&nbsp;&nbsp;&nbsp;opacity: 0;

}

.menu li p.hovermenu:hover ~ .dropdownmenu1,

.dropdownmenu1:hover

{

&nbsp;&nbsp;&nbsp;&nbsp;display:flex;

&nbsp;&nbsp;&nbsp;&nbsp;flex-direction: row;

&nbsp;&nbsp;&nbsp;&nbsp;top:56px;

&nbsp;&nbsp;&nbsp;&nbsp;min-width: 5rem;

&nbsp;&nbsp;&nbsp;&nbsp;max-height: 100%;

&nbsp;&nbsp;&nbsp;&nbsp;width: 100%;

&nbsp;&nbsp;&nbsp;&nbsp;background-color: rgb(40, 1, 113);

&nbsp;&nbsp;&nbsp;&nbsp;opacity: 1;

&nbsp;&nbsp;&nbsp;&nbsp;overflow: visible;

&nbsp;&nbsp;&nbsp;&nbsp;transition: all 0.75s ease-out, top 0s;

  }

All the links i used to find ways to make this work are above, I learned about ~ and about applying separate animations to an object on hover and on taking the mouse off it

 - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container: couldn’t figure out why the home icon wasn’t aligning properly, used this and did justify-content and it worked

 - https://stackoverflow.com/questions/16028878/animating-max-height-with-css-transitions 

 - https://www.w3schools.com/cssref/css_selectors.php 

 - https://stackoverflow.com/questions/15891633/how-to-change-the-css-of-one-image-when-hovering-another-image 
I didn’t know to use the ~ to target other parts but checking this helped me figure out that I needed ~ for what I wanted to occur

 - https://developer.mozilla.org/en-US/docs/Web/CSS/transition-delay 

 - https://stackoverflow.com/questions/5921073/different-css-transition-delays-for-hover-and-mouseout apply separate transition and transition delays to hovering and mousing off
