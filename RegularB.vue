<template>
    <div :class="type">
        {{title}}
    </div>
</template>

<script>

export default {
    props: {
        title: String,
        type: String //primary, danger, warning, success
    }
}

</script>

<style scoped>
.regular {
    background-color: #2686e7;
    border-color: #06386a;
}
.angry {
    background-color: #e72636;
    border-color: #6a0609;
}
.sad {
    background-color: #e76326;
    border-color: #6a1806;
}
.happy {
    background-color: #11c839;
    border-color: #045e22;
}
div {
    padding: 4px;
    color: white;
    border-radius: 4px;
    border: 4px solid;
    margin: 8px 0;
    text-align: center;
}
</style>