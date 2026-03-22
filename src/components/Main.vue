<script setup>
import {ref} from 'vue'
const preambleHeader = ref('Preamble')
const nationalTerrHeader = ref('National Territory')
const statePolHeader = ref('Declaration of Priciples and State Policies Principles')
const count = ref(0);
</script>

<template>
    <main>
        <section>
            <button @click="count++">
                {{ count }}
            </button>
            <h2>
                {{ preambleHeader }}
            </h2>
            <p>
                We, the sovereign Filipino people, imploring the aid of Almighty God, in order to build a just and humane society, and establish a Government 
                that shall embody our ideals and aspirations, promote the common good, conserve and develop our patrimony, and secure to ourselves and our 
                posterity, the blessings of independence and democracy under the rule of law and a regime of truth, justice, freedom, love, equality, and peace, 
                do ordain and promulgate this Constitution.
            </p>
        </section>
        <section>
            <h2>
                ARTICLE I
            </h2>
            <h2>
                {{ nationalTerrHeader }}
            </h2>
            <p>
                The national territory comprises the Philippine archipelago, with all the islands and waters embraced therein, and all other territories over which 
                the Philippines has sovereignty or jurisdiction, consisting of its terrestrial, fluvial and aerial domains, including its territorial sea, the seabed, 
                the subsoil, the insular shelves, and other submarine areas. The waters around, between, and connecting the islands of the archipelago, regardless of their 
                breadth and dimensions, form part of the internal waters of the Philippines.
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
}
</style>