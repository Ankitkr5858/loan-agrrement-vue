<template>
  <div class="p-3">
    <b-card>
      <div class="d-flex">
        <span class="font-weight-bold mr-2">{{bankName}}</span>
        <b-badge pill variant="success" class="pt-1">Active</b-badge>
        <a class="text-primary font-weight-bold ml-auto">More <b-icon-chevron-right></b-icon-chevron-right></a>
      </div>
      <span class="text-primary small font-weight-bold">{{loanType}}</span>
      <div class="d-flex justify-content-between text-muted small">
        <span>Amount Due</span>
        <span>Interest Rate</span>
      </div>
      <div class="d-flex justify-content-between mb-2">
        <span class="font-weight-bold medium">$ {{dueAmt}}</span>
        <span class="font-weight-bold">{{interestRate}} %</span>
      </div>
      <div class="bg-light pb-2">
        <div class="d-flex align-items-center mb-2">
          <span
            class="ml-3 bg-primary p-1 d-icon rounded-circle text-white font-weight-bold"
          >
            $
          </span>
          <span class="ml-1 font-weight-bold">Interest and Fees </span>
        </div>
        <div class="d-flex justify-content-center mb-2">
          <div class="d-flex flex-column border-right pr-3">
            <span class="text-muted">Interest</span>
            <span class="font-weight-bold">$ 232.12</span>
          </div>
          <div class="d-flex flex-column pl-3">
            <span class="text-muted">Late Fees</span>
            <span class="font-weight-bold">$ 20.00</span>
          </div>
        </div>
        <div class="mb-2 small">
          Your statement contain interest and fees. which represent 14%of your
          statement balance
        </div>
      </div>
      <div class="d-flex">
        <button class="w-100 mx-2 btn btn-sm btn-outline-primary">
          Remind me later
        </button>
        <button class="w-100 mx-2 btn btn-sm btn-primary">Pay now</button>
      </div>
    </b-card>
  </div>
</template>
<script>
/**
 * 
 * bankName - Loan Bank Name
 * loanType - Enter Loan Type like Housing Loan or else
 * dueAmt - Enter Loan Due Amount
 * interestRate - Enter Interest Rate for loan
 */
export default {
  name: "LoanCard",
  components: {},
  props:['bankName','loanType',"dueAmt",'interestRate']
};
</script>