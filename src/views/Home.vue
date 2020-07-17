<template>
<div>
    <Info/>
    <Skill/>
    <Hero/>
</div>
</template>

<script>

import Info from '../components/Info';
import Skill from '../components/Skill';
import Hero from '../components/Hero';

export default {
  name: 'Home',
  components: {
    Info,
    Skill,
    Hero,
  }
}
</script>