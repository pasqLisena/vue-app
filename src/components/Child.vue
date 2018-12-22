<template>
  <div>
    <p>Visualising a Message:</p>
    <span>{{myMessage}}</span>
  </div>
</template>

<script>
  export default {
      props: {
         'myMessage': {
           type: String,
           required: true
          }
      }
  }
</script>
