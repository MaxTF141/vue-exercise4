<template>
    <div class="container-fluid d-flex justify-content-center my-5">
        <div class="row mx-5 px-5">
            <Div v-for="obj in hoodies" :key="obj.id" class="col-4 mx-auto my-4">
                <div class="card mx-auto" style="width: 18rem;">
                    <img :src="obj.image" class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">{{ obj.name }}</h5>
                        <h3>R {{ obj.price }}</h3>
                        <a href="#" class="btn btn-dark">Buy</a>
                    </div>
                </div>
            </Div>
        </div>
    </div>



</template>
<script>
export default {
    data() {
        return {
            hoodies: [
                {
                    id: 1,
                    name: "Essentials Oversize Hoodie Apricot",
                    size: "L",
                    image: "https://i.postimg.cc/d0tPsMNX/essentials-oversize-hoodie.webp",
                    price: 1396.34
                },
                {
                    id: 2,
                    name: "Essentials Oversize Hoodie Black",
                    size: "M",
                    image: "https://i.postimg.cc/j5F8YmBz/essentials-black-oversize-hoodie.webp",
                    price: 1396.34
                },
                {
                    id: 3,
                    name: "Essentials Oversize Hoodie White",
                    size: "XS",
                    image: "https://i.postimg.cc/DZp1Sx4v/O1-CN01-Cf-Kxh-I1-Rd-Pu-SFeop7-2067872134-0-cib-700x.webp",
                    price: 143.99
                },
                {
                    id: 4,
                    name: "Essentials Oversize Hoodie Khaki",
                    size: "M",
                    image: "https://i.postimg.cc/DZ1HPbFb/O1-CN01-Ry-Xui-Q1-Rd-Pu-Ux-ZYl2-2067872134-0-cib-700x.webp",
                    price: 143.99
                },
                {
                    id: 5,
                    name: "Essentials Oversize Hoodie Khaki",
                    size: "M",
                    image: "https://i.postimg.cc/DZ1HPbFb/O1-CN01-Ry-Xui-Q1-Rd-Pu-Ux-ZYl2-2067872134-0-cib-700x.webp",
                    price: 143.99
                },
                {
                    id: 6,
                    name: "Essentials Oversize Hoodie Khaki",
                    size: "M",
                    image: "https://i.postimg.cc/DZ1HPbFb/O1-CN01-Ry-Xui-Q1-Rd-Pu-Ux-ZYl2-2067872134-0-cib-700x.webp",
                    price: 143.99
                }
            ]
        }

    },
    created() {
        localStorage.setItem('hoodies', JSON.stringify(this.hoodies))
    }

}
</script>
<style>

</style>