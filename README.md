# Flip-card-with-hovering-text
.....html......
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="wrapper">
  <h1>Parallax Flipping Cards</h1>
  <div class="cols">
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://tse4.mm.bing.net/th?id=OIP.c0rKQnY3U8ckLQAlxJ7JuAAAAA&pid=Api&P=0&w=226&h=151)">
            <div class="inner">
              <p>Break a leg</p>
              <span>Good luck</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>!@#$%^&*()_+</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image:url(https://tse4.mm.bing.net/th?id=OIP.T4k6U5d289X1uPe0-AerbgAAAA&pid=Api&P=0&w=228&h=172)">
            <div class="inner">
              <p>Hang in there</p>
              <span>Don't give up</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>1209348756</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://tse3.mm.bing.net/th?id=OIP.ZaU4FN4vXRKA0c2JwA-JoAAAAA&pid=Api&P=0&w=222&h=167)">
            <div class="inner">
              <p>Hit the sack</p>
              <span>Go to sleep</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>~~~~~~~~~~~~</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://tse1.mm.bing.net/th?id=OIP.FgHvL43lF1wFk2k0almQJwAAAA&pid=Api&P=0&w=250&h=167)">
            <div class="inner">
              <p>On the ball</p>
              <span>Doing a good job</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>**********</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image:url(https://tse4.mm.bing.net/th?id=OIP.MJUKoITDIx1CZzxa21DKyQAAAA&pid=Api&P=0&w=300&h=300)">
            <div class="inner">
              <p>On thin ice</p>
              <span>On probation</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>"""""""""""""""""""</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://tse3.mm.bing.net/th?id=OIP.bkR-XalmCZqKCdAdyQoP5AAAAA&pid=Api&P=0&w=230&h=172)">
            <div class="inner">
              <p>Burn bridges</p>
              <span>Destroy relationships</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>/////////</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://tse3.mm.bing.net/th?id=OIP.UTAXskdirfONIKRL6h9bbQAAAA&pid=Api&P=0&w=309&h=175)">
            <div class="inner">
              <p>On cloud nine</p>
              <span>Very happy</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>++++++++++</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col" ontouchstart="this.classList.toggle('hover');">
        <div class="container">
          <div class="front" style="background-image: url(https://i.pinimg.com/236x/53/ce/c4/53cec40ded6142239ed13b388034de9d.jpg)">
            <div class="inner">
              <p>Snowed under</p>
              <span>Busy</span>
            </div>
          </div>
          <div class="back">
            <div class="inner">
              <p>==========</p>
            </div>
          </div>
        </div>
      </div>
    </div>
 </div>
  </body>
</html>
......css........
*{
  margin: 0;
  padding: 0;
  -webkit-box-sizing: border-box;
          box-sizing: border-box;
}

h1{
  font-size: 2.5rem;
  font-family: 'Montserrat';
  font-weight: normal;
  color: rgb(167, 32, 137);
  text-align: center;
  margin: 2rem 0;
}

.wrapper{
  width: 90%;
  margin: 0 auto;
  max-width: 80rem;
}

.cols{
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
}

.col{
  width: calc(25% - 2rem);
  margin: 1rem;
  cursor: pointer;
}

.container{
  -webkit-transform-style: preserve-3d;
          transform-style: preserve-3d;
  -webkit-perspective: 1000px;
          perspective: 1000px;
}

.front,
.back{
  background-size: cover;
  box-shadow: 0 4px 8px 0 rgba(17, 76, 99, 0.25);
  border-radius: 10px;
  background-position: center;
  -webkit-transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
  transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
  -o-transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
  transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
  transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1), -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  text-align: center;
  min-height: 280px;
  height: auto;
  border-radius: 10px;
  color: rgb(148, 250, 139);
  font-size: 1.5rem;
}

.back{
  background: #e7fc2e;
  background: -webkit-linear-gradient(45deg,  #051e31 0%,#c507a5 100%);
  background: -o-linear-gradient(45deg,  #0d5083 0%,#0975a7 100%);
  background: linear-gradient(45deg,  #bdba18 0%,#119206 100%);
}

.front:after{
  position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
    width: 100%;
    height: 100%;
    content: '';
    display: block;
    opacity: .6;
    background-color: #000;
    -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
    border-radius: 10px;
}
.container:hover .front,
.container:hover .back{
    -webkit-transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    -o-transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1), -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
}

.back{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
}

.inner{
    -webkit-transform: translateY(-50%) translateZ(60px) scale(0.94);
            transform: translateY(-50%) translateZ(60px) scale(0.94);
    top: 50%;
    position: absolute;
    left: 0;
    width: 100%;
    padding: 2rem;
    -webkit-box-sizing: border-box;
            box-sizing: border-box;
    outline: 1px solid transparent;
    -webkit-perspective: inherit;
            perspective: inherit;
    z-index: 2;
}

.container .back{
    -webkit-transform: rotateY(180deg);
            transform: rotateY(180deg);
    -webkit-transform-style: preserve-3d;
            transform-style: preserve-3d;
}

.container .front{
    -webkit-transform: rotateY(0deg);
            transform: rotateY(0deg);
    -webkit-transform-style: preserve-3d;
            transform-style: preserve-3d;
}

.container:hover .back{
  -webkit-transform: rotateY(0deg);
          transform: rotateY(0deg);
  -webkit-transform-style: preserve-3d;
          transform-style: preserve-3d;
}

.container:hover .front{
  -webkit-transform: rotateY(-180deg);
          transform: rotateY(-180deg);
  -webkit-transform-style: preserve-3d;
          transform-style: preserve-3d;
}

.front .inner p{
  font-size: 2rem;
  margin-bottom: 2rem;
  position: relative;
}

.front .inner p:after{
  content: '';
  width: 4rem;
  height: 2px;
  position: absolute;
  background: #C6D4DF;
  display: block;
  left: 0;
  right: 0;
  margin: 0 auto;
  bottom: -.75rem;
}

.front .inner span{
  color: rgba(175, 233, 15, 0.7);
  font-family: 'Montserrat';
  font-weight: 300;
}

@media screen and (max-width: 64rem){
  .col{
    width: calc(33.333333% - 2rem);
  }
}

@media screen and (max-width: 48rem){
  .col{
    width: calc(50% - 2rem);
  }
}

@media screen and (max-width: 32rem){
  .col{
    width: 100%;
    margin: 0 0 2rem 0;
  }
}
