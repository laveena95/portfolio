<template>
  <div>
      <ContactInfo/>
      <ContactForm/>
  </div>
</template>

<script>
import ContactInfo from '../components/ContactInfo';
import ContactForm from '../components/ContactForm';

export default {
    name: 'contact',
    components: {
        ContactInfo,
        ContactForm,
    }

}
</script>

<style>

</style>