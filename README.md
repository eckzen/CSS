# CSS

em sizing

    body{
        font-size: 62.5%;
    }
    1.6em = 16px

Background image

    to repeat
        background-image: url("image.jpg");
    repeating pattern is default

Fix background while scrolling

    background-attachment: fixed;

To center 

    margin: 0 auto;

Create a gradient background

    background-image: linear-gradient (top, #000, gray);
    starts from top. from black to gray

Scalable background

    background-image: url("image.png");
    background-position: center center;
    background-attachment: fixed;
    background-size: cover;

Set all

    * {
        margin: 0;
        padding: 0;

        box-sizing: border-box;
    }

Non repeating background

    background-image: url("image.png");
    background-repeat: no-repeat;
    background-position: bottom right;

    single line
    background: url("image.png") bottom right no-repeat, #fff;

    opacity: 0.9;

##Google Fonts

    copy the code from google fonts
    insert the code into your HTML
    to use in CSS use the sample font-family in the google fonts

##Links

visited links

    a:link, a:visited{
        text-decoration: none;
    }    

    a:hover{
        background-color: #21234;
    }

Text shadow

    h1{
        text-shadow: 2px 2px 3px gray; y x shadow color
    }

Remove the margin if it follows a p in h1

    h1 + p {
        margin-top: 0;
    }

Indent text

    .firstp{
        padding-left: 1.4em;
    }

    fourthp:first-letter{
        font-size: 200%;
        line-height: 1;
    }

Dropp shadow in an image

    box-shadow: 2px 2px 3px gray;

Round corners

    border-radius: 10px;

Rotate the image

    transform: rotate (3deg);

Use image inside the list item

    ul{
        list-style-image: url("image.png");
        list-style-type: none;
    }

To display the list items in horizontal

    li{
        display: inline;
    }

##Tables

    table{
        caption-side:bottom;
    }

        width:600px;
        border: 1px solid #000;
        border-collpase: collapse;
        text-align: center;
        font-weight: bold;

alternate the color

        .row tr:nth-child(odd){
            background-color: #434324;
        }            

hover in table

        .row tr:hover{
            background-color: #434534;
        }

##Forms

    width: 375px
    float: left;
    width
    padding

    label{
        float:left;
        width
    }

    input{
        width
    }

    submit{
        float: right;
        width: auto;
    }

Highlight different parts of the form when accepting input

    .class input:focus{
        background-color: #434534;
    }

##Floats

    .float{
        position: absolute;         #reference is the whole page
        top: 0px;
        right: 55px;
    }
        .wrapper{
            position: relative:     #the new reference of .float
        }

#Gallery

    ul.gallery{
        list-style-none     #to remove the bullets
        clear: both         #no other object on both sides
    }         

    ul.gallery li{
       display: inline-block;   #no new line and can be styled
       position: relative;
    }

To show text whenever the mouse hovers on the image

    ul.gallery span{
        width: 25;
        height: 35px; 
        text-aligh: center;
        position: absolute;
        bottom: 0px;
        left: 0px;
        background-color: #000;
        opacity: 0.75;
        color: #fff;
    }

    ul.gallery span{
        margin-left: -10000px;              #default state
    }

    ul.gallery li:hover span{
        margin-left: 0;                     #when the mouse hovers margin-left 
    }                                       goes to 0


    inline - are elements that are NOT FOLLOWED by a new line;
        note: in inline you cannot style the margin, height, padding

    block - are elements that are FOLLOWED by a new line;

#Layouts

    * {
        margin: 0;
        padding: 0;
    }

    body {
        background-color: gray;
        font-size: 62.5%
    }

    .wrapper{
        width: 900px;
        font-size: 1.6em;               # 1.6em = 16px
        margin: 0 auto;
    }
    normalize


    text-align: left;               #align text
    background-color: pink;         #background
    color: white;                   #font color
    font-family: serif;
    text-shadow: 2px 2px 3px rgba(0, 0, 0, 0.5) #text shadow

    .main{
        position: relative;
    }

Scenario


    }
    aside {
        width: 250px;
        float: right;
    #to extend the sidebar all the way to the bottom
        padding-bottom: 5000px;
        margin-bottom: -5000px;
    }

    main{
        float: left;
        width: 550px;
    }

    .wrapper {
        overflow: hidden;     #to make the sidebar same ht as the main
    }

    footer {
        clear: both;
    }