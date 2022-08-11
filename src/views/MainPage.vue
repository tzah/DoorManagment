<template>
    <div class="container">
        <Floor :rooms="rooms"/>
    </div>
</template>
<script>
import Floor from '../components/Floor.vue'

export default {
    name: 'MainPage',

    data: () => ({
        rooms: [{
            isOpen: true,
            name: "door 1",
            doorDirection: "top",
        }, {
            isOpen: true,
            name: "door 2",
            direcdoorDirectiontion: "bottom",
        }, {
            isOpen: false,
            name: "door 3",
            doorDirection: "top",
        }, {
            isOpen: false,
            name: "door 4",
            doorDirection: "top",
        }, {
            isOpen: true,
            name: "door 5",
            doorDirection: "bottom",
        }, {
            isOpen: true,
            name: "door 6",
            doorDirection: "bottom",
        }, {
            isOpen: false,
            name: "door 7",
            doorDirection: "top",
        }, {
            isOpen: true,
            name: "door 8",
            doorDirection: "bottom",
        }, {
            isOpen: true,
            name: "door 9",
            doorDirection: "top",
        }, {
            isOpen: false,
            name: "door 10",
            doorDirection: "top",
        }, {
            isOpen: true,
            name: "door 11",
            doorDirection: "bottom",
        }, {
            isOpen: false,
            name: "door 12",
            doorDirection: "bottom",
        }, {
            isOpen: true,
            name: "door 13",
            doorDirection: "bottom",
        }, {
            isOpen: false,
            name: "door 12",
            doorDirection: "top",
        }, {
            isOpen: true,
            name: "door 13",
            doorDirection: "bottom",
        }
        ]
    }),
    components: {
        Floor,
    }
}
</script>

<style scoped>
.container {
    padding: 25vh;

    justify-content: center;
}
</style>