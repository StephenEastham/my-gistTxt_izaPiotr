---
init: !!js/function |
  function() {
    window.city = window.city + 1 || 1;
    if(window.city > 2) window.result = 'YOU LOSE, HAHAHAHA';
  }
state:
  numberOfViews: !!js/function |
    function() {
      return window.city;
    }
  getResult: !!js/function |
    function() {
      return window.result;
    }
style: |
  body{
    background-image: url("http://www.vectorfree.com/media/vectors/cartoon-city-skyline.jpg");
  }
---

Dear {{#names}}{{name}}{{/names}}, you are in the city! It's amazing!

Number of views: {{numberOfViews}} 

{{getResult}}

[back to index](index)