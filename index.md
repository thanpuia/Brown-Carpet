<!DOCTYPE html>
<html lang="en">
<head>
	<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">

     <title>Make me rich</title>
<!-- 

Get Ready Template

https://templatemo.com/tm-521-get-ready

-->
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="team" content="">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/vegas.min.css">
     <link rel="stylesheet" href="css/font-awesome.min.css">

     <!-- MAIN CSS -->
     <link rel="stylesheet" href="css/templatemo-style.css">

</head>
<body>
     <!-- HOME -->
     <section id="home">
        <div class="overlay"></div>
          <div class="container">
               <div class="row">

                    <div class="col-md-12 col-sm-12 ">
                         <div class="home-info">
                              <h1 style="font-size:80px;">Make me rich quick</h1><br>
							  
                              <!-- You can change the date time in init.js file -->
							  		
							

                              <ul class="countdown">
							   <h5>Please sent money.More or less whatever. But more will be very good, hah. And I will spend it happily</h5>

							    <h2>But, if it exceed <b>$13,456.78</b> within </h2>

                                   <li>
                                        <span class="days">14</span>
                                        <h3>Days</h3>
                                   </li>
                                   <li>
                                        <span class="hours">10</span>
                                        <h3>hours</h3>
                                   </li>
                                   <li>
                                        <span class="minutes">15</span>
                                        <h3>minutes</h3>
                                   </li>
                                   <li>
                                        <span class="seconds">34</span>
                                        <h3>seconds</h3>
                                   </li>   
							  <br><h4>every money send will go help feed the need, seriously</h4>								   
                              </ul>
							
                             <a href="#pay">I will give you my money :)</a>
                         </div>
                    </div>

               </div>
          </div>
     </section>
	<div  id="pay" 	class="row m-5 mb-100">
							
								
			<div class="col">
				<div class="card" style="width: 25rem;">
				  <img class="card-img-top p-3" src="images/1.jpg" alt="Card image cap">
				  <div class="card-body">
					<h5 class="card-title">I give you <b>$1</b> happily</h5>
					<p class="card-text"></p>
					<div id="paypal-button-container_1"></div>
				  </div>
				</div>
			
			</div>
			
			<div class="col">
				<div class="card" style="width: 25rem;">
				  <img class="card-img-top p-3" src="images/10.jpg" alt="Card image cap">
				  <div class="card-body">
					<h5 class="card-title">I give you<b> $10</b> happily</h5>
					<p class="card-text"></p>
					<div id="paypal-button-container_10"></div>
				  </div>
				</div>
			
			</div>
			
			<div class="col">
				<div class="card" style="width: 25rem;">
				  <img class="card-img-top p-3" src="images/100.jpg" alt="Card image cap">
				  <div class="card-body">
					<h5 class="card-title">I give you <b>$100 </b>happily</h5>
					<p class="card-text"></p>
					<div id="paypal-button-container_100"></div>
				  </div>
				</div>
			
			</div>
			<div class="col">
				<div class="card" style="width: 25rem;">
				  <img class="card-img-top p-3" src="images/1000.jpg" alt="Card image cap">
				  <div class="card-body">
					<h5 class="card-title">I give you <b>$1000</b> happily</h5>
					<p class="card-text"></p>
					<div id="paypal-button-container_1000"></div>
				  </div>
				</div>
			
			</div>

		</div>
		<br>
		<br>
		<br>
		<br>
		<br>
		<br>
		<br>
		<br>
		<br>
		<br>
     <!-- SCRIPTS -->
     <script src="js/jquery.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/vegas.min.js"></script>
     <script src="js/countdown.js"></script>
     <script src="js/init.js"></script>
     <script src="js/custom.js"></script>
	 
	 
		
		
<script src="https://www.paypal.com/sdk/js?client-id=sb&currency=USD" data-sdk-integration-source="button-factory"></script>
<script>
  paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'gold',
          layout: 'vertical',
          label: 'paypal',
          
      },
      createOrder: function(data, actions) {
          return actions.order.create({
              purchase_units: [{
                  amount: {
                      value: '1'
                  }
              }]
          });
      },
      onApprove: function(data, actions) {
          return actions.order.capture().then(function(details) {
              alert('Transaction completed by ' + details.payer.name.given_name + '!');
          });
      }
  }).render('#paypal-button-container_1');
  
    paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'gold',
          layout: 'vertical',
          label: 'paypal',
          
      },
      createOrder: function(data, actions) {
          return actions.order.create({
              purchase_units: [{
                  amount: {
                      value: '10'
                  }
              }]
          });
      },
      onApprove: function(data, actions) {
          return actions.order.capture().then(function(details) {
              alert('Transaction completed by ' + details.payer.name.given_name + '!');
          });
      }
  }).render('#paypal-button-container_10');
  
    paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'gold',
          layout: 'vertical',
          label: 'paypal',
          
      },
      createOrder: function(data, actions) {
          return actions.order.create({
              purchase_units: [{
                  amount: {
                      value: '100'
                  }
              }]
          });
      },
      onApprove: function(data, actions) {
          return actions.order.capture().then(function(details) {
              alert('Transaction completed by ' + details.payer.name.given_name + '!');
          });
      }
  }).render('#paypal-button-container_100');
  
    paypal.Buttons({
      style: {
          shape: 'rect',
          color: 'gold',
          layout: 'vertical',
          label: 'paypal',
          
      },
      createOrder: function(data, actions) {
          return actions.order.create({
              purchase_units: [{
                  amount: {
                      value: '1000'
                  }
              }]
          });
      },
      onApprove: function(data, actions) {
          return actions.order.capture().then(function(details) {
              alert('Transaction completed by ' + details.payer.name.given_name + '!');
          });
      }
  }).render('#paypal-button-container_1000');
</script>


</body>
</html>