# EXP 03 - CREATE A WEB-LAYOUT USING FLEXBOX

## AIM:
To create a web-layout using flexbox.

## SOFTWARE:

Visual Studio Code

## ALGORITHM:

1) Create a new HTML file or open an existing one.Add the necessary HTML elements to represent your layout sections, such as header, sidebar, main content, and footer.
2) Give each section a meaningful class or ID to target them in CSS.
3) Open your CSS file or add a style block within the HTML file.Set the display property of the parent container to display flex. This activates Flexbox layout for the container.
4) Optionally, adjust the flex-direction property to control the flow of elements. The default value is row, which creates a horizontal layout. Other options are column, row-reverse, and column-reverse.
5) Add additional CSS properties as needed, such as width, height, background color, and margins, to style the container and its child elements.
6) Organize the child elements
7) Check if the layout behaves as expected and adjusts correctly on different screen sizes.
8) Make any necessary adjustments to the Flexbox properties or additional CSS styles.
Repeat the testing and iteration process until the layout meets your requirements.

## PROGRAM:

java

<!doctype html>
<title>Example</title>
<style>
  * {
    box-sizing: border-box; 
  }
  body {
    display: flex;
    min-height: 100vh;
    flex-direction: column;
    margin: 0;
  }
  #main {
    display: flex;
    flex: 1;
  }
  #main > article {
    flex: 1;
    order: 1;
  }
  #main > nav, 
  #main > aside {
    flex: 0 0 20vw;
  }
  #main > nav {
    background: #D7E8D4;
    order: 3;
  }
  #main > aside {
    background: beige;
    order: 2;
  }
  header, footer {
    background: yellowgreen;
    height: 20vh;
  }
  header, footer, article, nav, aside {
    padding: 1em;
  }
</style>
<body>
  <header>Header</header>
  <div id="main">
    <article>Article</article>
    <nav>Nav</nav>
    <aside>Aside</aside>
  </div>
  <footer>Footer</footer>
</body>


## OUTPUT:

<img width="1280" alt="image" src="https://github.com/Monisha-11/EXP-03---MODERN-WEB/assets/93427240/b3a35b2d-cddd-4101-95c6-0900a6f2ab1b">

## RESULT:

Thus the web-layout using flexbox is created.
