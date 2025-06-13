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

{%
  include gallery.html
  image1="images/action/transmission_tree.jpg"
  link1="research"
  tooltip1="Our research"
  image2="images/action/xxxxxxxxx.jpg"
  link2="opportunities"
  tooltip2="Join us!"
%}

{% include gallery.html image1="images/action/transmission_tree.jpg" link1="<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3597.557068566589!2d85.1702235253957!3d25.61963062744144!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39ed58dce6732867%3A0x4059f39a1ac82f06!2sNational%20Institute%20of%20Technology%2C%20Patna!5e0!3m2!1sen!2sin!4v1749801424450!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>" tooltip1="Our research"}

### <i class="fas fa-mail-bulk"></i>Location
{:.center}
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


### <i class="fas fa-mail-bulk"></i>Mailing

Department of Applied Physics and Materials Engineering, 


### <i class="fas fa-mail-bulk"></i>Mailing Address

Department of Applied Physics, and Materials Engineering, NIT Patna, Ashok Rajpath, Patna 800 005, Bihar, India
{:.center}
