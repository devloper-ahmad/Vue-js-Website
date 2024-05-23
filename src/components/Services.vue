<script>


export default {
    name: "Services",
    data() {
        return {
            cards: [{
                    title: "Collaboration",
                    heading: "Improve Collaboration",
                    description: "This is a sample card content. You can put any information you want here.",
                    image: "https://moderne.st/images/illustrations/cards-1.png",
                    bgColor: "bg-white",
                    textColor: "text-[#be7558]",
                    descriptionColor: "text-gray-100",
                    headingColor: "text-[#be7558]"

                },
                {
                    title: "Brainstorms.",
                    heading: "Present better.",
                    description: " Turn your great ideas into clean and beautiful presentations.",
                    image: "https://moderne.st/images/illustrations/cards-2.png",
                    bgColor: "bg-white",
                    titlecolor: "!bg-[#bdedd5]",
                    textColor: "text-[#3d9f6e]",
                    headingColor: "text-[#3d9f6e]"
                },
                {
                    title: "Creativity.",
                    heading: "Encourage creativity.",
                    description: " Spice up your team’s potential with best insights and ideas.",
                    image: "https://moderne.st/images/illustrations/cards-1.png",
                    titlecolor: "bg-[#fdd7f5]",
                    bgColor: "bg-white",
                    textColor: "text-[#b358be]",
                    headingColor: "text-[#b358be]"
                },
            ],
        };
    },
    methods: {
        changeColor(index) {
            const newColors = ['bg-blue-200', 'bg-green-200', 'bg-red-200', 'bg-yellow-200', 'bg-purple-200'];
            const currentColor = this.cards[index].bgColor;
            let newColor = newColors[Math.floor(Math.random() * newColors.length)];

            // Ensure the new background color is different from the current color
            while (newColor === currentColor) {
                newColor = newColors[Math.floor(Math.random() * newColors.length)];
            }

            // Define new text colors
            const textColors = ['text-gray-800', 'text-gray-600', 'text-blue-800', 'text-green-800', 'text-red-800'];
            let newTitleColor = textColors[Math.floor(Math.random() * textColors.length)];
            let newDescriptionColor = textColors[Math.floor(Math.random() * textColors.length)];

            // Ensure the new title and description colors are different from the current ones
            while (newTitleColor === this.cards[index].titleColor) {
                newTitleColor = textColors[Math.floor(Math.random() * textColors.length)];
            }
            while (newDescriptionColor === this.cards[index].descriptionColor) {
                newDescriptionColor = textColors[Math.floor(Math.random() * textColors.length)];
            }

            this.$set(this.cards, index, {
                ...this.cards[index],
                bgColor: newColor,
                titleColor: newTitleColor,
                descriptionColor: newDescriptionColor,
            });
        },
    },
};
</script>

<template>
<section class="Services container mx-auto ">
    <div class="caards container mt-24 grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 mx-6 px-5 ">
        <div v-for="(card, index) in cards" :key="index" :class="['w-[350px] h-[513.8px] rounded-lg shadow-lg custom-padding', card.bgColor]" @click="changeColor(index)">
            <h3 class="text-base font-bold text- mb-4 px-5 py-1 w-36 rounded-sm bg-[#fdd5c3]" :class="[card.titlecolor,card.textColor]">{{ card.title }}</h3>
            <img :src="card.image" alt="">
            <h1 class="mt-8 text-2xl font-semibold" :class="[card.headingColor]">{{ card.heading }}</h1>
            <p class="text-lg font-medium mt-5 text-[#7a7780] card.descriptionColor">{{ card.description }}</p>

        </div>
    </div>

</section>
</template>

<style>
.custom-padding {
    padding: 27px 28px 24px;
}
</style>
