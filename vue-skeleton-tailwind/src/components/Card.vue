<template>
    <div class="w-72 bg-white rounded shadow-2xl">
        <!-- image -->
        <div class="h-48 bg-gray-200 rounded-tr rounded-tl">
            <img src="~@/assets/images/tanjiro.jpg" class="h-48 w-full object-fill" alt="Tanjiro Kamado">
        </div>

        <div class="p-5">
            <!-- title -->
            <div class="h-6 rounded-sm mb-4">
                <h1 class="font-semibold text-gray-600 text-lg">{{dataCard.cardTitle}}</h1>
            </div>

            <!-- content -->
            <div class="text-left">
                <div class="h-42 bg-gray-200 rounded-sm px-2 py-2">
                    <p class="break-words text-sm text-gray-700">{{dataCard.bio}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script lang='ts'>
import { defineComponent,ref } from 'vue';

const loadCardData = async() =>{
    return new Promise((resolve)=>{
        setTimeout(()=>{
            resolve({
                cardTitle: "Tanjiro Kamado",
                bio:"A jornada de Tanjiro tem como fio principal 2 objetivos: transformar sua irmã novamente em humana e se vingar do demônio que destruiu sua família."
            });
        },3000);
    });
};
const Card = defineComponent({

    async setup(){
        const dataCard = ref(await loadCardData());

        return{
            dataCard
        };
    }

});

export default Card;
</script>

<style>

</style>