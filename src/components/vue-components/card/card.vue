<template>
    <v-app>
      <h5 class="mt-0">Simple cards</h5>
      <div class="row">
        <div class="col-md-6">
          <card :title="'Simple card'">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente. Ad architecto at aut
              et ex facilis fuga, laboriosam, magnam modi obcaecati officia officiis, omnis praesentium quam quas reiciendis
              rerum ullam velit veritatis vitae.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card>
            <h5 class="mt-0">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h5>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente. Ad architecto at aut
              et ex facilis fuga, laboriosam, magnam modi obcaecati officia officiis, omnis praesentium quam quas reiciendis
              rerum ullam velit veritatis vitae.</p>
          </card>
        </div>
      </div>

      <h5>Colored cards</h5>
      <div class="row">
        <div class="col-md-6">
          <card>
            <p><strong>Standard color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'success'">
            <p><strong>Success color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'info'">
            <p><strong>Info color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'warning'">
            <p><strong>Warning color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'danger'">
            <p><strong>Danger color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :customBgColor="'#9b479f'" :color="'#ccc'" :customColor="'#ccc'">
            <p><strong>Custom color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
      </div>

      <h5>Outline cards</h5>
      <div class="row">
        <div class="col-md-6">
          <card :outline="true">
            <p><strong>Standard color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'success'" :color="'success'" :outline="true">
            <p><strong>Success color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'info'" :color="'info'" :outline="true">
            <p><strong>Info color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'warning'" :color="'warning'" :outline="true">
            <p><strong>Warning color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :bgColor="'danger'" :color="'danger'" :outline="true">
            <p><strong>Danger color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :customBgColor="'#9b479f'" :customColor="'#9b479f'" :color="'#9b479f'" :outline="true">
            <p><strong>Custom color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
      </div>

      <h5>Image background cards</h5>
      <div class="row">
        <div class="col-md-6">
          <card :customBgColor="'rgba(0,128,0,0.7)'" :customColor="'#fff'" :bgImage="'/static/content/card-2.jpg'" :color="'white'">
            <p><strong>Image background</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. A adipisci assumenda at aut autem cupiditate
              dolorum ducimus eaque earum eveniet facere magni neque numquam odit, optio quas quod vel voluptatem?</p>
          </card>
        </div>
        <div class="col-md-6">
          <card :customBgColor="'rgba(220,20,60,0.6)'" :customColor="'#fff'" :bgImage="'/static/content/card-3.jpg'" :color="'white'">
            <p>Consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
            <ul>
              <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi!</li>
              <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus assumenda illum quae.</li>
              <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</li>
            </ul>
          </card>
        </div>
      </div>

      <h5>Align cards</h5>
      <div class="row">
        <div class="col-lg-4">
          <card :align="'left'" class="mb-lg-0">
            <p><strong>Standard color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-lg-4">
          <card :bgColor="'success'" :align="'center'" class="mb-lg-0">
            <p><strong>Success color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
        <div class="col-lg-4">
          <card :bgColor="'info'" :align="'right'" class="mb-0">
            <p><strong>Info color</strong>, consectetur adipisicing elit. Consequatur dolor ducimus est excepturi illo itaque
              modi quis repudiandae totam vitae. Accusamus beatae consectetur dolorum pariatur sapiente.</p>
          </card>
        </div>
      </div>

    </v-app>
</template>

<script>
import card from '../../card/card'
export default {
  name: 'card-body',
  components: {
    card
  }
}
</script>

<style scoped>

</style>
