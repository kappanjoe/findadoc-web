<template>
    <div class="h-full">
        <TopNav />
        <div class="flex flex-col md:flex-row h-full">
            <WelcomeHero />
            <FeaturedNews />
        </div>
        <div class="w-full">
            <MediaBanner />
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
    props: {
        name: {
            type: String,
            default: '',
        },
        msg: { 
            type: String, 
            required: false,
            default: '',
        }
    },
    data() {
        return {
            count: 1
        }
    },
    mounted() {
    }
})
</script>
