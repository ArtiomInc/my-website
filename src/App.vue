<template>
    <v-app id="bg">
        <v-card
        height="100%"
        color="transparent"
        >

            <v-container
            fill-height
            fluid
            >

                <v-row
                align="center"
                justify="center"
                >

                    <div>

                        <v-row
                        align="center"
                        justify="center"
                        class="mb-7"
                        >
                            <v-img
                            max-width="200"
                            src="../src/assets/my_logo_square.png"></v-img>
                        </v-row>

                        <v-row>
                            <v-container
                            align="center"
                            justify="center"
                            >
                                <v-col>
                                    <v-btn
                                    block
                                    @click="goToGitHub()"
                                    >
                                        <v-icon
                                        light
                                        class="pr-2"
                                        >
                                        mdi-xml</v-icon>
                                    Github
                                    </v-btn>
                                </v-col>

                                <v-col>
                                    <v-btn
                                    block
                                    color="rgba(17, 205, 239, 1)"
                                    @click="goToLinkedIn()"
                                    >
                                        <v-icon
                                        light
                                        class="pr-2"
                                        >
                                        mdi-account</v-icon>
                                    LinkedIn
                                    </v-btn>
                                </v-col>

                            </v-container>
                        </v-row>
                    </div>
                </v-row>

            </v-container>

        </v-card>
    </v-app>
</template>

<script>
export default {
    name: 'App',
    data: () => ({
        //
    }),
    methods: {
        goToGitHub() {
            window.open("https://github.com/ArtiomInc")
        },
        goToLinkedIn() {
            window.open("https://www.linkedin.com/in/artiom-duc-914922186")
        },
    },
};
</script>

<style>
    #bg {
        background-image: url(../src/assets/background.jpg);
        background-size: cover;
        background-position: center;
    }
</style>