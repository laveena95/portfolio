<template>
<div>
    <Info/>
    <Skill/>
</div>
</template>

<script>

import Info from '../components/Info';
import Skill from '../components/Skill';

export default {
  name: 'Home',
  components: {
    Info,
    Skill,
  }
}
</script>