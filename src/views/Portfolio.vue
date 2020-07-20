<template>
 <div>
     <PortfolioInfo/>
     <PortfolioTab/>
 </div>
</template>

<script>
import PortfolioInfo from '../components/PortfolioInfo';
import PortfolioTab from '../components/PortfolioTab';
export default {
    name : 'Portfolio',
    components : {
        PortfolioInfo,
        PortfolioTab,
    }
}
</script>

<style>

</style>