<template>
  <div id="app">
    <Loan />
  </div>
</template>

<script>
import Loan from "./components/page/Loan";
export default {
  name: "App",
  components: { Loan },
};
</script>
<style>
.d-icon {
  height: 30px;
  width: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.underline {
  border-bottom: 2px solid;
}
.card-body {
  padding: 0.7rem;
}
</style>
