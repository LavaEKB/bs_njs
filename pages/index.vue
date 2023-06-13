<div>
  <h1>Получение информации из Sales</h1>
  <div v-for="sale in sales" :key="sale.slug" class="blog">
    <div class="blog-title">{{ sale.ntab }}</div>
  </div>
</div>
</template>

<script>
import axios from "axios";
export default {
  async asyncData(ctx) {
    const { data } = await axios.get(`http://localhost:8000/api/sales/`);
    console.log(data)
    return {
      sales: data.results,
    }
  }
}
</script>

<style>

</style>