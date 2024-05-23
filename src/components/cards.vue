<template>
<div class="caards container mx-auto  grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 space-x-1 mt-11 ">
    <div v-for="n in 3" :key="n">

        <div class="group">
            <div class="icon mb-5">
                <img src="../assets/images/icon-cols-1.png" alt="">
            </div>
            <div class="textt text-2xl font-semibold">
                <h1>Built by creative people.</h1>
            </div>
            <div class="paraa justify-center item-center mt-3">
                <p>Moderne is the product of a team of art-directors, copywriters and developers who are passionate about
                    creativity</p>
            </div>
        </div>

    </div>
</div>
</template>

<script>

</script>

<style scoped></style>
