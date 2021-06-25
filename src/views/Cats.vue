<template>
    <div>
        <h1>Cats for adoption</h1>
        <!-- <b-table striped hover :items="cats">
            <template #cell(name)="data">
                <router-link
                    :to="`/pets/${data.index}`"
                >
                    {{ data.value }}
                </router-link>
            </template>
        </b-table> -->
        <li v-for="(item ,index) in arr" :key="index">
            {{item}}
        </li>
    </div>
</template>

<script>
import cats from '../data/cats'
export default {
    data() {
        return {
            cats,
            arr: { 
                one: "one", 
                two: "two",
                three: "three"
            }
        }
    },
}
</script>