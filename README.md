# 1.Romantic-html
My first project. I made this with html + CSS + js. Language used Bangla.
<!DOCTYPE html>
<html>
<head>
  <title>Romantic-html</title>
</head>
<style>
    body {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: black;
}

.heart {
    height: 100px;
    width: 100px;
    background: #f20044;
    position: relative;
    transform: rotate(-45deg);
    box-shadow: -10px -10px 90px #f20044;
    animation: heart 1.2s infinite;
}

@keyframes heart {
    0% {
        transform: rotate(-45deg) scale(1.02);
    }
    80% {
        transform: rotate(-45deg) scale(0.8);
    }
    100% {
        transform: rotate(-45deg) scale(1.02);
    }
}

.heart::before,
.heart::after {
    content: '';
    position: absolute;
    height: 100px;
    width: 100px;
    background: #f20044;
    border-radius: 70px;
    box-shadow: -5px -5px 100px #f20044;
}

.heart::before {
    top: -50%;
    left: 0;
}

.heart::after {
    right: -50%;
    top: 0;
}
.heart-btn {
    position: absolute;
    top: 65%;
    left: 50%;
    transform: translate(-50%, -50%);
    padding: 10px 20px;
    background-color: lightblue;
    border: none;
    border-radius: 8px;
    color: #03045e;
    font-weight: bold;
    cursor: pointer;
    z-index: 2; /* ensure it stays on top */
    box-shadow:
        0 0 30px #0077b6;
}
 

</style>
<body>

  <div class="heart"></div>

  <button class="heart-btn" onclick= "window.location.href='msg.html'">
    Tup Daw
  </button>


</body>
</html>
