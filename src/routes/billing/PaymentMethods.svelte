<script>
  import OrderHistory from './OrderHistory.svelte';


  import NavMobile from './NavMobile.svelte';
</script>

      <section class="methods">
        <div class="subtitle">
          <h2>Payment Method</h2>
          <p class="description__text">Manage billing information and view receipts</p>
        </div>
        <div class="methods__row">
          <div class="methods__icon button">
            <img class="methods__img" src="visa.png" alt="visa">
          </div>
          <p class="methods__desc">Visa ending in 2255</p>
          <button class="methods__remove">Remove</button>
        </div>
      </section>

<style>
  .methods__row {
    display: flex;
    align-items: center;
  }

  .methods__desc {
    margin-right: auto;
  }

  .methods__remove {
    padding: 0.25rem 0.75rem;
    border: solid 1px #c4c4d4;
    border-radius: 0.5rem;
    font-family: inherit;
    font-size: inherit;
  }
  
  .methods__icon {
    height: 4rem;
  }

  .methods__img {
    height: 100%;
  }

  .description__text {
    color: #62618F;
  }
</style>

