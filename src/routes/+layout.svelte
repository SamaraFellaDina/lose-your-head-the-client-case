<header>
  <img src='/assets/images/header.png' alt='hier een dummy header <3'>
</header>

<main>
  <slot />
</main>

<style>
    header {
      height: 10%;
      position: fixed;
  }

  @media only screen and (max-width: 1600px) {
    header img{
      display: none;
    }
}
</style>