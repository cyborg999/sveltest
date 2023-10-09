
<link rel="stylesheet" href="/global.css">

<style>
   
p.sec2_box {
  background: #f8f8f8;
  border: 1px solid #ccc;
  border-radius: 3px;
  box-shadow: none;
  -webkit-box-shadow: none;
  box-sizing: border-box;
  color: #666;
  font-size: 15px;
  line-height: 20px;
  margin: 100px 0 0px;
  padding: 10px 20px 5px 10px;
  position: relative;
  z-index: 99;
  letter-spacing: 0.5px;
  position: relative;
}

   
figure.sec1_fig1 {
  background: url(/images/logo.png) no-repeat 0 0;
  background-size: contain;
  height: 80px;
  margin: 5px 0 0;
  width: 154px;
}
.sec1 .sec_right {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.sec1 {
  background: #fff;
  box-shadow: 0 0 8px #ddd;
  height: 90px;
  left: 0;
  top: 0;
  width: 100%;
  z-index: 500;
}
.sec1 h5 {
  color: #000;
  font-size: 1.5rem;
  font-style: italic;
  font-weight: 700;
  padding: 0;
  margin-top: 17px;
  line-height: 1.3;
}
.sec1 p {
  color: #000;
  font-weight: 600;
  letter-spacing: 0.5px;
  font-size: 14px;
  padding: 0;
}




    .footer figure {
        background: url(/images/logo.png) no-repeat 0 0;
        background-size: contain;
        height: 40px;
        margin: 5px 0 0;
        width: 54px;
        margin: 0 auto;
        margin-top: 120px;
    }
    .footer .container {
        display: block;
    }
    .footer ul {
        text-align: center;
    }
    .footer li {
        padding: 5px;
        display: inline;
    }
    .footer p {
        color: black;
        font-size: 12px;
        text-align: center;
    }   
    .footer a {
        text-decoration: none;
        color: black;
        font-size: 12px;
    }

</style>
<script>
    import { goto } from "$app/navigation"

    let handleClick = (e) => {
        e.preventDefault();

        goto("/checkout")
    }
</script>
<main class="main">
    <section class="sec1">
        <article class="container">
            <div class="sec_left">
            <a href="/"><figure class="sec1_fig1"></figure></a>
            </div>
            <div class="sec_right">
            <div>
                <h5>Claim My Discount</h5>
                <p><em>Voted #1</em> Fungal Product in USA</p>
            </div>
            <a href="/" on:click={ handleClick } class="btn">Order Now</a>
            </div>
        </article>
    </section>
    <slot/>
    <footer class="footer">
        <article class="container">
            <figure></figure>
            <ul>
                <li><a href="/terms">Terms & Conditions</a></li>
                <li><a href="/privacy">Privacy & Policy</a></li>
                <li><a href="/contact">Contact Us</a></li>
            </ul>
            <p>Auvela 2023. All rights reserved.</p>
        </article>
    </footer>
</main>


