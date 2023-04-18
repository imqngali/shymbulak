<template>
  <Home :currentData="currentData"/>
</template>


<script>
import Home from './components/Home.vue'
import axios from 'axios'

export default {
  name: 'App',
  components: {
    Home
  },
  data() {
        return {
            currentData: null
        }
	},
	
	async mounted() {

    await axios.get('https://api.openweathermap.org/data/2.5/weather?id=1526384&appid=d1ab15d09fb14e54ddf28068bd85b748')
                .then(response => {
                    this.currentData = response.data;
                })
                .catch(function() {
                     
            });
		
	}
}

</script>

<style lang="css">
  @import 'assets/style.min.css';
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap');
</style>
