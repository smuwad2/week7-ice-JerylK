<script>
    export default { 
        // Add code in appropriate places
        data() {
            return {
                items: ['keyboard', 'mouse', 'iPhone', 'macbook', 'adapter'],
                item: ''
            }
            
        }
    }
</script>

<template>

    <h2>Shopping Cart</h2>
    <!-- TODO: Add Code Here -->
    <ul>
        <li v-for="item in items">{{ item }}<button @click="$event.target.parentElement.remove()">Delete!</button></li>
    </ul>
   
    <input type="text" v-model="item"><button @click="items.push(item); item=''">Add!</button>
</template>
