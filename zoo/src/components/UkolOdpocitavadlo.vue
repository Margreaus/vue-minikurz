<script setup>

import {ref} from "vue"


const pocet = ref(10);


setInterval(() => {
    //kdykoliv budeme chtit cist nebo menit hodnotu reactivni promenne, tak musime jit pres vlasntost value
    pocet.value = Math.floor(Math.random() * 10000);
}, 2000);

</script>