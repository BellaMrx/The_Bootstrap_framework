# The_Bootstrap_framework
 
 Introduction to the use of Bootstrap

### Contents
 1. What is Bootstrap?
 2. Download and integrate Bootstrap
 3. Create layouts with Bootstrap
 4. Use components
 
 
 
-------------------------------------------------------

## 1. What is Bootstrap?

Bootstrap is a ready-made CSS framework. Basically, it is a kind of construction kit with ready-made and dynamic design elements. Such a framework usually contains a collection of tools such as a grid layout, e.g. for responsive web design. Web typography is also an important part of such a framework. Very good and comprehensive documentation can also be found on the official website [Bootstrap](https://getbootstrap.com/).


## 2. Download and integrate Bootstrap

The first step is to download Bootstrap, which you can do here: [Bootstrap](https://getbootstrap.com/). To get started, the finished version is sufficient, which is already ready for use with CSS, JavaScript and fonts.

 <img src="images/Bootstrap_download_1.png" width="800">

 <img src="images/Bootstrap_download_2.png" width="800">

After downloading, the zip folder can be unpacked. The Bootstrap folder contains the "css" and "js" folders, each of which contains all the CSS files and JavaScript plug-ins required to use Bootstrap with an HTML document.

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_1) --> **Examples/Part_1/...** 

   ```
    <head>
        <title>Integrate Bootstrap</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <!-- integrate bootstrap css -->
        <link href="css/bootstrap.min.css" rel="stylesheet" type="text/css"> 
    </head>
    <body>
        <div class="container">
            <h1>h1. heading</h1>
            <blockquote>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere
                erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
            </blockquote>
        </div>
        <!-- integrate bootstrap js -->
        <script src="js/bootstrap.min.js" type="text/javascript"></script> 
   ```

The CSS file is inserted in the *head* area and the JavaScript file at the end of the HTML document. 

Alternatively, you can also use a CDN (Content Delivery Network). This eliminates the need to download the files. The CDN part for Bootstrap via jsDelivr looks like this:

   ```
    <!-- integrate bootstrap css -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">

    <!-- integrate bootstrap js -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
   ```

For the JavaScript functionalities of Bootstrap, the framework offers a bundle that includes Bootstrap and Popper. Popper is a JavaScript library that helps to create pop-overs etc. in web applications:

   ```
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.8/dist/umd/popper.min.js" integrity="sha384-I7E8VVD/ismYTF4hNIPjVp/Zjvgyol6VFvRkX/vR+Vc4jQkC+hVqc2pM8ODewa9r" crossorigin="anonymous"></script>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.min.js" integrity="sha384-BBtl+eGJRgqQAUMxJ7pMwbEyER4l1g+O15P+16Ep7Q9Q+zqX6gSbd85u4mG4QzX+" crossorigin="anonymous"></script>
   ```
Example:

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_2) --> **Examples/Part_2/...** 

   ```
    <head>
        <title>Integrate Bootstrap</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" 
        integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous"> 
    </head>
    <body>
        <div class="container">
            <h1>h1. heading</h1>
            <blockquote>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere
                erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
            </blockquote>
        </div>
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" 
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
    </body>
   ```

Once the files have been integrated, the framework can be used. The Bootstrap documentation can be used to find out which classes can be assigned to the elements. In the example above, for example, the entire content was packed in a `<div>` block with the bootstrap class `container`, which centers the entire content of the HTML document.


## 3. Create layouts with Bootstrap
The first step was to create an HTML framework for the web project. This is then further designed and improved with Bootstrap.

HTML basic structure without bootstrap:

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_3) --> **Examples/Part_3/...** 

   ```
   <body>
    <header>
        <h1>Title of the website</h1>
        <p>Short description of the website</p>
        <hr>
    </header>
    <nav>
        <a href="#">Home</a> |
        <a href="#">Reports</a> |
        <a href="#">Links</a> |
        <a href="#">About</a> |
        <a href="#">Contact</a>
    </nav>
    <article>
        <h2>Chicks </h2>
        <img src="../../images/chicks_480.jpg" alt="Chicks">
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
    </article>
    <article>
        <h2>Flowers </h2>
        <img src="../../images/flower_480.jpg" alt="Flowers">
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
    </article>
    <article>
        <h2>Clouds </h2>
        <img src="../../images/whale_480.jpg" alt="Clouds">
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
    </article>
    <article>
        <h2>Flora</h2>
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium
            quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
    </article>
    <article>
        <h2>Fauna</h2>
        <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium
            quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
    </article>
    <footer>
        <p>&copy; Name | <a href="#">Legal notice</a></p>
    </footer>
   </body>
   ```

 <img src="images/Bootstrap_part-3.png" width="800">
 
