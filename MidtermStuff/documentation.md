
Code I Figured Out: 
.dropdownmenu1 {
    display: flex;
    padding: 0;
    position: absolute;
    transition: all 0.75s ease-out, top 0s 0.75s;
    top: -50px;
    left:0;
    min-width: 5rem;
    width: 100%;
    box-shadow: none;
    max-height: 0;  
    z-index: -10;
    opacity: 0;
}

  .menu li p.hovermenu:hover ~ .dropdownmenu1,
  .dropdownmenu1:hover
  {
    display:flex;
    flex-direction: row;
    top:56px;
    min-width: 5rem;
    max-height: 100%;
    width: 100%;
    background-color: rgb(40, 1, 113);
    opacity: 1;
    overflow: visible;
    transition: all 0.75s ease-out, top 0s;
  }

All the links i used to find ways to make this work are above, I learned about ~ and about applying separate animations to an object on hover and on taking the mouse off it

 - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container: couldn’t figure out why the home icon wasn’t aligning properly, used this and did justify-content and it worked

 - https://stackoverflow.com/questions/16028878/animating-max-height-with-css-transitions 

 - https://www.w3schools.com/cssref/css_selectors.php 

 - https://stackoverflow.com/questions/15891633/how-to-change-the-css-of-one-image-when-hovering-another-image 
I didn’t know to use the ~ to target other parts but checking this helped me figure out that I needed ~ for what I wanted to occur

 - https://developer.mozilla.org/en-US/docs/Web/CSS/transition-delay 

 - https://stackoverflow.com/questions/5921073/different-css-transition-delays-for-hover-and-mouseout apply separate transition and transition delays to hovering and mousing off
