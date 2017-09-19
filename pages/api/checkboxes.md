---
title: Checkboxes
tags: 
keywords:
summary: 
sidebar: mydoc_sidebar
permalink: checkboxes.html
folder: mydoc
toc: false
---

## Data is saved locally:

<input type="checkbox" value="chB1" /> Checkbox 1<br />
<input type="checkbox" value="chB2" /> Checkbox 2<br />
<input type="checkbox" value="chB3" /> Checkbox 3<br />
<input type="checkbox" value="chB4" /> Checkbox 4<br />
<input type="checkbox" value="chB5" /> Checkbox 5<br /> 
<br />
<button onclick="save()">SAVE</button> <button onclick="load_()">LOAD</button> 


 <script>
      var i, checkboxes = document.querySelectorAll('input[type=checkbox]');

function save() {
    for (i = 0; i < checkboxes.length; i++) {
        localStorage.setItem(checkboxes[i].value, checkboxes[i].checked); 
    }
}

function load_() {
    for (i = 0; i < checkboxes.length; i++) {
        checkboxes[i].checked = localStorage.getItem(checkboxes[i].value) === 'true' ? true:false;
    }
} 

    </script>

{% include links.html %}

