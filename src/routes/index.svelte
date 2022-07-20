<svelte:head>
	<title>DaveJudd.dev</title>
</svelte:head>

<script>
  import Container910 from '$lib/container-910.svelte';
  import Button from '$lib/button.svelte';
  import QuoteBox from '$lib/quotebox.svelte';
  import dave from '$lib/assets/dave-sitting-with-laptop.jpg'
</script>

<section id="hero">
  <div class="hero">
    <div class="content">
      <h1 class="hero-title text-blue">Hi, my<br />name is <span class="text-semibold">Dave</span>.</h1>
      <h2 class="hero-subtitle">
        I'm a <span class="text-bold">front-end web developer</span><br />in Minneapolis, MN, USA
        <img class="hero-dave" src={dave} alt="dave sitting at a table with laptop" />
      </h2>
    </div>
  </div>
</section>

<section id="jamstack">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title jamstack-title"><div class="jamstack-blob text-blue">JAM</div> is my stack</h2>
      <p class="p-large"> 
        I have a passion for building fast fast, scalable, modern websites.<br />
        <a href="/">Learn more</a>
      </p>
      <div class="icons">
        ICONS
      </div>
    </div>
  </Container910>
</section>

<section id="make">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title">Let's make<br />something <span class="underline-pink">great</span>!</h2>
      <p class="p-large">Have an idea for a website or web project?  Ut enim ad minim.</p>
      <div class="button-wrapper">
        <Button>
          <span class="material-icons-outlined">mail</span> Contact me
        </Button>
      </div>
    </div>
  </Container910>
</section>

<section id="testimonial">
  <Container910>
    <QuoteBox>
      quote
    </QuoteBox>
  </Container910>
</section>

<style>
  .content {
    padding: 150px 0;
  }

  .hero {
    width: 100%;
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 15px;
  }

  .hero-title {
    font-size: 9rem;
    line-height: 1;
    font-weight: 400;
    margin-bottom: 25px;
    padding-left: 60px;
  }

  .hero-subtitle {
    position: relative;
    font-size: 4rem;
    line-height: 1.2;
    font-weight: 400;
    padding: 16px 0 20px 50px;
    background-color: #E4E4E4;
    border-left: 10px solid #F7ACD4;
  }

.hero-dave {
  width: 446px;
  height: auto;
  position: absolute;
  right: 66px;
  bottom: -96px;
}

  .big-title {
    font-size: 9rem;
    line-height: 1;
    font-weight: 400;
    margin-bottom: 60px;
  }

  .jamstack-title {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
  }

  .jamstack-blob {
    display: flex;
    align-items: center;
    height: 256px;
    background-image: url('images/shapes/jamstack-blob.svg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: 92%;
    font-size: 13rem;
    line-height: 1;
    font-weight: 700;
    padding-top: 10px;
    margin: 0 35px 25px 0;
  }

  .icons {
    margin-top: 40px;
    font-size: 2rem;
  }

  .button-wrapper {
    margin-top: 40px;
  }
</style>