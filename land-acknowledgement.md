---
layout: default
nav_order: 20
title: Land acknowledgement 
---
# Land acknowledgement

We acknowledge the indigenous lands where we are located.    

We acknowledge and respect the lək̓ʷəŋən peoples on whose traditional territory the university stands and the Songhees, Esquimalt and W̱SÁNEĆ peoples whose historical relationships with the land continue to this day.
<iframe src="https://native-land.ca/api/embed/embed.html?maps=territories&position=48.4634,-123.3117" style="width:100%; height:500px; border:none;"></iframe>

Visit [native-land.ca](https://native-land.ca/) to explore the indigenous territories, languages, and treaties in your area.

<script>
function includeHTML() {
  var z, i, elmnt, file, xhttp;
  /*loop through a collection of all HTML elements:*/
  z = document.getElementsByTagName("*");
  for (i = 0; i < z.length; i++) {
    elmnt = z[i];
    /*search for elements with a certain atrribute:*/
    file = elmnt.getAttribute("w3-include-html");
    if (file) {
      /*make an HTTP request using the attribute value as the file name:*/
      xhttp = new XMLHttpRequest();
      xhttp.onreadystatechange = function() {
        if (this.readyState == 4) {
          if (this.status == 200) {elmnt.innerHTML = this.responseText;}
          if (this.status == 404) {elmnt.innerHTML = "Page not found.";}
          /*remove the attribute, and call this function once more:*/
          elmnt.removeAttribute("w3-include-html");
          includeHTML();
        }
      }      
      xhttp.open("GET", file, true);
      xhttp.send();
      /*exit the function:*/
      return;
    }
  }
};
</script>
  
<div w3-include-html="https://richmccue.github.io/"></div>
  
<script>
includeHTML();
</script>
