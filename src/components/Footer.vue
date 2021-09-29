<template>
  <div class="footer-container-top">
    <div class="container">
      <div class="footer-top">
        <div class="lists-container">
          <div class="footer-list">
            <h4>DC COMICS</h4>
            <ul> 
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h4>SHOP</h4>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="footer-list">
            <h4>DC</h4>
            <ul> 
              <li><a href="#">Terms of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="footer-list">
            <h4>SITES</h4>
            <ul> 
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="footer-top-right-logo">
          <div class="logo">
            <img src="@/assets/images/dc-logo-bg.png" alt="DC Logo Footer">
          </div>
        </div>
      </div>
    </div>
    
    <div class="footer-container-bottom">
      <div class="container">
        <div class="sign-up">
          <a href=""><button>SIGN-UP NOW!</button></a> 
        </div>
        <div class="social">
          <span>FOLLOW US</span>
          <div class="facebook">
            <a href="#"><img src="@/assets/images/footer-youtube.png" alt="Facebook"></a> 
          </div>
          <div class="twitter">
            <a href="#"><img src="@/assets/images/footer-twitter.png" alt="Twitter"></a> 
          </div>
          <div class="youtube">
            <a href="#"><img src="@/assets/images/footer-youtube.png" alt="YouTube"></a> 
          </div>
          <div class="pinterest">
            <a href="#"><img src="@/assets/images/footer-pinterest.png" alt="Pinterest"></a> 
          </div>
          <div class="periscope">
            <a href="#"><img src="@/assets/images/footer-periscope.png" alt="Periscope"></a> 
          </div>
        </div>
      </div> 
    </div>
  </div>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss">
@import '@/assets/style/Variables';
  .footer-container-top {
    background-image: url('../assets/images/footer-bg.jpg');
    background-size: cover;
    .footer-top {
      display: flex;
      justify-content: space-between;
      .lists-container {
        display: flex;
        .footer-list{
          margin-right: 30px;
          h4 {
            color: #FEFFFF;
            margin-bottom: 10px;
          }
          ul {
            list-style: none;
            margin-bottom: 20px;
            a {
              color: #767B79;  
              text-decoration: none;
            }
          }
        } 
      } 
      .logo {
        max-width: 300px;
        img{
          width: 100%;
        }
      }
    }
  }
  .footer-container-bottom {
    background-color: #303030;
    padding: 15px;
    .container {
      display: flex;
      justify-content: space-between;
      .sign-up {
        max-width: 130px;
        button {
          display: inline-block;
          padding: 10px;
          color: #FEFFFF;
          border: 1px solid $mainColor;
          background-color: #303030;

        }
      }
      .social {
        display: flex;
        span {
          color: $mainColor;
          align-self: center;
          margin-right: 20px;
          font-weight: bold;
        }
        div {
          margin: 0 5px;
        }
      }
    }
  }
</style>