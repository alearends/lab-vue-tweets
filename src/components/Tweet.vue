<template>
  <div className="tweet">
    <img
      :src="imageT"
      className="profile"
      alt="profile"
    />

    <div className="body">
      <div className="top">
        <span className="user">
          <span className="name">{{nameT}}</span>
          <!-- <span className="name">Ironhack</span> -->
          <span className="handle">@{{handleT}}</span>
          <!-- <span className="handle">@ironhack</span> -->
        </span>

        <span className="timestamp">{{timestampT}}</span>
        <!-- <span className="timestamp">Nov 30, 2020</span> -->
      </div>

      <p className="message">{{messageT}}</p>
      <!-- <p className="message">
        On December 7th, we will be hosting a #webinar that will introduce you
        to #SQL! Are you ready? 🚀
      </p> -->

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
  const props =defineProps(['nameT', 'imageT', 'handleT', 'timestampT', 'messageT']);
</script>

<style scoped>
a {
  color: #42b983;
}
</style>

