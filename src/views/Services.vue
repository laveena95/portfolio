<template>
  <div>
      <ServiceInfo/>
      <ServicePackage/>
  </div>
</template>

<script>
import ServiceInfo from '../components/ServiceInfo';
import ServicePackage from '../components/ServicePackage';

export default {
    name: 'services',
    components: {
        ServiceInfo,
        ServicePackage,
    }
}
</script>

<style>

</style>