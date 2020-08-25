<template>
  <div class="footer">
    <p>
      stay safe.
      <span>Stay brave</span>
    </p>
    <small>Jeremy Wambugu &copy; 2020</small>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  height: 10vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  letter-spacing: 0.2rem;
  border-top: 1px solid rgba(117, 116, 116, 0.445);
  p {
    font-size: 2rem;
    color: #fff;
    span {
      color: #f88949;
    }
  }
  small {
    font-size: 1.2rem;
    color: rgb(82, 80, 80);
  }
}
</style>