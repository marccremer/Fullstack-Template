<script>
export default {
  async setup() {
    const API = 'http://localhost:3001'
    let data
    const res = await fetch(API+'/')
    data = await res.json()

    return {data}
  },
}
</script>

<template>
  <span>You got data: {{data}} </span>
</template>