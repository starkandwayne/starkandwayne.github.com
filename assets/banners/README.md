# Slider images

Slider images run across the top of many pages of the site. They are 450px high and wider than any screen resolution, say 1400px+. When the page has multiple slides, the banner/slider will slide across to reveal more of the scene.

## To add sliders

* Find a nice image that is 1400px+ and crop it to 450px high.
* Store it in this `articles/banner` folder.
* In `parallax-slider.css`, add a CSS class as below, replacing NAME with a useful name.

``` css
.da-slider-NAME{
  background: transparent url(/assets/banners/NAME.png) repeat 0% 0% !important;
}
```

The slider can now be used in posts and pages with a YAML header such as:

``` yaml
---
layout: post
banner:
  background: NAME
  title: "The slide title"
  text: The slide text
theme:
  name: smart-business-template
...
---
...
```