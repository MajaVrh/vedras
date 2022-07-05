<template>
  <div class="padding">
    <div class="userList">
      <div class="blueCard">
        <div style="padding: 10%">
          <H1>User list</H1>
          <div class="text">
            Here you can see a list of all users. Click on <i>Show more </i> to
            see their profile.
          </div>
        </div>
      </div>
      <user-card
        class="card"
        v-for="user in users"
        :key="user.id"
        :user="user"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [],
    };
  },

  methods: {
    async getUsers() {
      const getData = await this.$axios.$get(
        "https://dummyapi.io/data/v1/user",
        {
          headers: {
            "app-id": "62c2fa6ba27be94b5a0d48d1",
            "Access-Control-Allow-Origin": "*",
          },
        }
      );
      this.users = getData.data;
      console.log(this.users);
    },
  },
  mounted() {
    this.getUsers();
  },
};
</script>

<style>
* {
  margin: 0;
}
.padding {
  display: flex;
  justify-content: center;
  padding: 4rem 10%;
}
.userList {
  display: grid;
  gap: 50px;
  grid-template-columns: repeat(4, 1fr);
}

.blueCard {
  width: 14rem;

  height: 100%;
  background-color: #027fc1;
  color: white;
  display: flex;

  flex-direction: column;
}

.text {
  font-size: 20px;
}

@media (max-width: 1200px) {
  .userList {
    grid-template-columns: repeat(3, 1fr);
  }
}
@media (max-width: 900px) {
  .userList {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 560px) {
  .userList {
    grid-template-columns: repeat(1, 1fr);
    width: 100%;
    padding: 0;
    display: flex;
    flex-direction: column;

    align-items: center;
  }
  .padding {
    padding: 0;
  }
  .blueCard {
    width: 100%;
  }
}
</style>
