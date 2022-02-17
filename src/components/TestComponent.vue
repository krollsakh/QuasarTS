<template>
  <h6>Component Test</h6>
  <p>Prop msg = {{ msg }}</p>
  <p>Prop labels = {{ labels }}</p>
</template>

<script lang="ts" setup>

interface Props {
  msg?: string
  labels?: string[]
}

withDefaults(defineProps<Props>(), {
  msg: 'hello',
  label: () => ['one', 'two']
})

</script>
