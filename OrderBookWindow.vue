<template>
    <v-form>
        <v-container>
            <v-row>

                <v-col cols="12" sm="6" md="3">
                    <v-text-field
                            label="ISBN"
                            v-model="bookName"
                    ></v-text-field>
                </v-col>

                <v-col cols="12" sm="6" md="3">
                    <v-text-field
                            label="Name Of Book"
                            v-model="isbn"
                    ></v-text-field>
                </v-col>

                <v-col cols="12" sm="6" md="5">
                    <v-btn @click="orderBook()">OrderBook</v-btn>
                </v-col>


            </v-row>
        </v-container>
    </v-form>
</template>


return: {},
<script>
    export default {
        name: "OrderBookWindow",
        data: {
            bookName: '',
            isbn: ''
        },
        methods: {
            orderBook() {
                console.log("Book Ordered")
                console.log(this.bookName)
                console.log(this.isbn)
            }
        }
    }
</script>

<style scoped>

</style>