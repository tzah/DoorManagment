<template>
    <div class="fullPage">
        <div class="rooms-row">
            <div  v-for="room in getRoomsByDirection('bottom')" :key="room.name">
                <Room 
                  :isOpen="room.isOpen"
                  :name="room.name"
                  :doorDirection="room.doorDirection"/>
            </div>
        </div>
        <br/>
        <div class="rooms-row" >
            <div v-for="room in getRoomsByDirection('top')" :key="room.name">
                <Room 
                  :isOpen="room.isOpen"
                  :name="room.name"
                  :doorDirection="room.doorDirection"/>
            </div>
        </div>
    </div>
    
</template>
<script>
import Room from './Room.vue'

export default {
    name: 'Floor',

    data: () => ({
    }),
    components: {
        Room,
    },
    props: {
        rooms: {
            type: Array(),
            default: [],
        },
    },
    methods: {
        getRoomsByDirection(direction) {
            console.log(direction, this.rooms, this.rooms.filter(room => room.doorDirection === direction))
            return this.rooms.filter(room => room.doorDirection === direction);
        }
    }
}
</script>

<style scoped>
.rooms-row {
    display: flex;
}

.fullPage {
    height: 100%;
    width: 100%;
}
</style>