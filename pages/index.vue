/<template>
  <v-container>
    <div>
      <post-card />
      <post-card />
      <post-card />
      <post-card />
      <post-card />
    </div>
  </v-container>
</template>

<script>
import PostCard from '~/components/PostCard.vue'
export default {
  components: { PostCard },
  head () {
    return {
      title: '메인 페이지'
    }
  }
}
</script>

<style>

</style>