The same website with the use of Bootstrap:

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_4) --> **Examples/Part_4/...** 

   ```
   <head>
    <title>Bootstrap-Layout</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" 
    integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
   </head>
   <body>
    <div class="container">
        <div class="row">
            <header class="col-md-12">
                <h1>Title of the website</h1>
                <p>Short description of the website</p>
                <hr>
            </header>
        </div>
        <div class="row">
            <nav class="col-md-12">
                <a href="#">Home</a> |
                <a href="#">Reports</a> |
                <a href="#">Links</a> |
                <a href="#">About</a> |
                <a href="#">Contact</a>
            </nav>
        </div>
        <hr>
        <div class="row">
            <article class="col-md-4">
                <h2>Chicks </h2>
                <img src="../../images/chicks_480.jpg" alt="Chicks" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-md-4">
                <h2>Flowers </h2>
                <img src="../../images/flower_480.jpg" alt="Flowers" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-md-4">
                <h2>Clouds </h2>
                <img src="../../images/whale_480.jpg" alt="Clouds" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
        </div>
        <hr>
        <div class="row">
            <article class="col-md-6">
                <h2>Flora</h2>
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                    eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
            </article>
            <article class="col-md-6">
                <h2>Fauna</h2>
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                    eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
            </article>
        </div>
        <hr>
        <div class="row">
            <footer class="col-md-12 text-center">
                <p>&copy; Name | <a href="#">Legal notice</a></p>
            </footer>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" 
    integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
   </body>
   ```

 <img src="images/Bootstrap_part-4.png" width="800">

Here, the entire content is placed in the `.container` class. The layout was created line by line in this class. The `header` element was placed in the first line and the `nav` element in the next line. Both elements extend over all 12 columns of the class `.row` because of the class `.col-md-12`. In the third row, three elements with the class `.col-md-4` have been placed, each on three columns in the row. The fourth row contains two `article` elements with `.col-md-6` on two columns each. The last line contains the footer which behaves in the same way as the header. The class `.img-fluid` in `<img src="images/....jpg" alt="..." class="img-fluid">` ensures that Bootstrap automatically adjusts an image to the parent element.

With bootstraps, for example, the images are displayed side by side instead of one below the other if the screen size is wide enough. In the mobile view, the images are automatically displayed one below the other. This is an advantage of Bootstrap, as you don't have to write any media queries yourself. The viewport meta tag was added here so that zooming is possible on mobile devices.

A quick overview of how the layout is realized with Bootstrap:

1. First, it is determined whether the complete layout is to be defined in a fixed width with the class `.container` or in full width with the class `.container-fluid`. `.container` means that the value of `max-width` is reset at each breakpoint. With `.container-fluid`, on the other hand, `width: 100%;` applies to all breakpoints. If the content of the web page is packed in `.container`, it is displayed centered.

 - the complete content of a website is packaged in this way:

   ```
    <div class="container">
        ...
    </div>
   ```

2. Within the containers, the rows should be defined with the class `.row` to create horizontal groups with columns.

   ```
    <div class="container">
        <div class="row">...</div>
        <div class="row">...</div>
        ...
    </div>
   ```

3. The actual content is placed in the columns of the `.row` class. Bootstrap offers many different classes for this purpose. The grid is specified via class names, e.g. `.col-md-x`, the `x` stands for the number of 12 available columns. The `md` stands for medium-sized devices such as desktop PCs with a screen size of 768 pixels or more. If the class `.col-md-8` is used for an element, this element occupies 8 columns of the 12 available columns in a cell. If two elements with the class `.col-md-6` are packed into a row of the class `.row`, the two elements are created in two columns of the same size. The grid system of Bootstrap was realized with Flexbox.

   ```
    <div class="container">
        <div class="row">
            <header class="col-md-12">...</header>
        </div>
        <div class="row">
            <article class="col-md-4">...</article>   
            <article class="col-md-4">...</article>
            <article class="col-md-4">...</article>    
        </div>
        <div class="row">
            <article class="col-md-8">...</article> 
            <article class="col-md-4">...</article> 
        </div>
        ...
    </div>
   ```

