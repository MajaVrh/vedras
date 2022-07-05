<template>
  <div class="container">
    <div class="ImgSpace">
      <img class="userImg" :src="user.picture" alt="" />
    </div>
    <div class="info">
      <div class="userTitle">{{ user.title }}</div>
      <div class="firstName">{{ user.firstName }}</div>
      <div class="lastName">{{ user.lastName }}</div>
    </div>

    <NuxtLink :to="`user/${user.id}`">
      <button style="width: 60%" class="buttonMore">Show more</button>
    </NuxtLink>
  </div>
</template>

<script>
export default {
  props: ["user"],
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Titillium+Web:ital,wght@0,200;0,300;0,400;0,600;0,700;0,900;1,200;1,300;1,400;1,600;1,700&display=swap");
body {
  font-family: "Titillium Web", sans-serif;
}
.container {
  width: 14rem;

  box-shadow: 0 2px 32px 0 rgba(0, 0, 0, 0.226);
  font-size: 16px;
  height: 18rem;
}
.info {
  gap: 0.3rem;
  display: flex;
  flex-direction: row;
  font-size: 20px;

  width: 100%;
  justify-content: center;
}
.userImg {
  width: 60%;
  border-radius: 100%;
  min-height: 60% !important;
  max-height: 60% !important;
  margin-bottom: 10%;
}
.buttonMore {
  color: white;
  background-color: #027fc1;
  border: #027fc1;
  cursor: pointer;
  padding: 0.5rem 1rem;
  font-family: "Titillium Web", sans-serif;
  margin: 5% 20% 20% 20%;

  font-size: 16px;
}

.buttonMore:hover {
  background-color: #fff;
  color: #027fc1;
  border: 1.5px solid #027fc1;
  cursor: pointer;
}
.ImgSpace {
  width: 100%;
  display: flex;
  margin-top: 10%;
  justify-content: center;
}
</style>
