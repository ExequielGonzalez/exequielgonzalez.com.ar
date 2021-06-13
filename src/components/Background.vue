<template>
  <div class="background">
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
   <span></span>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@keyframes move {
    100% {
        transform: translate3d(0, 0, 1px) rotate(360deg);
    }
}

.background {
    position: fixed;
    width: 100vw;
    height: 100vh;
    top: 0;
    left: 0;
    background: #1e2235;
    overflow: hidden;
}

.background span {
    width: 20vmin;
    height: 20vmin;
    border-radius: 20vmin;
    backface-visibility: hidden;
    position: absolute;
    animation: move;
    animation-duration: 45;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
}


.background span:nth-child(0) {
    color: $background;
    top: 23%;
    left: 8%;
    animation-duration: 40s;
    animation-delay: -42s;
    transform-origin: 3vw 25vh;
    box-shadow: 40vmin 0 5.743508923706637vmin currentColor;
}
.background span:nth-child(1) {
    color: $footer;
    top: 42%;
    left: 86%;
    animation-duration: 38s;
    animation-delay: -2s;
    transform-origin: 17vw 6vh;
    box-shadow: 40vmin 0 5.839596328089388vmin currentColor;
}
.background span:nth-child(2) {
    color: $background;
    top: 12%;
    left: 23%;
    animation-duration: 30s;
    animation-delay: -30s;
    transform-origin: 4vw 19vh;
    box-shadow: -40vmin 0 5.146595659235278vmin currentColor;
}
.background span:nth-child(3) {
    color: $background;
    top: 2%;
    left: 27%;
    animation-duration: 12s;
    animation-delay: -10s;
    transform-origin: 19vw -19vh;
    box-shadow: 40vmin 0 5.182691025965379vmin currentColor;
}
.background span:nth-child(4) {
    color: $background;
    top: 60%;
    left: 3%;
    animation-duration: 42s;
    animation-delay: -25s;
    transform-origin: 12vw -4vh;
    box-shadow: 40vmin 0 5.571653604274749vmin currentColor;
}
.background span:nth-child(5) {
    color: $accent-light;
    top: 90%;
    left: 83%;
    animation-duration: 6s;
    animation-delay: -9s;
    transform-origin: 17vw 14vh;
    box-shadow: 40vmin 0 5.905537852515546vmin currentColor;
}
.background span:nth-child(6) {
    color: $footer;
    top: 12%;
    left: 40%;
    animation-duration: 55s;
    animation-delay: -36s;
    transform-origin: 7vw 20vh;
    box-shadow: -40vmin 0 5.393495400131632vmin currentColor;
}
.background span:nth-child(7) {
    color: $footer;
    top: 72%;
    left: 24%;
    animation-duration: 22s;
    animation-delay: -44s;
    transform-origin: 2vw 17vh;
    box-shadow: 40vmin 0 5.751963103482968vmin currentColor;
}
.background span:nth-child(8) {
    color: $background;
    top: 94%;
    left: 64%;
    animation-duration: 27s;
    animation-delay: -13s;
    transform-origin: 14vw -10vh;
    box-shadow: 40vmin 0 5.539634589390115vmin currentColor;
}
.background span:nth-child(9) {
    color: $footer;
    top: 16%;
    left: 12%;
    animation-duration: 50s;
    animation-delay: -14s;
    transform-origin: -7vw -4vh;
    box-shadow: -40vmin 0 5.161636554047428vmin currentColor;
}
.background span:nth-child(10) {
    color: $background;
    top: 76%;
    left: 54%;
    animation-duration: 15s;
    animation-delay: -24s;
    transform-origin: -10vw 24vh;
    box-shadow: 40vmin 0 5.350718518003111vmin currentColor;
}
.background span:nth-child(11) {
    color: $accent-light;
    top: 46%;
    left: 48%;
    animation-duration: 47s;
    animation-delay: -34s;
    transform-origin: 6vw 13vh;
    box-shadow: -40vmin 0 5.303116119857681vmin currentColor;
}
.background span:nth-child(12) {
    color: $footer;
    top: 71%;
    left: 54%;
    animation-duration: 34s;
    animation-delay: -4s;
    transform-origin: 5vw -12vh;
    box-shadow: -40vmin 0 5.855377293396184vmin currentColor;
}
.background span:nth-child(13) {
    color: $background;
    top: 57%;
    left: 73%;
    animation-duration: 29s;
    animation-delay: -11s;
    transform-origin: 21vw 17vh;
    box-shadow: -40vmin 0 5.638789729314399vmin currentColor;
}
.background span:nth-child(14) {
    color: $background;
    top: 93%;
    left: 57%;
    animation-duration: 19s;
    animation-delay: -44s;
    transform-origin: -1vw 23vh;
    box-shadow: -40vmin 0 5.43806133565238vmin currentColor;
}
.background span:nth-child(15) {
    color: $accent-light;
    top: 46%;
    left: 45%;
    animation-duration: 14s;
    animation-delay: -24s;
    transform-origin: 12vw -10vh;
    box-shadow: -40vmin 0 5.624828367518427vmin currentColor;
}

.background span:nth-child(16) {
    color: $footer;
    top: 92%;
    left: 99%;
    animation-duration: 33s;
    animation-delay: -41s;
    transform-origin: -19vw 14vh;
    box-shadow: -40vmin 0 5.557818891741954vmin currentColor;
}
.background span:nth-child(17) {
    color: $accent-light;
    top: 4%;
    left: 49%;
    animation-duration: 17s;
    animation-delay: -43s;
    transform-origin: -1vw 15vh;
    box-shadow: -40vmin 0 5.143208012715466vmin currentColor;
}
.background span:nth-child(18) {
    color: $background;
    top: 90%;
    left: 10%;
    animation-duration: 17s;
    animation-delay: -20s;
    transform-origin: -5vw -19vh;
    box-shadow: -40vmin 0 5.966062413307612vmin currentColor;
}
.background span:nth-child(19) {
    color: $footer;
    top: 66%;
    left: 18%;
    animation-duration: 35s;
    animation-delay: -3s;
    transform-origin: 20vw 16vh;
    box-shadow: -40vmin 0 5.305828678128981vmin currentColor;
}
</style>