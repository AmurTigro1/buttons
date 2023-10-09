<template>
    <div class="container">
        <h2>Josephen Stern Salera</h2>
        <div class="buttons">
            <h4>Buttons</h4>
            <RegularB style="flex: 1" title="Regular" type="regular" />
            <RegularB style="flex: 1" title="Happy" type="happy" />
            <RegularB style="flex: 1" title="Sad" type="sad" />
            <RegularB style="flex: 1" title="Angry" type="angry" />
        </div>

        </div>
</template>

<script>
import RegularB from './RegularB.vue';

export default {
    props: {
        person: Object
    },
    components: {
        RegularB,
    }
}

</script>

<style scoped>
img {
    width: 100%;
}
h2 {
    border-bottom: 1px solid black;
}
.buttons {
    display: flex;
    gap: 4px;
}
.container {
    max-width: 900px;
    border: 1px solid #888;
    padding: 12px;
    border-radius: 8px;
    box-shadow: 0px 0px 5px #888;
    margin: 16px 0;
    height: 100vh;
}
</style>