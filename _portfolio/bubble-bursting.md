---
title: "The Scheming Admin"
excerpt: "A managerial dashboard implemented as an embedded Shopify application with advanced administrative functionalities."
header:
  teaser: assets/images/the-scheming-admin/home-page.png
resources:
  - name: "Desktop Demo Video"
    src: "https://github.com/madisonthantu/about_mgt/raw/gh-pages/assets/videos/the-scheming-admin-desktop-demo.mov"
  - name: "Desktop View"
    src: "https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/images/the-scheming-admin/desktop-view.png"
  - name: "Mobile Demo Video"
    src: "https://github.com/madisonthantu/about_mgt/raw/gh-pages/assets/videos/the-scheming-admin-mobile-demo.MP4"
  - name: "Mobile View"
    src: "https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/images/the-scheming-admin/mobile-view.jpeg"
---

![The Scheming Admin Home Page.](https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/images/the-scheming-admin/home-page.png)

Implemented as an independent freelance shopify developer, working for [Roses del Fuego](https://rosesdelfuego.com/).

**The Scheming Admin** is a managerial dashboard implemented as an embedded Shopify application with advanced administrative functionalities customized to the business use cases and needs of a startup flower company.

The GitHub repo is private and can be made (partially) available upon request.

### Key custom features include:
- The implementation of custom data fields (e.g., delivery date, packaging date, product name used by distributor, etc.)
- The automatic updating of these custom data fields upon: (a) installation of the app by a new/former shopify storefront, and (b) upon the creation of new or modification of existing orders and products. This was accomplished via the usage of the Shopify Flow platform (e.g., triggers, actions), GraphQL Admin API, and webhook subscriptions.
- The ability to render and export specific resources relevant to business needs. For each order, the administrator can format and print the personalized note, if included, print the shipping label. The administrator is also able to export all/selected/current page orders to .csv or .xlsx files, with the relevant information (e.g., packing date, delivery date) present.
- The deployment of the embedded web app, hosted on `fly.io`. 

### Tech specs:
    Shopify API, GraphQL, React, JavaScript, Polaris, Liquid,
    SQLite, Prisma, Fly.io, REMIX web framework, Shopify App Bridge


### Demos & Views:
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<body>
  <div>
    <div id="myCarousel" class="carousel slide" data-ride="carousel">
      <!-- Indicators -->
      <ol class="carousel-indicators">
        <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        <li data-target="#myCarousel" data-slide-to="1"></li>
        <li data-target="#myCarousel" data-slide-to="2"></li>
        <li data-target="#myCarousel" data-slide-to="3"></li>
      </ol>
      <!-- Wrapper for slides -->
      <div class="carousel-inner">
        <div class="item active" style="left:2%;">
          <h3 style="color:#30CECE;text-align:center;">{{page.resources[0].name}}</h3>
          <a href="https://drive.google.com/file/d/1H0pN1JSlHa3O0XUFmrCSmg9QVMIaX-ON/view?usp=sharing">
            <video src="{{page.resources[0].src}}" alt="{{page.resources[0].name}}" style="width:95%;" controls></video>
          </a>
        </div>
        <div class="item" style="left:2%;">
          <h3 style="color:#30CECE;text-align: center;">{{page.resources[1].name}}</h3>
          <a href="https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/images/the-scheming-admin/desktop-view.png">
            <img src="{{page.resources[1].src}}" alt="{{page.resources[1].name}}" style="width:95%;">
          </a>
        </div>
        <div class="item" style="left:37%;">
          <h3 style="color:#30CECE;">{{page.resources[2].name}}</h3>
          <a href="https://drive.google.com/file/d/1LsAS9_HrJ4Sv-J0veNhwkHd_MeT5gePH/view?usp=sharing">
            <video src="{{page.resources[2].src}}" alt="{{page.resources[2].name}}" style="width:28%;" controls></video>
          </a>
        </div>
        <div class="item" style="left:37%;">
          <h3 style="color:#30CECE;">{{page.resources[3].name}}</h3>
          <a href="https://raw.githubusercontent.com/madisonthantu/about_mgt/gh-pages/assets/images/the-scheming-admin/mobile-view.jpeg">
            <img src="{{page.resources[3].src}}" alt="{{page.resources[3].name}}" style="width:28%;">
          </a>
        </div>
      <!-- Left and right controls -->
      <a class="left carousel-control" href="#myCarousel" data-slide="prev">
        <span class="glyphicon glyphicon-chevron-left"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="right carousel-control" href="#myCarousel" data-slide="next">
        <span class="glyphicon glyphicon-chevron-right"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
