<template>
  <div class="poravnanja">
    <div v-if="userInfo" class="container">
      <div class="cardTitle">
        {{ userInfo.title }} {{ userInfo.firstName }} {{ userInfo.lastName }}
      </div>

      <div class="grid">
        <div class="col-1">
          <img class="userImg" :src="userInfo.picture" alt="" />
        </div>
        <div class="col-2">
          <div>
            <b>Date of birth:</b>
            {{ new Date(userInfo.dateOfBirth).getDate() }}.{{
              new Date(userInfo.dateOfBirth).getMonth() + 1
            }}.{{ new Date(userInfo.dateOfBirth).getFullYear() }}.
          </div>

          <div><b>Gender:</b> {{ userInfo.gender }}</div>
          <div><b>Email:</b> {{ userInfo.email }}</div>
          <div><b>Phone: </b>{{ userInfo.phone }}</div>
          <div>
            <b>Location: </b> {{ userInfo.location.city }},
            {{ userInfo.location.street }}, {{ userInfo.location.state }},
            {{ userInfo.location.country }}
          </div>
          <div>
            <b>Register date: </b>
            {{ new Date(userInfo.registerDate).getDate() }}.{{
              new Date(userInfo.registerDate).getMonth() + 1
            }}.{{ new Date(userInfo.registerDate).getFullYear() }}.
          </div>
          <div>
            <b>Updated date: </b>
            {{ new Date(userInfo.updatedDate).getDate() }}.{{
              new Date(userInfo.updatedDate).getMonth() + 1
            }}.{{ new Date(userInfo.updatedDate).getFullYear() }}.
          </div>
        </div>
        <div class="col-3">
          <NuxtLink to="/user">
            <button class="buttonMore">Return</button>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "currentUser",

  data() {
    return {
      userInfo: null,
    };
  },
  methods: {
    async userData() {
      const user = await this.$axios.$get(
        `https://dummyapi.io/data/v1/user/${this.$route.params.user}`,
        {
          headers: {
            "app-id": "62c2fa6ba27be94b5a0d48d1",
            "Access-Control-Allow-Origin": "*",
          },
        }
      );
      this.userInfo = user;

      console.log(this.userInfo);
    },
  },
  mounted() {
    this.userData();
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
.container {
  padding: 3rem 6rem;
  width: 35rem;
  color: #5c5c5c;
}

.grid {
  display: grid;
  grid-template-columns: (30% 60% 10%);
  justify-content: center;
}
.cardTitle {
  color: #027fc1;
  font-size: 36px;
  font-weight: bold;
}

.userImg {
  width: 8rem;
  border-radius: 100%;
  min-height: 8rem !important;
  max-height: 8rem !important;
}
.col-1 {
  display: flex;
  align-items: center;
}
.col-2 {
  gap: 0.2rem;
  margin: 0 -4rem 0 2rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}
.col-3 {
  display: flex;
  align-items: flex-end;
}
.grid {
  width: 100%;
  display: flex;
  flex-direction: row;
}
.buttonMore {
  height: 2rem;
  width: 8rem;
}
.buttonMore:hover {
  background-color: #fff;
  color: #027fc1;
  border: 1.5px solid #027fc1;
  cursor: pointer;
}

.poravnanja {
  width: 100%;
  height: 100vh !important;
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  align-self: center;
}

@media (max-width: 900px) {
  .grid {
    display: flex;
    margin: 0 !important;
    flex-direction: column;
    justify-content: center;
  }
  .container {
    height: auto;
    width: 50% !important;
    margin: 0;
  }
  .col-2 {
    justify-content: center;
    margin: 1rem 0;
  }
  .col-3 {
    justify-content: center;
    margin-top: 1rem;
    margin-bottom: 1rem;
  }
  .col-1 {
    justify-content: center;
    margin-top: 1rem;
    margin-bottom: 1rem;
  }
  .cardTitle {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
@media (max-width: 650px) {
  .container {
    padding: 3rem 4rem;
    width: 90%;
    height: 90%;
  }
  .poravnanja {
    width: 100%;
  }
  .cardTitle {
    font-size: 24px;
    margin: auto;
    min-width: 100%;
    white-space: nowrap;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
@media (min-width: 1920px) {
  .grid {
    font-size: 22px;
  }
  .buttonMore {
    font-size: 25px;
    height: 3rem;
    width: 8rem;
  }
  .userImg {
    min-width: 12rem;
    min-height: 12rem !important;
    object-fit: contain;
    margin-right: 1rem;
  }
  .container {
    width: auto;
    height: auto;
  }
  .cardTitle {
    margin-bottom: 1rem;
  }
}
</style>
