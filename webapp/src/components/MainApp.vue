<template>
    <section class="container-fluid d-flex flex-row">
        <AsideApp class="col-2" />
        <CalenderApp class="col-10" />
    </section>
</template>
  
<script>
import CalenderApp from '../components/CalenderApp.vue';
import AsideApp from '../components/AsideApp.vue';

export default {
    name: 'main',
    components: {
        AsideApp,
        CalenderApp
    }
};
</script>
  