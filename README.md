# JQueryBasics
Dollar Sign ($)
The original jQuery code is like this

jQuery(document).ready(function(){
    //do something here..
});

By default, jQuery uses "$" as a shortcut for "jQuery" (replace jQuery with dollar sign)

$(document).ready(function(){
    //do something here..
});

Using javascript built-in function to select element

<div id="ele">This is a test</div>
var e = document.getElementById("ele");

Using jQuery to select element

<div id="ele">This is a test</div>
var e = $("#ele");

 
Document Ready
Most of the time we want to run javascripts on page load, we could write the code like this

window.onload = function(){ 
    alert("Document ready!"); 
}

But there is a catch, window.onload only get triggered when all assets(e.g. images) are loaded, what if we
want to run the codes as soon as DOM hierarchy has been fully constructed? you could use the code like this

$(document).ready(function(){
    //run your code here
});

 
id selector(#id)
jQuery uses id attribute to identify each unique element throughout the page.
