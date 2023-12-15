<template>
  <div class="bio-content">
    <div class="bio-card bg-background-secondary justify-around rounded-lg shadow-xl">
      <div class="firstinfo flex flex-col justify-center my-4 sm:flex-row">
        <Logo />
        <div class="profileinfo mb-4 sm:mb-0 flex flex-col justify-center">
          <h3 class="text-copy-primary hover:text-gray-600 text-center sm:text-left">Darren Odden</h3>
          <h5 class="text-center sm:text-left">Charismatic Codefauna</h5>
          <p class="bio font-normal text-xs py-3 text-center sm:text-left">
            Developer, designer, and father.<br/>
            User focused development and design.
          </p>
        </div>
      </div>
    </div>
<!--    <ul class="badgescard bg-background-tertiary flex-wrap justify-center py-2 rounded-b-lg shadow-lg">-->
<!--      <li title="PHP">-->
<!--        <font-awesome-icon :icon="['fab','php']" />-->
<!--      </li>-->
<!--      <li title="Javascript">-->
<!--        <font-awesome-icon :icon="['fab','js']" />-->
<!--      </li>-->
<!--      <li title="VueJS">-->
<!--        <font-awesome-icon :icon="['fab','vuejs']" />-->
<!--      </li>-->
<!--      <li title="Java">-->
<!--        <font-awesome-icon :icon="['fab','java']" />-->
<!--      </li>-->
<!--      <li title="WordPress">-->
<!--        <font-awesome-icon :icon="['fab','wordpress']" />-->
<!--      </li>-->
<!--      <li title="SquareSpace">-->
<!--        <font-awesome-icon :icon="['fab','squarespace']" />-->
<!--      </li>-->
<!--      <li title="Shopify">-->
<!--        <font-awesome-icon :icon="['fab','shopify']" />-->
<!--      </li>-->
<!--      <li title="HubSpot">-->
<!--        <font-awesome-icon :icon="['fab','hubspot']" />-->
<!--      </li>-->
<!--      <li title="Wine Developer">-->
<!--        <font-awesome-icon :icon="['fad','wine-glass']" />-->
<!--      </li>-->
<!--    </ul>-->
  </div>
</template>
<script setup lang="ts">
</script>

<style>
.bio-content {
  position: relative;
  animation: animatop 0.9s cubic-bezier(0.425, 1.14, 0.47, 1.125) forwards;
  height: 153px;
}

.bio-card {
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.2);
  position: relative;
  overflow: hidden;
}
.bio-card h5 {
  color: #x`;
}
.content-wrapper:not(.theme-light) .bio-card h5 {
  color: #8094b4;
}

.badgescard {
  display: flex;
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.2);
  position: absolute;
  left: 10px;
  bottom: -3px;
  width: calc(100% - 20px);
  animation: animainfos 0.5s cubic-bezier(0.425, 1.04, 0.47, 1.105) 0.75s forwards;
  list-style: none;
  z-index: -1;
}

ul.badgescard {
  margin: 0
}

.badgescard span,
.badgescard li {
  font-size: 1.4em;
  margin: 0px 6px;
}

.bg-background-secondary {
  background-color: hsla(204, 45%, 98%, 90%);
}

.bg-background-tertiary {
  background-color: hsla(214, 32%, 91%, 85%);
}

.firstinfo {
  display: block;
  flex-direction: row;
  z-index: 2;
  position: relative;
}

.firstinfo img {
  border-radius: 50%;
  box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.2);
}

.firstinfo .profileinfo {
  padding: 0px 20px;
}

.firstinfo .profileinfo h1 {
  /*font-size: 1.8em;*/
}

.firstinfo .profileinfo h3 {
  /*font-size: 1.2em;*/
  /*color: #002868;*/
  font-style: italic;
}

.firstinfo .profileinfo p.bio {
  /*padding: 10px 0px;*/
  /*color: #3c3c3c;*/
  line-height: 1.2;
  font-size: .7em;
  font-style: initial;
}

@keyframes animatop {
  0% {
    opacity: 0;
    bottom: -550px;
  }

  100% {
    opacity: 1;
    bottom: 0px;
  }
}

@keyframes animainfos {
  0% {
    bottom: 10px;
  }

  100% {
    bottom: -54px;
  }
}

@keyframes rotatemagic {
  0% {
    opacity: 0;
    transform: rotate(0deg);
    top: -24px;
    left: -253px;
  }

  100% {
    transform: rotate(-30deg);
    top: -24px;
    left: -78px;
  }
}
</style>
