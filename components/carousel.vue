<template>
    <div data-aos="fade-right" data-aos-duration="3000" class="heroBlock mt-20">
        <v-carousel cycle hide-delimiters show-arrows="hover" width="40vh">
            <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src" reverse-transition="fade-transition"
                transition="fade-transition">
                <v-row class="title fill-height hidden-xs-only" align="center" justify="center">{{ item.title }}</v-row>
            </v-carousel-item>
        </v-carousel>
    </div>
</template>
  
<script>
import AOS from "aos";
import "aos/dist/aos.css";
export default {
    name: "Hero",
    data() {
        return {
            items: [
                {
                    src: 'https://i.ibb.co/wQ97NS7/3081648.jpg',
                },
                {
                    src: 'https://i.ibb.co/fvDy6rd/4380.jpg',
                },
                {
                    src: 'https://i.ibb.co/wQ97NS7/3081648.jpg',
                },
                {
                    src: 'https://i.ibb.co/fvDy6rd/4380.jpg',
                },
            ]
        };
    },


    mounted() {
        AOS.init({});
    },
};

</script>