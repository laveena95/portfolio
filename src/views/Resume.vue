<template>
  <div>
      <ResumeInfo/>
      <CV/>
  </div>
</template>

<script>
import ResumeInfo from '../components/ResumeInfo';
import CV from '../components/CV';

export default {
    name: 'resume',
    components: {
        ResumeInfo,
        CV,
    }
}
</script>

<style>

</style>