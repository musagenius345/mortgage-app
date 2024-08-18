<div class="options">
  <h3>Mortgage Type</h3>
  <label class="repayment form-box form-control">
    <input
      type="radio"
      name="mortgage-type"
      id="repayment"
      value="repayement"
    />
    <p class="text">Repayment</p>
  </label>
  <label class="interest-only form-box form-control">
    <input
      type="radio"
      name="mortgage-type"
      id="interest-only"
      value="interest-only"
    />
    <p class="text">Interest Only</p>
  </label>
</div>

<style>
  label {
    padding-inline-start: 0.8em;
  }
  .form-control {
    font-size: var(--step-0);
    font-weight: bold;
    line-height: 1.1;
    padding-block: 0.25rem;
    margin-top: 1em;
    display: grid;
    grid-template-columns: 5px 1fr 1fr;
    gap: var(--space-s-m);
    transform: translateY(-0.025em);

    display: grid;
    /* place-content: center; */
    /* place-self: center; */

    & > :not(.form-control + .form-control) {
      margin-block: 1ch;
    }
  }
  input[type="radio"]::before {
    content: "";
    width: 0.75em;
    height: 0.75em;
    border-radius: 50%;
    transform: scale(0);
    transition: 20ms transform ease-in-out;
    box-shadow: inset 1em 1em var(--form-control-color);
  }

  input[type="radio"] {
    border-color: var(--slate-500);
  }

  input[type="radio"]:is(:focus-visible, :focus ){
    border-color: transparent;
  }

  input[type="radio"]:checked::before {
    transform: scale(1);
    isolation: isolate;
  }

  input[type="radio"]:focus {
    outline: max(2px, 0.15em) solid var(--clr-lime);
    outline-offset: max(2px, 0.15em);
    background-color: var(--clr-lime);
  }

  .form-control + .form-control {
    margin-block: 0.5ch;
  }

  .form-control:is(:hover, :focus) {
    background-color: hsla(61, 70%, 52%, 0.3);
    background-color: hsla(from var(--clr-lime) h s l / 30%);
  }
  .form-box {
  border: 1px solid var(--slate-700);
  border-radius: 4px;
  
}

.form-box:has(input[type="radio"]:checked){
    border: 2px solid var(--clr-lime);
  }
  

  .text{
    margin-inline-start: .5em;;
  }
</style>
