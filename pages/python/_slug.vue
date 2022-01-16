<template>
<div class="flex">

    <div class="w-80 py-10 px-8 border-r border-slate-600">
        <div class="font-semibold text-slate-600 text-lg mb-3">파이썬 기초 문법</div>

        <div v-for='list of python_list' :key="list">
                <nuxt-link :to='`${list.slug}`'>
                <div class="group">
                    <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">{{list.slug}}. {{list.title}}</div>
                </div>
                </nuxt-link>
        </div>
    </div>

    <div class="w-full">

        <CourseHeader />

        <div class="max-w-5xl pt-10 pb-24 px-5 mx-auto">
            <p class="custom-text leading-snug md:leading-normal px-5 md:px-0 mb-8 text-3xl text-gray-800 title font-semibold">{{python.slug}}. {{python.title}}</p>

            <nuxt-content :document="python" class="prose max-w-5xl custom-text"/>
        </div>
    </div>

</div>
</template>

<script>
export default {
async asyncData({ $content, params }) {
        const python = await $content('python', params.slug)
        .fetch();
        
        const python_list = await $content('python')
        .sortBy('slug', 'asc')
        .fetch();
        return { python, python_list }
    }
}
</script>

<style scoped>
.keep-all{
    word-break: keep-all;
}
</style>