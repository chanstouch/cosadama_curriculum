<template>
<div class="flex">

    <div class="hidden md:block w-80 min-w-max py-10 px-8 border-r border-slate-600 min-h-screen">

        <div class="font-semibold text-slate-600 text-xl mb-4">{{currilist[0]["name"]}}</div>

        <div>

            <div v-if="cat_1==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_1}}</div>

                <div v-for='list of list_1' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_2==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_2}}</div>

                <div v-for='list of list_2' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_3==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_3}}</div>

                <div v-for='list of list_3' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_4==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_4}}</div>

                <div v-for='list of list_4' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_5==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_5}}</div>

                <div v-for='list of list_5' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_6==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_6}}</div>

                <div v-for='list of list_6' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_7==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_7}}</div>

                <div v-for='list of list_7' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_8==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_8}}</div>

                <div v-for='list of list_2' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_9==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_9}}</div>

                <div v-for='list of list_9' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

            <div v-if="cat_10==null"></div>
            <div v-else>
                <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_10}}</div>

                <div v-for='list of list_10' :key="list" class="pl-5">
                        <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                        <div class="group">
                            <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                {{list.slug}}. {{list.title}}
                            </div>
                        </div>
                        </nuxt-link>
                </div>
            </div>

        </div>

        <div class="pt-3.5 text-sm text-slate-400">커리 개발: {{currilist[0]["authors"][0]}} {{currilist[0]["authors"][1]}}</div>

    </div>

    <div class="w-full">

        <!-- 헤더  -->

        <div class="px-5 md:px-10 py-0 md:py-2">
            <div class="border-b border-slate-400 h-16 mx-auto flex items-center justify-between">
                    <div class="flex">
                        <div class="md:hidden flex content-center">
                            <button @click="drawer">
                            <Menu class="mr-1"/>
                            </button>
                        </div>
                        <nuxt-link to='/'> <Logo class="drop-shadow-sm pl-2" /> </nuxt-link>
                    </div>
                    <div class="group pr-3">
                        <a href="https://github.com/Team-COSADAMA" target="blank" class="">
                            <GithubLogo />
                        </a>
                    </div>
            </div>
            <transition
                enter-class="opacity-0"
                enter-active-class="ease-out transition-medium"
                enter-to-class="opacity-100"
                leave-class="opacity-100"
                leave-active-class="ease-out transition-medium"
                leave-to-class="opacity-0"
            >
                <div @keydown.esc="isOpen = false" v-show="isOpen" class="z-10 fixed inset-0 transition-opacity">
                    <div @click="isOpen = false" class="absolute inset-0 bg-black opacity-50" tabindex="0"></div>
                </div>
            </transition>

            <aside class="p-5 transform top-0 left-0 w-64 bg-white fixed h-full overflow-auto ease-in-out transition-all duration-300 z-30" :class="isOpen ? 'translate-x-0' : '-translate-x-full'">
                
                <div class="close">
                <button class="absolute top-0 right-0 mt-4 mr-4" @click=" isOpen = false">
                    <Close />
                </button>
                </div>

                <div class="px-4">
                    <div class="font-semibold text-slate-600 pt-10 text-xl mb-4">{{currilist[0]["name"]}}</div>

                    <div>

                        <div v-if="cat_1==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_1}}</div>

                            <div v-for='list of list_1' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_2==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_2}}</div>

                            <div v-for='list of list_2' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_3==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_3}}</div>

                            <div v-for='list of list_3' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_4==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_4}}</div>

                            <div v-for='list of list_4' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_5==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_5}}</div>

                            <div v-for='list of list_5' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_6==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_6}}</div>

                            <div v-for='list of list_6' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_7==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_7}}</div>

                            <div v-for='list of list_7' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_8==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_8}}</div>

                            <div v-for='list of list_2' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_9==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_9}}</div>

                            <div v-for='list of list_9' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                        <div v-if="cat_10==null"></div>
                        <div v-else>
                            <div class="font-medium text-slate-600 text-lg mb-2.5">{{cat_10}}</div>

                            <div v-for='list of list_10' :key="list" class="pl-5">
                                    <nuxt-link :to="{path: `/${currititle}/${list.slug}`}" replace>
                                    <div class="group">
                                        <div class="keep-all text-slate-600 text mb-2 group-hover:text-blue-500 transition duration-200">
                                            {{list.slug}}. {{list.title}}
                                        </div>
                                    </div>
                                    </nuxt-link>
                            </div>
                        </div>

                    </div>

                    <div class="pt-3.5 text-sm text-slate-400">커리 개발: {{currilist[0]["authors"][0]}} {{currilist[0]["authors"][1]}}</div>
                </div>

            </aside>
        </div>

        <!-- 커리큘럼  -->

        <div class="max-w-5xl pt-8 pb-24 px-6 md:px-11 mx-auto">
            <p class="custom-text leading-normal mb-6 text-lg text-slate-600 font-medium">{{python.category}} > {{python.slug}}. {{python.title}}</p>
            <p class="custom-text leading-normal mb-8 text-3xl text-slate-800 font-semibold">{{python.title}}</p>

            <nuxt-content :document="python" class="prose max-w-5xl custom-text"/>

            <Prevnext :prev="prev" :next="next" :currititle="currititle" />

        </div>
    </div>

