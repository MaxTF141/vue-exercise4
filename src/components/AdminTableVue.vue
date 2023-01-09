<template>
    <table class="table">
        <thead>
            <tr>
                <th scope="col">ID</th>
                <th scope="col">NAME</th>
                <th scope="col">SIZE</th>
                <th scope="col">PRICE</th>
            </tr>
        </thead>
        <tbody>
            <Tr v-for="hoodie in hoodies" :key="hoodie.id">
                <th scope="row">{{ hoodie.id }}</th>
                <td>{{ hoodie.name }}</td>
                <td>{{ hoodie.size }}</td>
                <td class="d-flex justify-content-between">{{ hoodie.price }} <i class="fa-sharp fa-solid fa-trash me-4"></i></td>
            </Tr>
        </tbody>
    </table>
    <button class="btn btn-primary bg-dark d-block mx-auto ">ADD A PRODUCTS</button>
</template>
<script>
export default {
    data(){
        return {
            hoodies:[]
        }
    },
    created(){
        let savedHoodies = JSON.parse(localStorage.getItem('hoodies'))
        if(savedHoodies){
            this.hoodies = savedHoodies
        }
    }
}
</script>
<style>
    .btn {
        font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
        color: grey;
    }
</style>