<script setup>
import { toRefs, reactive } from 'vue';
import { Link, router } from '@inertiajs/vue3';

import AccountMultiple from 'vue-material-design-icons/AccountMultiple.vue' 
import ThumbUp from 'vue-material-design-icons/ThumbUp.vue'
import Check from 'vue-material-design-icons/Check.vue'
import Delete from 'vue-material-design-icons/Delete.vue'

import { useGeneralStore } from '@/stores/general';
import { storeToRefs } from 'pinia';
const useGeneral = useGeneralStore()
// const { isImageDisplay} = storeToRefs(useGeneral)

const form = reactive({ comment:null })

// const props = defineProps({
//     use: Object,
//     post: Object,
//     comments: Object,
// });

// const { post, user, comments } = toRefs(props)

</script>

<template>
    <div id="Post" class="w-full bg-white rounded-lg my-4 shadow-md">
        <div class="flex items-center py-3 px-3">
            <button class="mr-2">
                <img class="rounded-full ml-1 min-w-[42px] max-h-[42px]" src="https://picsum.photos/id/87/300/320">
            </button>
        </div>
    </div>
</template>