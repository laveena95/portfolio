<template>
<div>
    <Info/>
    <Skill/>
    <Hero/>
    <Project/>
</div>
</template>

<script>

import Info from '../components/Info';
import Skill from '../components/Skill';
import Hero from '../components/Hero';
import Project from '../components/Project';

export default {
  name: 'Home',
  components: {
    Info,
    Skill,
    Hero,
    Project,
  }
}
</script>