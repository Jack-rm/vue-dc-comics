<template>
<div class="my_comic-element">
    <div class="my_comic-img">
        <img :src="source" :alt="title">
    </div>
    <h3>{{ title }}</h3>
</div>
</template>

<script>
export default {
    name: 'Box',
    props: ['title', 'source']
}
</script>

<style lang="scss" scoped>

.my_comic-element{
    flex-basis: calc(100% / 6);
    padding-top: 50px;
    text-align: left;

    & h3 {
        color: white;
        text-transform: uppercase;
        font-size: 0.9em;
        padding-top: 15px;
    }
}

.my_comic-img{
    height: 200px;
    overflow: hidden;
}

</style>