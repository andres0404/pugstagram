<script>
  // import Share from "./Share.svelte";
</script>
<div class="Modal">
  <div class="Modal-overlay">
  </div>
</div>
<style>
    .Modal {
    position: relative;
  }
  .Modal-overlay {
    background-color: rgba(0, 0, 0, 0.5);
    color: aliceblue;
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 8;
    cursor: pointer;
  }
</style>