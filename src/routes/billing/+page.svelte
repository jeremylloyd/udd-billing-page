<script>
  import Plan from './Plan.svelte';

  import PaymentMethods from './PaymentMethods.svelte';

  import OrderHistory from './OrderHistory.svelte';


  import NavMobile from './NavMobile.svelte';
</script><svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;700&display=swap" rel="stylesheet">
</svelte:head>

<div class="page">
  <div class="container-mobile">
    <NavMobile></NavMobile>
  </div>
  <aside class="container-desktop">
    <div class="nav-desktop">
      <div class="nav-desktop__profile">
        <img class="nav-desktop__img" src="ildiko.png" alt="profile">
        <div class="nav-desktop__info">
          <p class="nav-desktop__name">Ildiko Gaspar</p>
          <p class="nav-desktop__contact">@igaspar</p>
        </div>
      </div>
      <div class="nav-desktop__links">
        <a href="/general">General</a>
        <a href="/password">Password</a>
        <a href="/invites">Invitations</a>
        <a href="/billing">Billing</a>
        <a href="/apps">Apps</a>
    </div>
  </aside>

  <main class="main">
    <h1 class="desktop">Billing</h1>
    <div class="content">
      <div class="content__main">
        <OrderHistory></OrderHistory>
        <PaymentMethods></PaymentMethods>
      </div>
      <div class="content__aside">
        <Plan></Plan>
      </div>
    </div>
  </main>
</div>

<style>
  .page {
    font-family: 'Poppins', sans-serif;
    display: flex;
    flex-direction: column;
  }

  .main {
    flex-grow: 1;
  }
  
  .container-mobile {
    display: none;
  }

  .content {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .content__main {
    flex-grow: 1;
  }

  .content__aside {
    align-self: flex-start;
  }

  .nav-desktop__profile {
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .nav-desktop__img {
    height: 4rem;
  }

  .nav-desktop__name {
    font-weight: 700;
  }

  .nav-desktop__links {
    display: flex;
    flex-direction: column;
  }

  .nav-desktop__contact {
    color: #62618F;
  }
  
  .container-desktop {
    display: none;
  }

  @media (max-width: 500px) {
    .container-mobile {
      display: unset;
    }

    .desktop {
      display: none;
    }
  }
  
  @media (min-width: 800px) {
    .content {
      flex-direction: row;
    }

    .container-desktop {
      display: block;
    }

    .page {
      flex-direction: row;
    }
  }
</style>