Bootstrap offers even more raster classes besides `.col-md-x`. There are also the classes `.col-xs-x`, `.col-sm-x` and `.col-lg-x`, which work accordingly on the different devices.

| Class Prefix | Device       |
| ------------ | ------------ |
| `.col-xs-`      | extra-small devices such as smartphones with a screen smaller than 576 px |
| `.col-sm-`   | small devices such as smartphones or tablets with a screen size greater than or equal to 576 px |
| `.col-md-`   | medium-sized devices such as tablets or desktop PCs with a screen size greater than or equal to 768px |
| `.col-lg-`   | large devices such as tablets or desktop PCs with a screen size greater than or equal to 960 px |
| `.col-xl-`   | large devices such as desktop PC with a screen larger than or equal to 1200 px |
| `.col-xxl-`  | extra-large devices such as desktop PCs with a screen larger than or equal to 1400 px |

The class `.col-md-x` is used to create a basic column grid whose columns are arranged one above the other on smartphones and narrow tablets and next to each other from medium screen sizes.

If the elements are not simply to be arranged on top of each other on the tablet, the arrangement can be changed with the device grid class `.col-sm-x`:

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_5) --> **Examples/Part_5/...** 

   ```
    <div class="container">
        <div class="row">
            <header class="col-md-12">
                <h1>Title of the website</h1>
                <p>Short description of the website</p>
                <hr>
            </header>
        </div>
        <div class="row">
            <nav class="col-md-12">
                <a href="#">Home</a> |
                <a href="#">Reports</a> |
                <a href="#">Links</a> |
                <a href="#">About</a> |
                <a href="#">Contact</a>
            </nav>
        </div>
        <hr>
        <div class="row">
            <article class="col-sm-6 col-md-4">
                <h2>Chicks </h2>
                <img src="../../images/chicks_480.jpg" alt="Chicks" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-sm-6 col-md-4">
                <h2>Flowers </h2>
                <img src="../../images/flower_480.jpg" alt="Flowers" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-sm-12 col-md-4">
                <h2>Clouds </h2>
                <img src="../../images/whale_480.jpg" alt="Clouds" class="img-fluid">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
        </div>
        <hr>
        <div class="row">
            <article class="col-md-6">
                <h2>Flora</h2>
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                    eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
            </article>
            <article class="col-md-6">
                <h2>Fauna</h2>
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                    eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. <br><a href="#">Read more ...</a></p>
            </article>
        </div>
        <hr>
        <div class="row">
            <footer class="col-md-12 text-center">
                <p>&copy; Name | <a href="#">Legal notice</a></p>
            </footer>
        </div>
    </div>
   ```

 <img src="images/Bootstrap_part-5.png" width="500">

The display of the website is automatically adjusted again on larger screens.


### Show and hide elements with the help of Bootstrap

Bootstrap provides ready-made (helper) classes for different display window sizes for showing and hiding elements. For example, to show and hide individual graphics for a smartphone version, the class `.d-none-{value}` or `.d-{value}-block` (d = display) can be used. For *value*, `sm`, `md`, `lg` and `lx` must be used according to the screen size. To hide elements for small screens only, `.d-none .d-sm-block` is used: 

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_6) --> **Examples/Part_6/...** 

   ```
    ...
    <div class="container">
        <div class="row">
            <header class="col-md-12">
                <h1 class="d-none d-sm-block">Title of the website</h1>
                <p class="d-none d-sm-block">Short description of the website</p>
                <img src="logo.png" alt="Logo" class="img-fluid d-block d-sm-none">
                <hr>
            </header>
        </div>
        <div class="row">
            <nav class="col-md-12">
                <a href="#">Home</a> |
                <a href="#">Reports</a> |
                <a href="#">Links</a> |
                <a href="#">About</a> |
                <a href="#">Contact</a>
            </nav>
        </div>
        <hr>
        <div class="row">
            <article class="col-sm-6 col-md-4">
                <h2>Chicks </h2>
                <img src="../../images/chicks_480.jpg" alt="Chicks" class="img-fluid d-none d-sm-block">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-sm-6 col-md-4">
                <h2>Flowers </h2>
                <img src="../../images/flower_480.jpg" alt="Flowers" class="img-fluid d-none d-sm-block">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
            <article class="col-sm-12 col-md-4">
                <h2>Clouds </h2>
                <img src="../../images/whale_480.jpg" alt="Clouds" class="img-fluid d-none d-sm-block">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. <a href="#">Read more ...</a></p>
            </article>
        </div>
     ...
    </div>
   ```

 <img src="images/Bootstrap_part-6a.png" width="800">

 <img src="images/Bootstrap_part-6b.PNG" width="300">


