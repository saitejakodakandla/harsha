<!DOCTYPE HTML>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Happy Birthday ra mama </title>

<link rel="icon" href="images/favicon.png">
<style>
html {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  height: 100%;
  margin: 0;
}

body {

  align-items: center;
  background-color: #D3D3D3;
  display: flex;
  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; 


}

 

h1 {
  font-weight: normal;
  letter-spacing: .125rem;
  text-transform: uppercase;
}


li {
  display: inline-block;
  font-size: 1.5em;
  list-style-type: none;
  padding: 1em;
  text-transform: uppercase;
}

li span {
  display: block;
  font-size: 4.5rem;
}

.message {
  font-size: 4rem;
}

#content {
  display: none;
  padding: 1rem;
}

.emoji {
  padding: 0 .25rem;
}

@media all and (max-width: 768px) {
  h1 {
    font-size: 1.5rem;
  }
  
  li {
    font-size: 1.125rem;
    padding: .75rem;
  }
  
  li span {
    font-size: 3.375rem;
  }
}



.harsha{
display: block;
width: 215px; 
height: 215px; 
border-radius: 50%;
margin: 0 auto;
object-fit: cover;
border:4px solid #7fff00;
}




  
</style>
<script type="text/javascript">(function () {
  const second = 1000,
        minute = second * 60,
        hour = minute * 60,
        day = hour * 24;

  let birthday = "dec 6, 2020 00:00:00",
      countDown = new Date(birthday).getTime(),
      x = setInterval(function() {    

        let now = new Date().getTime(),
            distance = countDown - now;

        document.getElementById("days").innerText = Math.floor(distance / (day)),
          document.getElementById("hours").innerText = Math.floor((distance % (day)) / (hour)),
          document.getElementById("minutes").innerText = Math.floor((distance % (hour)) / (minute)),
          document.getElementById("seconds").innerText = Math.floor((distance % (minute)) / second);

        //do something later when date is reached
        if (distance < 0) {
          let headline = document.getElementById("headline"),
              countdown = document.getElementById("countdown"),
              content = document.getElementById("content");

          headline.innerText = "It's my birthday!";
          countdown.style.display = "none";
          content.style.display = "block";

          clearInterval(x);
        }
        //seconds
      }, 0)
  }());</script>

</head>
<body>

<div class="innova">
<a href="https://www.instagram.com/harsha_mudhiraj_12/"><img class="harsha" src="harsha.png"></a><br>
 
  <h1 id="headline">Happy Birthday Mama <br>( 𝐼𝓃 𝒜𝒹𝓋𝒶𝓃𝒸𝑒 ) </h1>
  <div id="countdown">
    <ul>
      <li><span id="days"></span>days</li>
      <li><span id="hours"></span>Hours</li>
      <li><span id="minutes"></span>Minutes</li>
      <li><span id="seconds"></span>Seconds</li>
    </ul>
  </div>
  <div class="message">
    <div id="content">
      <span class="emoji">🥳</span>
      <span class="emoji">🎉</span>
      <span class="emoji">🎂🍾</span>
    </div>
  </div>
</div>

</body>
</html>
