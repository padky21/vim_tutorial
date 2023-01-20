<template>
  <form action="">
    <InputText/>
    <input-text/>
    <submit/>
  </form>
</template>
<script>
  import InputText from "@/components/Form/InputText";
  import Submit from "@/components/Form/Submit";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Form',
  components: {
    InputText,
    Submit
  }
}
</script>