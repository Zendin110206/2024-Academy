Before we've make a responsive content, but how to make the web become android friendly??

We can use media query with `@media`. try adding those code to your stylesheet (style.css) and minimize your web into a smartphone size (you can use inspect element to make it more clear).

## @media Query
```css
/* for 1250px and smaller */
@media screen and (max-width: 1250px) {
    .container {
        max-width:max-content;
    }
    .myBio {
        margin-left: 2rem;
    }
}
/* for 500px and smaller */
@media screen and (max-width: 500px){
    .container {
        min-width: 300px;
    }
    nav {
        text-align: center;
        height:auto;
    }                
    .right-nav, .left-nav {
        background-color: #528aae;
        float: none;
        margin: 0%;
    }
    .right-nav a, .left-nav a {
        color: white;
        float: none;
    }
    .myPic{
        width: 250px;
    }
    .myBio {
        margin: 0 2rem;
    }
}
```

as you can't use a `1920px` appearance in your smarphone, so `@media` is needed to edit based on the width you want.

with `@media` you can set a new rules to any properties so it will fit the size of a certain devices.
