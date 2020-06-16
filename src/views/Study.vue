<template>
    <div class="study">
        <button @click="tap">点击</button>
    </div>
</template>
<script>
    export default {
        name: "Study",
        data(){
            return {
                arr : ['Tom', 'Mary', 'Peter', 'Jack'],
                baseData : [
                    {
                        name: 'xulin',
                        age: 29
                    },
                    {
                        name: 'hui',
                        age: 28
                    }
                ]
            }
        },
        methods: {
            getDate(data){
                data.forEach((item, index, myArr) => {
                    console.log(item)
                })
            },
            tap: function(){
                this.getDate(this.baseData);
            }
        }
    };
</script>