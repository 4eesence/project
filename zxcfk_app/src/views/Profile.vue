<template>
  <v-container>
    <v-row justify="center">
        <v-card>
          <v-card-text>
            <v-avatar size="150">
              <img src="https://photo8.wambacdn.net/92/07/84/1793487029/2104907226_square_small.jpg?hash=CSpHxzhs4FCP3EdAvaORcQ&expires=64060578000&updated=1644395230" alt="Avatar">
            </v-avatar>
            <h2 class="profile-name">{{ profile.name }}</h2>
            <p class="profile-username">{{ profile.username }}</p>
            <p class="profile-bio">{{ profile.bio }}</p>
            <div class="profile-info">
              <v-row>
                <v-col>
                  <p>Followers:</p> {{ profile.followers }}
                </v-col>
                <v-col>
                  <p>Following:</p> {{ profile.following }}
                </v-col>
              </v-row>
            </div>
            <v-divider></v-divider>
            <v-list>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title>phone: {{ profile.phone }}(hidden)</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title>mail: {{ profile.email }}</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card-text>
        </v-card>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      profile: {
        name: 'Zxcursed Denisovich',
        bio: 'SF MID 1X1',
        followers: '100000000000000000',
        following: '993',
        phone: '1000-7',
        email: 'zxcursed@mail.ru'
      }
    }
  }
}
</script>

<style scoped>
.profile-name {
  font-size: 24px;
  margin-top: 10px;
}

.profile-username {
  color: grey;
  margin-top: -10px;
}

.profile-bio {
  margin-top: 10px;
}

.profile-info {
  margin-top: 20px;
}

.profile-info strong {
  margin-right: 5px;
}
</style>
