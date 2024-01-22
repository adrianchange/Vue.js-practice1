<template>
    <div>
       <ul>
        <li v-for="country in countries" :key="country.code">{{ country.name }}</li>
       </ul>
    </div>

</template>

<script setup>
import {ref} from 'vue';
let countries = ref([
    { code: 'es',
      name: 'Spain'

    },
    { code: 'en',
      name: 'UK'

    },
    { code: 'fr',
      name: 'France'

    },
    { code: 'pt',
      name: 'Portugal'

    }
])
</script>

<style scoped></style>