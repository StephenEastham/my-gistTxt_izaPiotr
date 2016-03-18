---
init:
  function() {
    window.city = window.city + 1 || 1;
  }
state:
  numberOfViews: !!js/function |
    function() {
      return window.city;
    }
style: |
  body{
    background-image: url("http://www.vectorfree.com/media/vectors/cartoon-city-skyline.jpg");
  }
---

Dear {{name}}, you are in the city! It's amazing!

Number of views: {{numberOfViews}}

[back to index](index)