</div>
</template>

<script>
export default {
    data() {
        return {
        isOpen: false
        };
    },
    methods: {
        drawer() {
        this.isOpen = !this.isOpen;
        }
    },
    watch: {
        isOpen: {
        immediate: true,
        handler(isOpen) {
            if (process.client) {
            if (isOpen) document.body.style.setProperty("overflow", "hidden");
            else document.body.style.removeProperty("overflow");
            }
        }
        }
    },
    mounted() {
        document.addEventListener("keydown", e => {
        if (e.keyCode == 27 && this.isOpen) this.isOpen = false;
        });
    },
async asyncData({ $content, params }) {
        const python = await $content('python', params.slug)
        .fetch();

        const currilist = await $content('courses')
        .where({slug: 'python'})
        .fetch();

        const currititle = currilist[0]["slug"]

        const cat_1 = currilist[0]["category"][0]
        const cat_2 = currilist[0]["category"][1]
        const cat_3 = currilist[0]["category"][2]
        const cat_4 = currilist[0]["category"][3]
        const cat_5 = currilist[0]["category"][4]
        const cat_6 = currilist[0]["category"][5]
        const cat_7 = currilist[0]["category"][6]
        const cat_8 = currilist[0]["category"][7]
        const cat_9 = currilist[0]["category"][8]
        const cat_10 = currilist[0]["category"][9]

        const list_1 = await $content('python')
        .where({category: cat_1})
        .sortBy('slug', 'asc')
        .fetch();

        const list_2 = await $content('python')
        .where({category: cat_2})
        .sortBy('slug', 'asc')
        .fetch();

        const list_3 = await $content('python')
        .where({category: cat_3})
        .sortBy('slug', 'asc')
        .fetch();

        const list_4 = await $content('python')
        .where({category: cat_4})
        .sortBy('slug', 'asc')
        .fetch();

        const list_5 = await $content('python')
        .where({category: cat_5})
        .sortBy('slug', 'asc')
        .fetch();

        const list_6 = await $content('python')
        .where({category: cat_6})
        .sortBy('slug', 'asc')
        .fetch();

        const list_7 = await $content('python')
        .where({category: cat_7})
        .sortBy('slug', 'asc')
        .fetch();

        const list_8 = await $content('python')
        .where({category: cat_8})
        .sortBy('slug', 'asc')
        .fetch();

        const list_9 = await $content('python')
        .where({category: cat_2})
        .sortBy('slug', 'asc')
        .fetch();

        const list_10 = await $content('python')
        .where({category: cat_10})
        .sortBy('slug', 'asc')
        .fetch();

        const [prev, next] = await $content('python')
        .only(['title', 'slug'])
        .sortBy('slug', 'asc')
        .surround(params.slug)
        .fetch();

        return { python, currilist, 
        cat_1, cat_2, cat_3, cat_4, cat_5, cat_6, cat_7, cat_8, cat_9, cat_10,
        list_1, list_2, list_3, list_4, list_5, list_6, list_7, list_8, list_9, list_10,
        prev, next, currititle
        }
    }
}
</script>

<style scoped>
.keep-all{
    word-break: keep-all;
}
code::before {
    content: none !important;
}
code::after {
    content: none !important;
}
</style>