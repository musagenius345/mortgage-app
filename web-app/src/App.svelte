<script lang="ts">

</script>
<svelte:head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./assets/images/favicon-32x32.png">
  
  <title>Frontend Mentor | Mortgage repayment calculator</title>
</svelte:head>
<main class="content-grid">

  <section class="calculator">
    <h1>Mortgage Calculator</h1>
    <p>Clear All</p>
    <h3>Mortgage Amount</h3>
    <h3>Mortgage Term</h3>
    <h3>Interest Rate</h3>
    <h3>Mortgage Type</h3>
    <div class="option-one">
      <input type="radio" name="mortgage" id="repayment" value="repayement" checked>
      <label for="mortgage-type">
        Repayment
      </label>
    </div>
    <div class="option-two">
      <input type="radio" name="mortgage" id="interest-only" value="interest-only">
      <label for="interest-only">
        Interest Only
      </label>
    </div>
    
    <button class="calculate-repayments">Calculate Repayments</button>
  </section>
  <!-- Empty results start -->
<section class="results">
  Results shown here

  Complete the form and click “calculate repayments” to see what 
  your monthly repayments would be.

  <!-- Empty results end -->

  <!-- Completed results start -->

  Your results

  Your results are shown below based on the information you provided. 
  To adjust the results, edit the form and click “calculate repayments” again.

  Your monthly repayments

  Total you'll repay over the term

  <!-- Completed results end -->
</section>

</main>

<style>

</style>
