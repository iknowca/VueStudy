<template>
  <!--html파트는 templete에서 관리한다. -->
  <div class="about">
      <h1>This is an about page</h1>
      <p>{{ msg }}</p>
  </div>
</template>

<script>
export default {
    data() {
        return  {
            msg: "Hi, Hello, Vue.Js!",

        }
    }
}
</script>