## 4. Use components

Bootstrap offers a large number of ready-made components such as icons, menus, warnings, cards, labels and navigation bars.

### Integrate a navigation
There are several options for navigations, e.g. tabs, pills or navbars:

Pills are navigation points that look like buttons. Here is an example with pills and a dropdown menu:

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_7) --> **Examples/Part_7/...** 

   ```
    ...
        <div class="row">
            <nav class="col-sm-8 col-md-8">
                <ul class="nav nav-pills">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Reports</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Links</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#">
                          Contact</a>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#">E-Mail</a></li>
                            <li><a class="dropdown-item" href="#">Social Media</a></li>
                            <li><a class="dropdown-item" href="#">Legal notice</a></li>
                        </ul>
                    </li>
                </ul>
            </nav>
        </div>
    ...
   ```

 <img src="images/Bootstrap_part-7a.png" width="800">

Here, the navigation points were simply packed into an unordered list with the class `.nav`. The navigation points are displayed as pills with the class `.nav-pills`. The active navigation point is marked with the class `.active`.

If the navigation points are to be displayed as tabs, simply change `.nav-pills` to `.nav-tabs`.

 <img src="images/Bootstrap_part-7b.png" width="800">

The drop-down menu is realized with the class `.drop-down` and it is controlled with `data-bs-toggle="dropdown"`.

 <img src="images/Bootstrap_part-7c.png" width="800">

The attributes that begin with the prefix `data`- are HTML attributes that were introduced with HTML5. This allows custom data to be saved with an HTML element without there being a defined HTML attribute for it. With `data-bs-toggle`, the element was linked to the corresponding widget, in this case the drop-down menu.

It is also possible to define your own attributes, simply preceded by `data`:

   ```
    <li data-birth-year="1879">Albert Einstein</li>
    <li data-birth-year="1856">Nikola Tesla</li>
   ```

JavaScript can be used to access the values of your own `data` attributes with `dataset`:

   ```
    let scientist = document.getElementsByTagName('li');
    // The hyphen in HTML must be displayed in JavaScript as camel case notation birth-year = birthYear
    console.log(scientist[0].dataset['birthYear']);
   ```


#### Add a navigation bar
A complete navigation bar can be realized with `.navbar`, on which other elements such as input fields, buttons and drop-down menus can also be placed. On wide screens, the navigation is displayed as a bar and on smartphones it is minimized and can be folded in and out using a button.

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_8) --> **Examples/Part_8/...** 

   ```
    ...
        <div class="row">
            <nav class="navbar navbar-expand-lg navbar-light bg-light col-sm-12 mb-2">
                <a class="navbar-brand" href="#">Navigation</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent">
                  <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav mr-auto">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">Home 
                      </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Reports</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Links</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown">
                        Contact
                      </a>
                            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                                <a class="dropdown-item" href="#">E-Mail</a>
                                <a class="dropdown-item" href="#">Social Media</a>
                                <a class="dropdown-item" href="#">Legal notice</a>
                            </div>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    ...
   ```

 <img src="images/Bootstrap_part-8a.png" width="800">

 <img src="images/Bootstrap_part-8b.PNG" width="300">

The navbar is introduced with `.navbar` and `.navbar-expand-lg` in the `nav` element. When the navigation is collapsed can be specified with `.navbar-expand-lg`, another value is also possible here instead of `lg` (`-sm`, `-md`, -`lg`, `-xl`). The navbar for the mobile version is introduced with `.navbar-toggler`. The button activates the JavaScript `colapse`, which expands the navigation bar and has the element with the ID `#navbarSupportContent` as target with `data-bs-target`. The icon with the three dashes is inserted by the class `.navbar-toggler-icon`. The title is created with `.navbar-brand`.


