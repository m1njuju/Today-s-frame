<template>
  <div class="about pa-16">
    <h1>This is an {{$route.params.user}} 's page</h1>
  </div>
</template>

<script>
export default {
  name: 'AboutView',
  methods: {
    methodName: function() {
      this.$EventBus.$emit('eventName',this.$route.params.user)
    }
  }
}
</script>
