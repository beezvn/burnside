---
layout: master
title: Burnside Nails and Spa Beauty Salon
services: services.md
pricing: price.md

---
<!-- Page content -->
<div class="w3-content" style="max-width:1100px">

  <!-- specials -->
  <div class="w3-row w3-padding-32" id="specials">
    <div class="w3-col w3-right  w3-padding-large">
      <h2 class="w3-center"> </h2>
    </div>

   <div class="w3-col l8">
    <!-- Specials deals-->
      <div class="w3-row w3-padding-xlarge" height="500">
        <span style="font-size:20px; text-align:justify">
          {{ site.data.specials.announcement }}
        </span>
      </div>
   </div>

   <div  class="w3-col l4 w3-right">
    <div class="w3-content w3-section" style="max-width:500px" id="firstrow">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop02.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop01.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop05.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop06.png"  width="500" height="300">
    </div>        
    <div class="w3-content w3-section" style="max-width:500px" id="secondrow">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop07.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop08.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop09.png"  width="500" height="300">
          <img class="slideshow" src="{{ site.url }}/assets/images/newshop10.png"  width="500" height="300">
     </div>  
   </div>
   

  </div>

   <hr style="font-weight:bold">

  <!-- About Section -->
  <div class="w3-row w3-padding-32" id="specials">

    <div class="w3-col l6">
      <div class="w3-col m6">
      <img src="{{ site.url }}/assets/images/aboutus01.png" class="w3-round w3-image w3-right" alt="about us" width="200" height="200">
      </div>
      <div class="w3-col m6">
      <img src="{{ site.url }}/assets/images/aboutus03.png" class="w3-round w3-image" alt="about us" width="200" height="200">
      </div>
      <div class="w3-col m6">
      <img src="{{ site.url }}/assets/images/aboutus04.png" class="w3-round w3-image w3-right" alt="about us" width="200" height="200">
      </div>
      <div class="w3-col m6">
      <img src="{{ site.url }}/assets/images/aboutus02.png" class="w3-round w3-image" alt="about us" width="200" height="200">
      </div>
    </div>

   <div class="w3-col l6 w3-right">
       <div class="w3-col w3-right  w3-padding-large">
      <h2 class="w3-center">ABOUT US </h2>
    </div>
      <div class="w3-row w3-padding-xlarge" height="500">
    <span style="font-size:20px; text-align:justify">
      {{ site.data.aboutus }}
    </span>
    </div>
    </div>
  </div>

   <hr style="font-weight:bold">


  <hr>
  <!-- Services -->
  {% include {{ page.services }} %}
  <hr>

 
   <!--Reviews-->
   <div class="w3-row w3-padding-32" id="reviews">
   <div class="w3-col l12">
    <h1 class="w3-center">Feature in CliqueMag</h1><br>
   <img src="{{ site.url }}/assets/images/clique.png" class="w3-round w3-image" alt="Menu" width="auto" height="750">
   </div>
    <div class="w3-col l12">
	 <h1 class="w3-center">Reviews</h1><br>
    <img src="{{ site.url }}/assets/images/yelp.png" class="w3-round w3-image w3-right dropShadow" alt="Menu" width="auto" height="750">
   </div>
  </div>

  <hr>

  <!-- Contact Section -->
  <div class="w3-container w3-padding-32" id="contact">
  <div class="w3-col l6 w3-padding-large">
   <h1 class="w3-center">Contact us</h1><br>  
	<ul class="w3-ul w3-card-4">
    <li><h4>OPENING HOURS</h4></li>            
            <li>
            Monday - Friday: 9am - 5:30pm <br>
            Thursday: 9am - 9pm <br>
            Saturday: 9am - 5pm <br>
            Sunday : 11am - 5pm
            </li>            
            <li>Shop 67 Burnside Village, 447 Portrush Road, Glenside, SA 5065</li>
            <li>Shop 2, 398 Greenhill Road, Glenside, SA 5065</li>
            <li>Phone:  (08) 8338 6616 </li>
            <li>After hours: 0488896868 </li>
            <li>Email: customerservice@burnsidenailsandspa.com</li>
	</ul>
  </div>

<div class="w3-col l6 w3-padding-large">
<iframe
  width="500"
  height="450"
 src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3270.6807033849914!2d138.63965131617968!3d-34.939543980374005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6ab0cc03d6f8be51%3A0x894fea0e6a9342d!2sBurnside+Nails+And+Spa!5e0!3m2!1sen!2sau!4v1487130580377" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

</div>  

<!-- End page content -->
</div>

<script>

var index = 0;
carousel();

function carousel() {

    var first = $("#firstrow").children();
    var second = $("#secondrow").children();

    if (index >= first.length) {index = 0}    
    slideshow(first[index]);

    setTimeout(slideshow(second[index]), 1000);

    index++;  

    setTimeout(carousel, 2000); // Change image every 2 seconds
}

function slideshow(element){
  $(element).show();
  $(element).siblings().hide();

}

</script>

