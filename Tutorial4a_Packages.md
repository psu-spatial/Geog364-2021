---
title: "Tutorial 4: Packages and Libraries"
subtitle: <h4 style="font-style:normal">GEOG-364 - Spatial Analysis</h4>
output: 
  html_document:
    toc: true
    toc_depth: 3
    toc_float: true
    theme: flatly
    code_folding: show
---

<style>
p.comment {
background-color: #DBDBDB;
padding: 10px;
border: 1px solid black;
margin-left: 25px;
border-radius: 5px;
font-style: normal;
}


</style>

<style type="text/css">
#TOC {
  font-size: 13px;
  font-family: Arial;
}
</style>


\


### Packages

R is open source, meaning that anyone can create their own commands.  Over the years, the number of commands available has risen to several million!  

This is too many to store on your computer, so most live on the internet, grouped together into collections, known as "packages" or "libraries". Sometime packages contain cool datasets. 

A close analogy is your phone.  There are millions of apps available from banking, to social media to camera filters.  You don't have every app in the world installed on your phone - and you don't have every app you *do* download running at the same time.  Instead you download the apps that you think you will need (occasionally downloading a new one on the fly) - and when you need to use an app, you click on it to open.

R is just the same. We have

 - R: The programming language itself
 - Functions: Specific commands or actions written in the R language
 - Packages/libraries: Commands are grouped into bundles by theme (dplyr makes table commands easier, bardr contains the full works of William Shakespeare as a test dataset..)
 
You can see the full available list here: https://cran.r-project.org/web/packages/available_packages_by_name.html

If you look at the packages tab next to the plot one, you can see which ones are already preinstalled onto your computer 

### How to download/install packages

Just as you don't need to go to the app store every time you use your weather app, you only need to download and install packages once.  There are two methods

1. Clicking the INSTALL button in the Packages tab, then start typing the package name and it will show up (check the include dependencies box).
2. In the console, run the `install.packages()` command with quotes around the package name e.g. `install.packages("bardr")`.

Try installing the bardr package onto your computer

<br>

<div style="margin-bottom:25px;">
</div>
### How to load packages you want to use

Installing a package doesn't make it available to you.  For that you need to load it (like clicking on an app).  This can be done with the library command.  In the console type




If you have managed to install them successfully, often nothing happens - this is great!  It means it loaded the package without errors.

Sometimes, it will tell you friendly messages.  For example, this is what shows up when you install the tidyverse package.  The computer telling you the sub-packages that it downloaded and also that some commands, like filter - now have a different meaning.  E.g. originally the filter command did one thing, but now the tidyverse package has made filter do something else.

<div class="figure">
<img src="Tutorial4a_fig1_tidyversetext.png" alt="Tidyverse install messages" width="1532" />
<p class="caption">Tidyverse install messages</p>
</div>

**To find out if what you are seeing is a friendly message or an error, run the command again.  If you run it a second time and there is no error then nothing should happen.**


***



Website created and maintained by [Helen Greatrex](https://www.geog.psu.edu/directory/helen-greatrex). Website template by [Noli Brazil](https://nbrazil.faculty.ucdavis.edu/)