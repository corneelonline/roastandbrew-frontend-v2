<template>
  <div id="register">

  </div>
</template>

<script>
export default {
  data(){
    return {
      form: {
        name: '',
        email: '',
        password: '',
        confirm_password: ''
      },
      validations: {
        name: {
          valid: true,
          message: ''
        },
        email: {
          valid: true,
          message: ''
        },
        password: {
          valid: true,
          message: ''
        },
        confirm_password: {
          valid: true,
          message: ''
        }
      }
    }
  },
}
</script>

<style lang="scss" scoped>

</style>
