<!DOCTYPE html>
<html>
<head>
<title>Fade In Text Effect</title>
<style>
@import url("https://fonts.googleapis.com/css?family=Roboto&display=swap");

body{
  background: black;

}
.main-text {
  color: white;
  font-size: 4rem;
  font-family: Roboto, sans-serif;
  text-align: left;
  margin-left: 25%;
  margin-right: 10%;
  animation: fadein 4s;
  animation-timing-function: ease-in;
  -moz-animation: fadein 4s; /* Firefox */
  -webkit-animation: fadein 4s; /* Safari and Chrome */
  -o-animation: fadein 4s; /* Opera */
}

.jobs {
  color: white;
  font-size: 4rem;
  font-family: Roboto, sans-serif;
  text-align: left;
  animation: fadein 4s;
  animation-timing-function: ease-in;
  -moz-animation: fadein 4s; /* Firefox */
  -webkit-animation: fadein 4s; /* Safari and Chrome */
  -o-animation: fadein 4s; /* Opera */
}

@keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@-moz-keyframes fadein {
  /* Firefox */
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadein {
  /* Safari and Chrome */
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-o-keyframes fadein {
  /* Opera */
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
</head>
<body>
 <h1 class="main-text">
  </h1>
<script>
const text = document.querySelector(".main-text");

var n = 0;
let timer = setInterval(onTick, 2500);

function onTick() {
  if (n === 0) {
    text.innerHTML = " Hi there! I'm <span >Shashi</span>";

    n = 1;
    return;
  }
  if (n === 4) {
    text.innerHTML = ' Hi there! I\'m <span class="jobs" ">Shashi</span>';

    n = 1;
    return;
  } else if (n == 1) {
    text.innerHTML = ' Hi there! I\'m <span class="jobs">a Developer</span>';
    n = 2;
    return;
  } else if (n == 2) {
    text.innerHTML =
      ' Hi there! I\'m <span class="jobs">a Software Developer</span>';
    n = 3;
    return;
  } else if (n == 3) {
    text.innerHTML = ' Hi there! I\'m <span class="jobs">a Full-Stack-Developer</span>';
    n = 4;
    return;
  }
}

</script>
</body>
</html>
