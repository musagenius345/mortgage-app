<script>import "./app.css";
import RadioGroup from "./lib/components/RadioGroup.svelte";
</script>

<svelte:head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./assets/images/favicon-32x32.png" />

  <title>Frontend Mentor | Mortgage repayment calculator</title>
</svelte:head>
<main class="content-grid">
  <section class="calculator">
    <h1>Mortgage Calculator</h1>
    <p>Clear All</p>
    <form action="/">
      <h3>Mortgage Amount</h3>
      <h3>Mortgage Term</h3>
      <h3>Interest Rate</h3>
      <RadioGroup />
     

      <button class="calculate-repayments">Calculate Repayments</button>
    </form>

    
  </section>
  <!-- Empty results start -->
  <section class="results full-width">
    <div>
      <h2>Results shown here</h2>
      <p class="complete-form">
        Complete the form and click “calculate repayments” to see what your
        monthly repayments would be.
      </p>
      <!-- Empty results end -->
      <!-- Completed results start -->
      Your results Your results are shown below based on the information you
      provided. To adjust the results, edit the form and click “calculate
      repayments” again. Your monthly repayments Total you'll repay over the term
      <!-- Completed results end -->
    </div>
  </section>
</main>


<style>
</style>
