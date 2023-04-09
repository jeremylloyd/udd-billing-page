<script>

  import NavMobile from './NavMobile.svelte';
</script>

      <section>
        <div class="description">
          <h2>Order History</h2>
          <p class="description__text">Manage billing information and view receipts</p>
        </div>
        <table class="table">
          <tr class="table__headers">
            <th>Date</th>
            <th>Type</th>
            <th>Receipt</th>
          </tr>
          <tr class="table__row">
            <td class="table__data">2021-10-21</td>
            <td class="table__data">Pro Annual</td>
            <td class="table__download"><a class="table__receipt" href="receipt" download>Download</a></td>
          </tr>
          <tr class="table__row">
            <td class="table__data">2021-08-21</td>
            <td class="table__data">Pro Portfolio</td>
            <td class="table__download"><a class="table__receipt" href="receipt" download>Download</a></td>
          </tr>
          <tr class="table__row">
            <td class="table__data">2021-07-21</td>
            <td class="table__data">Sponsored Post</td>
            <td class="table__download"><a class="table__receipt" href="receipt" download>Download</a></td>
          </tr>
          <tr class="table__row">
            <td class="table__data">2021-06-21</td>
            <td class="table__data">Sponsored Post</td>
            <td class="table__download"><a class="table__receipt" href="receipt" download>Download</a></td>
          </tr>
        </table>
        <button class="table__more">Load more</button>
      </section>

<style>
  .description__text {
    color: #62618F;
  }
  
  .table {
    width: 100%;
    border-spacing: 0px;
  }

  .table__headers {
    color: #62618F;
    font-weight: 500;
    text-align: left;
  }

  .table__download {
    width: 6rem;
  }

  .table__receipt {
    text-decoration: none;
    color: #62618F;
    border-color: #c4c4d4;
    border: solid 1px;
    border-radius: 0.5rem;
    padding: 0.4rem 1rem;
  }

  .table__row:hover {
    background-color: #F8F8FF;
    box-shadow: 0rem 5px 10px 5px #d7d7f1;
  }

  .table__data {
    padding: .75rem 0 .75rem;
  }

  .table__more {
    color: #EE4D38;
    font-size: inherit;
    text-decoration: underline;
  }

  button {
    font-family: 'Poppins', sans-serif;
  }
</style>

