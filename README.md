<html>
<title>Mainland China </title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>
body, html {
  height: 100%;
  font-family: "Calibri", sans-serif;
}

.bgimg {
  background-position: center;
  background-size: cover;
  min-height: 75%;
}

.menu {
  display: none;
}
</style>
<body>

<!-- Links (sit on top) -->
<div class="w3-top">
  <div class="w3-row w3-padding w3-black">
    <div class="w3-col s3">
      <a href="#" class="w3-button w3-block w3-grey">HOME</a>
    </div>
    <div class="w3-col s3">
      <a href="#about" class="w3-button w3-block w3-black">ABOUT</a>
    </div>
    <div class="w3-col s3">
      <a href="#menu" class="w3-button w3-block w3-grey">MENU</a>
    </div>
    <div class="w3-col s3">
      <a href="#where" class="w3-button w3-block w3-black">WHERE</a>
    </div>
  </div>
</div>

<!-- Header with image -->
<header class="bgimg w3-display-container w3-grayscale-min" id="home">
  <div class="w3-display-bottomleft w3-center w3-padding-large w3-hide-small">
    <span class="w3-tag">Open from 11 am to 6 pm </span>
  </div>
  <div class="w3-display-middle w3-center">
    <span class="w3-text-white" style="font-size:90px"> Mainland <br> China </span>
  </div>
  <div class="w3-display-bottomright w3-center w3-padding-large">
    <span class="w3-text-white">4th Floor, Acropolis Mall, Rajdanga Main Rd, Kolkata </span>
  </div>

<!-- Add a background color and large text to the whole page -->
<div class="w3-sand w3-grayscale w3-large">

<!-- About Container -->
<div class="w3-container" id="about">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-64"><span class="w3-tag w3-wide">About Mainland China  </span></h5>
    <p> Mainland China restraunt series was a brand first started in Mumbai by Anjan Chatterjee. This chain serves mainly chinese and mediterinian food items.  </p>
    
    <div class="w3-panel w3-leftbar w3-light-grey">
    
      <p> Founder : Anjan Chatterjee </p>
    </div>
   
    <p><strong>Opening hours:</strong> Open from 11 am to 6 pm</p>
    <p><strong>Address:</strong>4th Floor, Acropolis Mall, Rajdanga Main Rd, Kolkata </p>
  </div>
</div>

Some of the items in the menu are listed below :

<!-- Menu Container -->
<div class="w3-container" id="menu">
  <div class="w3-content" style="max-width:700px">
 
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">THE MENU</span></h5>
  
    <div class="w3-row w3-center w3-card w3-padding">
      <a href="javascript:void(0)" onclick="openMenu(event, 'Starters');" id="myLink">
        <div class="w3-col s6 tablink">Starters</div>
      </a>
      <a href="javascript:void(0)" onclick="openMenu(event, 'Apetizers');">
        <div class="w3-col s6 tablink">Apetizers</div>
      </a>
    </div>

    <div id="Starters" class="w3-container menu w3-padding-48 w3-card">
      <h5>Truffle Oil INfused Edamame Dumplings </h5> 
    
      <h5>Corn and Water Chestnut Dumplings </h5>
  
      <h5>Basil Flavoured Vegetable Dumplings </h5>
    
      
    </div>

    <div id="Apetizers" class="w3-container menu w3-padding-48 w3-card">
      <h5>Crispy Corn Cubes </h5>
    
    
      <h5>Cracking Spinach</h5>
   
      <h5>Crispy Corn Chilly Pepper  </h5>
     
      <h5>Ginger Chilly Cauliflower </h5>
      
      <h5>Stri Fried Vegetables with spices </h5>
    
    </div>  
   
  </div>
</div>

<!-- Contact/Area Container -->
<div class="w3-container" id="where" style="padding-bottom:32px;">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">WHERE TO FIND US</span></h5>
    <p>Find us at the address mentioned above</p>
 
    
    <p><strong>Reserve</strong> a table, ask for today's special or just send us a message:</p>
    <form action="/action_page.php" target="_blank">
      <p><input class="w3-input w3-padding-16 w3-border" type="text" placeholder="Name" required name="Name"></p>
      <p><input class="w3-input w3-padding-16 w3-border" type="number" placeholder="How many people" required name="People"></p>
      <p><input class="w3-input w3-padding-16 w3-border" type="datetime-local" placeholder="Date and time" required name="date" value="2020-11-16T20:00"></p>
      <p><input class="w3-input w3-padding-16 w3-border" type="text" placeholder="Message \ Special requirements" required name="Message"></p>
      <p><button class="w3-button w3-black" type="submit">SEND MESSAGE</button></p>
    </form>
  </div>
</div>

<!-- End page content -->
</div>

<script>
// Tabbed Menu
function openMenu(evt, menuName) {
  var i, x, tablinks;
  x = document.getElementsByClassName("menu");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < x.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" w3-dark-grey", "");
  }
  document.getElementById(menuName).style.display = "block";
  evt.currentTarget.firstElementChild.className += " w3-dark-grey";
}
document.getElementById("myLink").click();
</script>


