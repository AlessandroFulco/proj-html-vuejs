<template>
  <div id="app">
    
    <!-- header -->
      <!-- logo -->
      <!-- nav-link -->
    <MyHeader/>
  


      
        
        
    <!-- main -->
    <main>

      <!-- jumbo -->
      <div class="jumbo">
        <img src="./assets/images/video_law_home_preview.jpg" alt="Home Preview">
      </div>

      <!-- sez -->
        <!-- comp. x3 -->
      <div class="info objective">
        <section>
          <h2>
            WHO WE ARE
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>
          <div class="btn">
            LEARN MORE
          </div>
        </section>

        <section>
          <h2>
            WHO WE DO
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>
          <div class="btn">
            LEARN MORE
          </div>
        </section>

        <section>
          <h2>
            WHO WE WORK
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>
          <div class="btn">
            LEARN MORE
          </div>
        </section>
      </div>

      <!-- comp. x4 -->
      <div class="info rules">
        <section>
          <h1>=</h1>
          <h2>
            WHO WE ARE
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>

        </section>

        <section>
          <h1>=</h1>
          <h2>
            WHO WE DO
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>

        </section>

        <section>
          <h1>=</h1>
          <h2>
            WHO WE WORK
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>

        </section>

        <section>
          <h1>=</h1>
          <h2>
            WHO WE WORK
          </h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius animi ea repudiandae expedita rerum. Lorem ipsum dolor sit amet.
          </p>

        </section>
      </div>



    </main>

      <!-- /sez -->

      <!-- ask -->

      <!-- sez -->
        <!-- comp. x18 -->
      <!-- /sez -->

      <!-- cit. -->

      <!-- sez -->
        <!-- comp. x3 -->
      <!-- /sez -->

      <!-- Enquiry -->

    <!-- footer -->
    
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
  }
}
</script>

<style lang="scss">
$bg-sez: #f5f5f5;
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Helvetica, Arial, sans-serif;
  color: #000;

  main {
    .info {
      text-align: center;
    }

    .jumbo {

      section {
        display: flex;
        align-items: center;
        height: 20px;
        width: 70%;
        margin: 0 auto;
      }
      img {
        height: 600px;
        width: 100%;
        object-fit: cover;
        object-position: top;
      }
    }

    .info.objective {
      background-color: $bg-sez;
      display: flex;
      justify-content: center;
      padding: 70px;

      section {
        flex-basis: calc(70% / 3);  
        padding: 10px;
        background-color: #fff;
      }
    }
    .info.rules {
      border-top: 2px solid #eee;
      background-color: #fff;
      display: flex;
      justify-content: center;
      padding: 70px;
      section {
        flex-basis: calc(70% / 4);
      }
    }
  }
}
</style>
