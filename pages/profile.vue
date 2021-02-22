<template>
    <div>
        <v-container>
            <v-card style="margin-bottom: 20px">
                <v-container>
                    <v-subheader>내 프로필</v-subheader>
                </v-container>
            </v-card>
            <v-form>
                <v-text-field label="닉네임" required />
                <v-btn color="blue" type="submit">수정</v-btn>
            </v-form>
        </v-container>
        <v-card style="margin-bottom: 20px">
            <v-container>
                <v-subheader>팔로잉</v-subheader>
                <follow-list />
            </v-container>
        </v-card>
        <v-card style="margin-bottom: 20px">
            <v-container>
                <v-subheader>팔로워</v-subheader>
                <follow-list />
            </v-container>
        </v-card>
    </div>
</template>
<script>
import FollowList from '~/components/FollowList'
export default {
//   layout: 'admin',
  components: {
    FollowList
  },
  head () {
    return {
      title: '프로파일'
    }
  }
}
</script>
<style>

</style>
