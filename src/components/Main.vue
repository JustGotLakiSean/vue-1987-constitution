<script setup>
import {ref} from 'vue'
const preambleHeader = ref('Preamble')
const nationalTerrHeader = ref('National Territory')
const statePolHeader = ref('Declaration of Priciples and State Policies Principles')
const count = ref(0);
const href = ref('https://lawphil.net/')
const isButtonDisabled = ref(true)
import lawImage from '@/assets/images/law.png'

// wrap array of objects inside the ref to make it reactive
const facts = ref([
    { "constitutionTitle": "Preamble", "constitutionContent": "We, the sovereign Filipino people, imploring the aid of Almighty God, in order to build a just and humane society"},
    { "constitutionTitle": "National Teritorry", "constitutionContent": "The national territory comprises" },
    { "constitutionTitle": "Article II", "constitutionContent": "Section 1" }
])
</script>

<template>
    <main>
        <section>
            <!-- absolute path to /public folder -->
            <!-- <img src="/images/law_image.jpg" alt="" /> -->
            
            <!-- relative path to /assets folder -->
            <!-- <img src="@/assets/images/law.png" alt="" /> -->

            <!-- import asset or bind an image to the src attr -->
            <!-- <img v-bind:src="lawImage" alt /> -->
            <button v-bind:disabled="isButtonDisabled" @click="count++">
                {{ count }}
            </button>
            <!-- :href for shorthand for v-bind:attr-->
            <!-- only :href if the same name as the attr-->
            <a v-bind:href="href">Lawphil</a>
            <h2>
                {{ facts[0].constitutionTitle }}
            </h2>
            <p>
                {{ facts[0].constitutionContent }}
            </p>
        </section>
        <section>
            <h2>
                ARTICLE I
            </h2>
            <h2>
                {{ facts[1].constitutionTitle }}
            </h2>
            <p>
                {{ facts[1].constitutionContent }}
            </p>
        </section>
        <section>
            <h2>
                ARTICLE II
            </h2>
            <h2>
                {{ statePolHeader }}
            </h2>
            <p>
                <span class="section_ii">Section 1.</span> The Philippines is a democratic and republican State. Sovereignty resides in the people and all government authority emanates from them.
            </p>
            <p>
                <span class="section_ii">Section 2.</span> The Philippines renounces war as an instrument of national policy, adopts the generally accepted principles of international law as part of the law of the land and adheres to the policy of peace, equality, justice, freedom, cooperation, and amity with all nations.
            </p>
            <p>
                <span class="section_ii">Section 3.</span> Civilian authority is, at all times, supreme over the military. The Armed Forces of the Philippines is the protector of the people and the State. Its goal is to secure the sovereignty of the State and the integrity of the national territory.
            </p>
            <p>
                <span class="section_ii">Section 4.</span> The prime duty of the Government is to serve and protect the people. The Government may call upon the people to defend the State and, in the fulfillment thereof, all citizens may be required, under conditions provided by law, to render personal, military or civil service.
            </p>
            <p>
                <span class="section_ii">Section 5.</span> The maintenance of peace and order, the protection of life, liberty, and property, and promotion of the general welfare are essential for the enjoyment by all the people of the blessings of democracy.
            </p>
            <p>
                <span class="section_ii">Section 6.</span> The separation of Church and State shall be inviolable.
            </p>
        </section>
    </main>
</template>

<style scoped>
/*MAIN CSS*/
main {
  margin-top: 15px;
}

section {
  margin-top: 25px;
}

h2 {
  font-size: 1.3rem;
  color: #34495e;
  margin-bottom: 3px;
}

p {
    font-size: 0.9rem;
    color: #555;
    text-align: justify;
    line-height: 1.5;
    margin-bottom: 16px;
}

button:hover {
    transform: scale(1.05);
}

button:disabled {
    background: grey;
    cursor: not-allowed;
    opacity: 0.5;
}
</style>