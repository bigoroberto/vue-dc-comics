<template>
<footer>
  <div class="container footer-top"> 
    <div class="list">
  
      <div> 
        <h5>DC COMICS</h5>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">news</a></li>
        </ul>
        <h5>SHOP</h5>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div> 
        <h5>DC</h5>
        <ul> 
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy Policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent workshops</a></li>
          <li><a href="#">CPSC certificates</a></li>
          <li><a href="#">ratings</a></li>
          <li><a href="#">shop help</a></li>
          <li><a href="#">contact us</a></li>
        </ul>
      </div>
      <div>
        <h5>SITES</h5>
        <ul>
          <li><a href="/">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC power visa</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-logo">

    </div>
  </div>
  <div class="footer-bottom">
    <div class="container">
    <div class="footer-button">
      <button>
        <a href="#">SIGN UP NOW!</a>
      </button>
    </div>
    <div  class="socials">
      <span><h5>FOLLOW US</h5></span>
      <ul>
        <li>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-twitter.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-youtube.png" alt="">
           </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-pinterest.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-periscope.png" alt="">
          </a>
        </li>
      </ul>
    </div>
  </div>

  </div>
</footer>

</template>

<script>
export default {
  name: 'FooterComp'
}
</script>

<style lang="scss" scoped>
footer{
  height: 500px;
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
}

@import '../assets/style/vars.scss';
.footer-top{
  height: 450px;
}

.list{
  display: flex;
  width: 50%;
  padding: 3rem 1rem;
    a,
  div{
    flex-basis: calc(100% / 3);
    text-transform: capitalize;
  }
  h5{
    text-transform: uppercase;
    font-size: 1.3rem;
    margin-bottom: 0.75rem;
    padding-top: 1rem;
    color: white;
  }
    a{
    display: inline-block;
    text-decoration: none;
    font-size: 0.85rem;
    margin-bottom: 0.2rem;
    color: rgb(135, 135, 135);
  }
}
.footert-logo{
  width: 50%;
  display: flex;
  background-image: url(../assets/img/dc-logo-bg.png);
  background-size: cover;
  background-repeat: no-repeat;
}

.footer-bottom{
  padding: 50px 0;
  height: 70px;
  display: flex;
  align-items: center;
  background-color: rgb(48, 48, 48);
}

.footer-button{
  width: 50%;

  button{
    background-color: rgb(48, 48, 48);
    border: 3px solid $blue-dc;
    padding: 15px;

          a{
        color: white;
        text-transform: uppercase;
        font-weight: bold;
        }
    }
}

.socials{
  width: 50%;
  text-align: right;
  display: flex;
  align-items: center;
  justify-content: flex-end;

  ul{
    list-style: none;

    li{
      padding: 5px;
      display: inline;
    }
  }
}

.socials h5{
  padding-right: 15px;
  font-size: 1rem;
  text-transform: uppercase;
  color: $blue-dc;
}
</style>