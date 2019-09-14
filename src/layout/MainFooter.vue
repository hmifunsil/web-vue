<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https:///presentation.creative-tim.com">
              Terms
            </a>
          </li>
          <li>
            <a href="https:///blog.creative-tim.com">
              Privacy
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        Copyright &copy; {{ year }} - HMIF Siliwangi University All Right
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
