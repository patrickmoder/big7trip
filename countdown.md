# Countdown to Event

<p id="timer"></p>

<script>
  // Set the date of your event (example: March 25, 2025)
  var eventDate = new Date("March 25, 2025 00:00:00").getTime();

  var timer = setInterval(function() {
    // Get current time
    var now = new Date().getTime();
    
    // Calculate the time remaining
    var distance = eventDate - now;
    
    // Calculate days, hours, minutes, and seconds
    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);

    // Display the result
    document.getElementById("timer").innerHTML = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";

    // If the event has passed, display a message
    if (distance < 0) {
      clearInterval(timer);
      document.getElementById("timer").innerHTML = "Event has started!";
    }
  }, 1000);
</script>

