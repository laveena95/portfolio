<template>
<div>
    <Info/>
    <Skill/>
    <Hero/>
    <Project/>
    <Blog/>
</div>
</template>

<script>

import Info from '../components/Info';
import Skill from '../components/Skill';
import Hero from '../components/Hero';
import Project from '../components/Project';
import Blog from '../components/Blog';

export default {
  name: 'Home',
  components: {
    Info,
    Skill,
    Hero,
    Project,
    Blog,
  }
}
</script>