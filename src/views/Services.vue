<template>
  <div>
      <ServiceInfo/>
      <ServicePackage/>
      <FAQ/>
  </div>
</template>

<script>
import ServiceInfo from '../components/ServiceInfo';
import ServicePackage from '../components/ServicePackage';
import FAQ from '../components/FAQ';

export default {
    name: 'services',
    components: {
        ServiceInfo,
        ServicePackage,
        FAQ,
    }
}
</script>

<style>

</style>