<template>
    <div class="form-wrapper">
        <form name="form" class="form">
            <input v-model="newValue" type="text" name="input-text" placeholder="Type something...">
            <button @click.prevent="addToArray">Save!</button>
        </form>
        <ul class="list">
            <li v-for="(value, key) in componentArray" v-bind:key="key">
                <p>{{ key }}</p> 
                <p>{{ value }}</p> 
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "simple-form",
    props: {
        myArray: Array,
    },
    data() {
        return {
            newValue: "",
            componentArray: this.myArray,
            }
    },
    methods: {
        addToArray() {
            // let value = this.newValue;
            console.log('todoArray: ');
            // console.log(value);
            this.componentArray.push(this.newValue);
        },
    },
    
}
</script>