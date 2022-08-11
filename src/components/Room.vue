<template>
    <div class="frame">
        <div>
            <div :class= "`${isOpen ? 'open' : 'close'} ${doorDirection === 'bottom' ? 'buttom' : 'top'}`"/>
        </div>
         <div :class="`name-container ${doorDirection === 'top' ? 'name-bottom' : 'name-top'}`">
            <p class="name">{{name}}</p>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Room',

    data: () => ({
    }),
    props: {
        isOpen: {
            type: Boolean,
            default: false,
        },
        name: {
            type: String,
            default: "room",
        },
        doorDirection: {
            type: String,
            default: "bottom"
        }
    }
}
</script>