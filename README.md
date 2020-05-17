This is about re-factoring an HTML code so it will be semantically valid:
1. First thing I did was to remove all the <div> elements and replace them with semantic HTML elements instead. I have used this page as a guide to do that:    https://www.w3schools.com/html/html5_semantic_elements.asp. You have to do it step-by-step and update the CSS file as you change each one of them otherwise you       will lose track of your changes and you will break the code.
2. Then I have changed an empty <div> with the class named "Hero" I think to a <figure> element as it was used to contain the main big image as a background which I    don't understand why but I nevertheless replaced this <div> with a <figure> element which is semantic. I wanted to include the image inside this <figure> element    instead of a background in CSS but for some reason the code broke and I didn't know how to fix it so I decided to leave it empty which I think is a big          weakness in my refactoring of this code.
3. Completely organised the CSS file into different sections and copy pasted the appropriate styles for each section under it's related commented title in CSS. I was    able to realize there are so many unnecessary ids and classes during this process and you can safely remove them all. In fact when you finish this step there are    only 2 absolutely necessary classes remain in three places in the code so all the other ids and classes are unnecessary. The format that I used for organizing  the    CSS code was like this (In order from top to bottom):  
   /* Global */   
   /* header and nav bar */   
   /* figure */   
   /* main content */   
   /* aside */   
   /* footer */   
   In each section you should start from the most general selectors to the most specific ones.
4. Finally I have checked the code for validity using https://validator.w3.org/ . This is a very helful tool that shows you whether or not your code has all the    standards. The idea is to fix the errors until the validator gives you no errors.  Most of the errors in this file will be fixed by adding alt text to the <img>    elements. There is also an incorrect </img> element in the code that should be removed since <img> is a self-closing element and does not need a seperate closing       tag. 
