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
                            <p id="myname" class="white--text">artiom</p>
                        </v-row>

                        <v-row
                        align="center"
                        justify="center"
                        class="mb-10"
                        >
                            <p
                            align="center"
                            id="description"
                            class="white--text mx-10"
                            >My personal website to explore ideas and technologies</p>
                        </v-row>

                        <v-row
                        align="center"
                        justify="center"
                        class="px-10"
                        >
                            <v-col>
                                <v-btn
                                block
                                class="pa-5"
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
                                class="white--text pa-5"
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
    #myname {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 400%;
        font-weight: 900;
    }
    #description {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 200%;
        font-weight: 200;
    }
</style>