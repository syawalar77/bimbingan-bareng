<template>
    <div>
        <button 
            class="btn text-light"
            @button="$emit('update', $event.target.value)">
            {{ titleBtn }}
        </button>
    </div>
</template>

<script>
export default {
    props: {
        titleBtn: {
            type: String,
            default: "Daftar",
        }
    }

}
</script>

<style>
.btn {
    border: 1px solid white;
    width: 120px;

}

</style>