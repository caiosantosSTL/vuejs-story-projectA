<template>
    <div class="container">
        <div class="row">
            <div style="height: 100px;"><!-- space --></div>
            <div class="d-flex align-items-center justify-content-center">
                <h1>Stories home</h1>
            </div>
            <div style="height: 100px;"><!-- space --></div>

            <div class="d-flex flex-row flex-wrap justify-content-center">
                
                <div v-for="info, id in infos" :key="id">
                    <card-x-vue :info='info'></card-x-vue>
                </div>
            </div>


        </div>
    </div>
</template>

<script>
    import cardXVue from './cards/cardX.vue'
    export default {
        components: { cardXVue },
        name: 'homeNews',
        data() {
            return {
                infos: [
                    { id: 1, title: 'Story 1', by: 'sssss', ff: '123213' },
                    { id: 2, title: 'Story 2', by: 'ffffff', ff: '3424' },
                    { id: 3, title: 'Story 3', by: 'erw', ff: '346' },
                    { id: 4, title: 'Story 4', by: 'ewrty', ff: '346' },
                    { id: 5, title: 'Story 5', by: 'rwryy', ff: '346' },
                ]
            }

        }
    }
</script>

<style>

</style>