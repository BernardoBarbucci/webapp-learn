<template>
    <section class="container-fluid d-flex flex-row">
        <AsideApp />
        <CalenderApp @calenderEvent="handleCalenderEvent" />
    </section>
</template>
  
<script>
import CalenderApp from '../components/CalenderApp.vue';
import AsideApp from '../components/AsideApp.vue';

export default {
    name: 'MainApp',
    components: {
        AsideApp,
        CalenderApp,
    },
    methods: {
        handleCalenderEvent(data) {
            // Gestisci l'evento proveniente da CalenderApp
            console.log('Calender event:', data);
        },
    },
};
</script>