<template>
  <div>
    <h3><font-awesome-icon :icon="briefcaseIcon" />  Pacotes:</h3>
    
  </div>


</template>

<script>
  import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
  import { faBriefcase } from '@fortawesome/free-solid-svg-icons';
  
  export default{
    name: 'pacotes-view',
    components:{
      FontAwesomeIcon
    },
    data() {
      return {
        briefcaseIcon: faBriefcase
      }
    }
  }

</script>

<style>

</style>