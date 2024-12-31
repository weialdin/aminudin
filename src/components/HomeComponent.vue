<template>
  <div class="dizme_tm_section" id="home">
    <div class="dizme_tm_hero">
      <div
        class="background"
        :data-img-url="`/img/slider/${dark ? 2 : 1}.jpg`"
      ></div>
      <div class="container">
        <div class="content">
          <div class="details">
            <div class="hello">
              <h3 class="orangeText">Hello, I'm</h3>
            </div>
            <div class="name">
              <h3>Ahmad Aminudin</h3>
            </div>
            <div class="job">
              <p>
                A <span class="greenText">Fullstack Web Developer</span> From
                <span class="purpleText">Mojokerto</span>
              </p>
            </div>
            <div class="text">
              <p>
                I'm a full-stack web developer with expertise in Laravel and
                Vue.js, based in Mojokerto. I have 6 months of experience in
                full-stack web development, and I'm very passionate about coding
                and building web applications. Additionally, I have intermediate
                skills in Flutter and enjoy working on mobile development
                projects.
              </p>
            </div>
            <div class="button">
              <div class="dizme_tm_button">
                <a class="anchor" href="#about"><span>About Me</span></a>
              </div>
              <div class="social">
                <ul>
                  <li>
                    <a href="https://github.com/weialdin"
                      ><i class="icon-github-3"></i
                    ></a>
                  </li>
                  <li>
                    <a href="https://www.youtube.com/@weialdin"
                      ><i class="icon-youtube-1"></i
                    ></a>
                  </li>
                  <li>
                    <a href="https://www.linkedin.com/in/weialdin/"
                      ><i class="icon-linkedin-1"></i
                    ></a>
                  </li>
                  <li>
                    <a href="https://www.instagram.com/weialdin/"
                      ><i class="icon-instagram-1"></i
                    ></a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="avatar">
            <div class="image">
              <img src="require('@/public/img/slider/pic.png')" alt="" />
              <span
                class="skills illustrator anim_moveBottom"
                v-html="laravel"
              ></span>
              <span
                class="skills photoshop anim_moveBottom"
                v-html="vue"
              ></span>
              <span
                class="skills figma anim_moveBottom"
                v-html="flutter"
              ></span>
            </div>
          </div>
        </div>
      </div>
      <div class="dizme_tm_down">
        <a class="anchor" href="#process" v-html="dark ? mouseDark : mouse">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import { flutter, laravel, vue, mouse, mouseDark } from "../svg";
export default {
  name: "HomeComponent",
  data() {
    return { flutter, laravel, vue, mouse, mouseDark };
  },
  props: {
    dark: { type: Boolean },
  },
};
</script>
