---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# <i class="fas fa-envelope"></i>Contact

{%
  include link.html
  type="email"
  icon=""
  text="subrata@nitp.ac.in"
  tooltip=""
  link="subrata@nitp.ac.in"
  style="button"
%}

Our lab is part of the [Department of Applied Physics and Materials Engineering](https://www.nitp.ac.in/Department/Phy), at the [National Institute of Technology Patna](https://www.nitp.ac.in/). Our lab is nestled on the bank of the river Ganga, Eastern zone of India. 

### <i class="fas fa-mail-bulk"></i>Mailing Address

Department of Applied Physics and Materials Engineering, NIT Patna, Ashok Rajpath, Patna 800 005, Bihar, India


### <i class="fas fa-mail-bulk"></i>Mailing

webix.ui({
  // provide your own Google API key
  // https://developers.google.com/maps/documentation/javascript/get-api-key
  key:"AIzaSyAi0oVNVO-e603aUY8SILdD4v9bVBkmiTg",
  view:"google-map",
  id:"map",
  zoom:6,
  center:[25.6196306,85.1702235]
});

$$("map").getMap(true).then((map) => {
  var currentPosition = map.getCenter();
  let img = `http://maps.google.com/maps/api/staticmap?sensor=false&center=${currentPosition.lat()},${currentPosition.lng()}&zoom=${map.getZoom()}&size=512x512&markers=color:green|label:X|${currentPosition.lat()},${currentPosition.lng()}&key=${$$("map").config.key}`;
  console.log(img);
});

 
{:.center}
