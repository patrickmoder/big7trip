## Big 7 goes... 2025

<!-- <img src="https://github.com/patrickmoder/big7trip/blob/main/big7-athens-2024.JPG" alt="athens" width="50%"/> -->

![Big7 Athens](./big7-athens-2024.JPG)

Da sind wir wieder! Und (fast) vereint in einer der schönsten Destinationen auf unserem Planeten - rau und ehrlich, genauso wie die Big7!

stay tuned...

# Nur noch so lange müssen wir uns gedulden...

<style>
  #timer {
    font-family: 'Arial', sans-serif;
    font-size: 2em;
    color: #ff5733;
    font-weight: bold;
    text-align: center;
  }
</style>

<p id="timer"></p>

<script>
  // Set the date of your event (example: March 25, 2025)
  var eventDate = new Date("April 25, 2025 10:00:00").getTime();

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


Eine kleine Historie gefällig? [Hier](historie.md) geht es zu eindrucksvollen, lehrreichen, denkwürdigen und abstoßenden Impressionen der letzten gemeinsamen Jahre.

Na, neugierig? Ihr wollt wirklich wissen, wo es hingeht? Vielleicht helfen euch die [Fakten](fakten.md) über unser zukünftiges Ziel ja weiter...

Hier ein paar Anhaltspunkte, was in den Koffer sollte: [Packliste](packliste.md)