### Cards
Cards are flexible and expandable containers with many options for content and with headers and footers.

 [Complete Code](https://github.com/BellaMrx/The_Bootstrap_framework/tree/main/Examples/Part_9) --> **Examples/Part_9/...** 

   ```
    ...
        <div class="row">
            <article class="col-sm-6 col-md-4">
                <div class="card">
                    <!--<div class="card-body">-->
                    <h5 class="card-header">Chicks </h5>
                    <img src="../../images/chicks_480.jpg" alt="Chicks" class=" card-img-top img-fluid d-none d-sm-block">
                    <p class="card-text m-2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. </p>
                    <a href="#" class="btn btn-primary">Read more ...</a>
                    <!--</div>-->
                </div>
            </article>
            <article class="col-sm-6 col-md-4">
                <div class="card">
                    <!--<div class="card-body">-->
                    <h5 class="card-header">Flowers </h5>
                    <img src="../../images/flower_480.jpg" alt="Flowers" class="card-img-top img-fluid d-none d-sm-block">
                    <p class="card-text m-2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa.</p>
                    <a href="#" class="btn btn-primary">Read more ...</a>
                    <!-- </div>-->
                </div>
            </article>
            <article class="col-sm-12 col-md-4">
                <div class="card">
                    <!-- <div class="card-body">-->
                    <h5 class="card-header">Clouds </h5>
                    <img src="../../images/whale_480.jpg" alt="Clouds" class="card-img-top img-fluid d-none d-sm-block">
                    <p class="card-text m-2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa.</p>
                    <a href="#" class="btn btn-primary">Read more ...</a>
                    <!--</div>-->
                </div>
            </article>
        </div>
        <hr>
        <div class="row">
            <article class="col-md-6">
                <div class="card">
                    <!--<div class="card-body">-->
                    <h5 class="card-header">Flora</h5>
                    <p class="card-text m-2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                        eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa.</p>
                    <a href="#" class="btn btn-primary">Read more ...</a>
                    <!--</div>-->
                </div>
            </article>
            <article class="col-md-6">
                <div class="card">
                    <!--div class="card-body">-->
                    <h5 class="card-header">Fauna</h5>
                    <p class="card-text m-2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque
                        eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut. Aenean massa. </p>
                    <a href="#" class="btn btn-primary">Read more ...</a>
                    <!--</div>-->
                </div>
            </article>
        </div>
    ...
   ```

 <img src="images/Bootstrap_part-9a.png" width="800">

 <img src="images/Bootstrap_part-9b.PNG" width="300">

Cards are created with the class `.card`. With `.card-body` another block can be created within `.card` to create a padding within a card container. The size of a card container is always 100% unless otherwise specified.

## The End

This is just an introduction to using the Bootstrap framework, there are many more ways to create simple and beautiful website layouts. A complete overview can be found in the very good documentation of [Bootstrap](https://getbootstrap.com/). 

If you don't know HTML, CSS or JavaScript yet, have a look here:
  - [WebDevelopment Basics](https://github.com/BellaMrx/WebDevelopment_Basics) - Basics Guide for web developers
  - [HTML Guide](https://github.com/BellaMrx/HTML_Guide) - Detailed guide about HTML5 (all basics for HTML)
  - [HTML Cheat Sheets](https://github.com/BellaMrx/HTML_Cheat_Sheets) - All HTML5 elements and their attributes
  - [CSS Guide](https://github.com/BellaMrx/CSS_Guide) - Detailed guide about CSS (Introduction to CSS, CSS Selectors, Inheritance and the cascade, CSS Box Model, CSS Positioning, Flexbox, Responsive Web Design, CSS Grid Layout, Styling with CSS, Testing and Organizing) 
  - [Sass and SCSS Basic Guide](https://github.com/BellaMrx/Sass_and_SCSS) - An introduction to the CSS preprocessor Sass

  **JavaScript Basics:**

  1. [JS Introduction](https://github.com/BellaMrx/JS_introduction) - An introduction to JavaScript
  2. [Arrays, functions, objects in JS](https://github.com/BellaMrx/Arrays_functions_objects_in_JS) - Introduction: Arrays, functions and objects in JavaScript
  3. [DOM - Document Object Model](https://github.com/BellaMrx/DOM_Document-Object-Model) -  Introduction to the **DOM** and the **DOM** manipulation - Change web pages dynamically  
  4. [Introduction to Web APIs](https://github.com/BellaMrx/JavaScript_Introduction-To-Web-APIs)
  5. [Introduction to Ajax and jQuery](https://github.com/BellaMrx/JavaScript_Introduction_to_Ajax_and_jQuery)
  6. You are here --> [Introduction to Bootstrap framework](https://github.com/BellaMrx/The_Bootstrap_framework)

Or just visit my GitHub profile, you can find all guides/tutorials there [BellaMrx](https://github.com/BellaMrx)

Thanks for the attention.

#### This is the end, beautiful friend... ;)







