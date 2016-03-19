---
state:
  names: [
    {name: Stephen1},
    {name: Stephen2},
    
  ]
style: |
  p{
     color: #44e544;
  }
  a{
    color: gray;
  }
---

Hi {{#names}}<b>{{name}}, </b><br>{{/names}}!

[go to the city](city)
