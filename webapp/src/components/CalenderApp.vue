<template>
    <section class="col-10">
        <h1 @click="emitCalenderEvent">
            CALENDAR
        </h1>
    </section>
</template>
  
<script>
export default {
    name: 'CalenderApp',
    methods: {
        emitCalenderEvent() {
            // Emetti un evento verso il componente padre (MainApp)
            this.$emit('calenderEvent', { eventData: 'Qualsiasi dato' });
        },
    },
};
</script>