 Project's Title.  SDF04 Project | CSS Magic Buttons

Codepen link :https://codepen.io/siyabonga-masenya/pen/ZENbwYw

 Project Description.
  The aim is to create animated buttons for our website 

 How to Install and Run the Project.

  Copy both  the HTML and CSS code and paste it into VS Code or Codepen. 


Breakdown 
  
  In the Root section on CSS, I created three variables for the three primary colors I wanted the web page to be.
        

Root{}
    :root {
        --offwhite: #f2e8dc;
        --chutney: #d9a59a;
        --maroon: #73403c}

  These variables would be used to create a warm color palette for the web page.




Body

  In the body section would use a background instead of a flat image to create a warm tone throughout the web page .I did this by inputing the code below 
      
      Background-image: url(https://i.pinimg.com/736x/7b/06/c0/7b06c0fad2243d797015068c7e456d1b.jpg);



Button Attributes
  For the button hover  attributes (.btn) I would keep the styling  consistent by adding a chutney overlay with maroon text 
    e.g.. The code used for the animations was inspired from the examples provided at https://codepen.io/codespace-academy/pen/xxmWrjX


      btn-1:after {
        position: absolute;
        content: "";
        width: 0;
        height: 100%;
         top: 0;
        right: 0;
        z-index: -1;
        background-color: var(--chutney);
        border-radius: 5px;
        box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
        7px 7px 20px 0px rgba(0,0,0,.1),
         4px 4px 5px 0px rgba(0,0,0,.1);
        transition: all 0.3s ease;



     btn-1:hover {
        color: var(--maroon);
        font-size:1.3em;
