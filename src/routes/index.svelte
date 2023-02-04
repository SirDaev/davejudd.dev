<svelte:head>
	<title>Dave Judd | Front End Web Developer from Minneapolis, MN, USA</title>
</svelte:head>

<script>
  import Container910 from '$lib/container-910.svelte';
  import Container_1300 from '$lib/container-1300.svelte';
  import Button from '$lib/button.svelte';
  import Testimonial from '$lib/testimonial.svelte';
  import dave from '$lib/assets/dave-sitting-with-laptop.jpg'
</script>

<section id="hero">
  <Container_1300>
    <div class="content">
      <h1 class="hero-title text-blue">Hi, my<br />name is <span class="text-semibold">Dave</span>.</h1>
      <h2 class="hero-subtitle">
        I'm a <span class="text-bold">front-end web developer</span><br />in Minneapolis, MN, USA.
        <img class="hero-dave" src={dave} alt="dave sitting at a table with laptop" />
      </h2>
    </div>
  </Container_1300>
</section>

<section id="jamstack">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title jamstack-title"><div class="jamstack-blob text-blue">JAM</div> <span class="stack-text">is my stack</span></h2>
      <p class="p-large"> 
        I have a passion for building fast fast, scalable, modern websites and web applications. I love playing with new technologies and finding the right tool for the job, and my favorite are the Jamstack tools!
        <!-- <br />
        <a href="/">Learn more</a> -->
      </p>
      <div class="icons">
        <img src="images/icons/js-icon.svg" alt="javascript icon" />
        <img src="images/icons/svelte-icon.svg" alt="svelte icon" />
        <img src="images/icons/react-icon.svg" alt="react icon" />
        <img src="images/icons/mongodb-icon.svg" alt="mongodb icon" />
        <img src="images/icons/gatsby-icon.svg" alt="gatsby icon" />
        <img src="images/icons/nextjs-icon.svg" alt="nextjs icon" />
        <img src="images/icons/netlify-icon.svg" alt="netlify icon" />
      </div>
    </div>
  </Container910>
</section>

<section id="fullstack">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title">I'll dive in to <span class="underline-pink">anything</span></h2>
      <p class="p-large"> 
        Whether it's a new animation feature with Three.js, or a database-driven web dashboard, I love working with all web dev-related technologies.
      </p>
      <div class="dino-animation">
        <img src="images/icons/trex-dinosaur.gif" alt="animated t-rex" />
      </div>
  </Container910>
</section>

<section id="testimonials">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title"><span class="underline-pink">Satisfied</span> clients</h2>
      <Testimonial />
    </div>
  </Container910>
</section>

<section id="make">
  <Container910 class="text-center">
    <div class="content">
      <h2 class="big-title">Let's make<br />something <span class="underline-pink">great</span>!</h2>
      <p class="p-large">Have an idea for a website or web project?<br />I'd love to hear it!</p>
      <div class="button-wrapper">
        <Button>
          <span class="material-icons-outlined">mail</span> Contact me
        </Button>
      </div>
    </div>
  </Container910>
</section>

<style>
  .content {
    padding: 80px 0;
  }

  @media (min-width: 992px) {
    .content {
      padding: 150px 0;
    }
  }

  .hero-title {
    font-size: 9rem;
    line-height: 1;
    font-weight: 400;
    margin-bottom: 25px;
    padding-left: 30px;
  }

  .hero-subtitle {
    position: relative;
    font-size: 4rem;
    line-height: 1.2;
    font-weight: 400;
    padding: 16px 0 20px 22px;
    background-color: #E4E4E4;
    border-left: 10px solid #F7ACD4;
  }

  .hero-dave {
    width: 446px;
    height: auto;
    position: absolute;
    right: 66px;
    bottom: -96px;
    border-radius: 10% 30%;
  }

  @media (min-width: 992px) {
    .hero-title {
      padding-left: 60px;
    }

    .hero-subtitle {
      padding: 16px 0 20px 50px;
    }
  }

  .big-title {
    font-size: 6rem;
    line-height: 1;
    font-weight: 400;
    margin-bottom: 60px;
  }

  .jamstack-title {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    margin-bottom: 30px;
  }

  .jamstack-blob {
    display: flex;
    align-items: center;
    height: 210px;
    background-image: url('/images/shapes/jamstack-blob.svg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: 92%;
    font-size: 13rem;
    line-height: 1;
    font-weight: 700;
    padding-top: 10px;
    margin: 0;
  }

  @media (min-width: 576px) {
    .jamstack-blob {
      margin: 0 35px 25px 0;
    }

    .jamstack-title {
      margin-bottom: 20px;
      flex-direction: row;
    }
  }

  @media (min-width: 992px) {
    .jamstack-blob {
      height: 256px;
    }
  }

  .icons {
    margin-top: 40px;
    font-size: 2rem;
    width: 100%;
    max-width: 320px;
    margin: 30px auto 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }

  .icons img {
    height: 50px;
    width: auto;
    margin: 0 10px 20px;
  }

  @media (min-width: 576px) {
    .icons {
      margin: 50px auto 0;
    }
  }

  @media (min-width: 768px) {
    .icons {
      max-width: 500px;
      justify-content: space-between;
    }

    .icons img {
      margin: 0;
    }
  }

  @media (min-width: 900px) {
    .icons {
      max-width: 750px;
    }

    .icons img {
      height: 76px;
    }
  }

  .button-wrapper {
    margin-top: 40px;
  }

.dino-animation {
  margin-top: 40px;
  font-size: 2rem;
  width: 100%;
  max-width: 320px;
  margin: 30px auto 0;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.dino-animation img {
  display: block;
  width: 200px;
  border-radius: 12px;
  border: 4px solid #474747;
}
</style>