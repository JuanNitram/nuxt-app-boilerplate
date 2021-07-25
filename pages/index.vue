<template>
  <div>
    Welcome
  </div>
</template>

<script>
export default {
  mounted(){
    this.$auth.loginWith('local', {
      data: {
        email: '',
        password: ''
      }
    }).then(() => {
      console.log(this.$auth)
    });
  }
}
</script>
