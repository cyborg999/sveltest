<style>

.sec10 .container {
  background: url(./images/s6-bg.jpg) no-repeat 100% 0;
  min-height: 66vh;
}
.sec10 .sec_left {
  padding: 74px 0 0;
}
.sec10 b {
  font-size: 18px;
  font-weight: 700;
  line-height: 24px;
  margin: 20px 0 0;
  display: block;
}
.sec10 .btn {
  background: #f1c61a;
  border: none;
  border-radius: 8px;
  color: #77620d;
  cursor: pointer;
  display: block;
  font-size: 32px;
  font-weight: 800;
  height: 80px;
  letter-spacing: -1px;
  line-height: 80px;
  margin: 0;
  padding: 0;
  position: relative;
  text-align: center;
  text-decoration: none;
  text-transform: uppercase;
  -webkit-transition: all .2s;
  -moz-transition: all .2s;
  -o-transition: all .2s;
  transition: all .2s;
  font-size: 26px;
  line-height: 30px;
  padding: 13px 0 0;
  width: 350px;
  position: relative;
  margin-top: 20px;
}
.sec10 .btn::after {
  position: absolute;
  content: "";
  right: 0;
  top: 0;
  font-size: 18px;
  font-weight: 400;
  line-height: 18px;
  padding: 4px 0 0;
  text-transform: none;
  width: 47px;
  height: 47px;
  background: url(./images/30-off.png) no-repeat 0 0;
}
.sec10 small {
  display: block;
  font-size: 18px;
  font-weight: 400;
  line-height: 18px;
  padding: 4px 0 0;
  text-transform: none;
}
.sec10_box {
  position: relative;
  width: 243px;
  height: 100%;
}
figure.sec10_fig1 {
  position: absolute;
  left: 18%;
  bottom: 3%;
  background: url(./images/product.png) no-repeat;
  background-size: contain;
  width: 107px;
  height: 214px;
}
figure.sec10_fig2 {
  position: absolute;
  right: 20%;
  bottom: 0;
  background: url(./images/product.png) no-repeat;
  background-size: contain;
  width: 117px;
  height: 233px;
}
.sec10 .sec_right {
    position: relative;
}
</style>

<script>
    import { goto } from "$app/navigation"

    let handleClick = (e) => {
        e.preventDefault();

        console.log("click")
        goto("/checkout")
    }
    </script>
   <section class="sec10">
    <article class="container">
      <div class="sec_left">
        <h2>Healthy Nails And Skin Without Surgery!</h2>
        <p>Cuticara is changing the way people protect their skin and nails. By applying Cuticara to your skin and nails daily, you can purportedly protect nail keratin, fight nail fungus, and boost your natural immunity using a blend of proven ingredients. Join thousands of others who are already enjoying beautiful and blemish-free skin today!</p>
        <b>Order your supply of Cuticara now!
          Start feeling great about your skin & nails again.</b>

        <a href="" class="btn" on:click={ handleClick }>Try Cuticura <small>30% Instant Online Discount Today!</small></a>
      </div>
      <div class="sec_right">
        <div class="sec10_box">
          <figure class="sec10_fig1"></figure>
          <figure class="sec10_fig2"></figure>
        </div>
      </div>
    </article>
  </section>