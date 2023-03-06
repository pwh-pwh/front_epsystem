<template>
    <IFrame :src="url"/>
</template>

<script>
    import IFrame from "../../components/IFrame";
    export default {
        name: "Swagger",
        components: {IFrame},
        data() {
            return{
                url: process.env.VUE_APP_URL+"swagger-ui/index.html"
            }
        }
    }
</script>
