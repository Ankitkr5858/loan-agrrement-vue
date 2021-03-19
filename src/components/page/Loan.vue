<template>
  <div>
    <h5 class="text-center border-bottom">Loans</h5>
    <div class="d-flex justify-content-around">
      <span class="font-weight-bold underline nav-item active text-primary"
        >Active Loans</span
      >
      <span class="font-weight-bold">Completed</span>
      <span class="text-muted">In progress</span>
    </div>
    <LoanCard bankName="American Express" loanType="Housing Loan" dueAmt="400.00" intrestRate="9.00"/>
    <LoanCard bankName="Citi Bank" loanType="Car Loan" dueAmt="300.00" intrestRate="8.00"/>
    <div class="d-flex justify-content-between p-2 fixed-bottom border-top">
      <div
        class="d-flex flex-column justify-content-center align-items-center p-2"
      >
        <b-icon-grid></b-icon-grid>
        Dashboard
      </div>
      <div
        class="d-flex flex-column justify-content-center align-items-center p-2 text-primary"
      >
        <b-icon-journal></b-icon-journal>
        Loans
      </div>
      <div
        class="d-flex flex-column justify-content-center align-items-center p-2"
      >
        <b-icon-person></b-icon-person>
        Profile
      </div>
    </div>
  </div>
</template>
<script>
// This is page for loan screen
import LoanCard from "@/components/LoanCard";
export default {
  name: "Loan",
  components: { LoanCard },
};
</script>