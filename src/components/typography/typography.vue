<template>
    <v-app>
      <card :title="'Headers'">
        <p>All HTML headings, <code>&lt;h1&gt;</code> through <code>&lt;h6&gt;</code> are available. <code>.h1</code> through <code>.h6</code> classes are also available, for when you want to match the font styling of a heading but cannot use the associated HTML element.</p>
        <div class="row">
          <div class="col-md-6">
            <h1>Heading 1</h1>
            <h2>Heading 2</h2>
            <h3>Heading 3</h3>
            <h4>Heading 4</h4>
            <h5>Heading 5</h5>
            <h6>Heading 6</h6>
          </div>
          <div class="col-md-6">
            <h1 class="text-uppercase">Heading 1</h1>
            <h2 class="text-uppercase">Heading 2</h2>
            <h3 class="text-uppercase">Heading 3</h3>
            <h4 class="text-uppercase">Heading 4</h4>
            <h5 class="text-uppercase">Heading 5</h5>
            <h6 class="text-uppercase">Heading 6</h6>
          </div>
        </div>
      </card>

      <card :title="'Text style'">
        <p><code>.mark</code> and <code>.small</code> classes are also available to apply the same styles as <code>&lt;mark&gt;</code> and <code>&lt;small&gt;</code> while avoiding any unwanted semantic implications that the tags would bring.</p>
        <p>You can use the mark tag to <mark>highlight</mark> text.</p>
        <p><del>This line of text is meant to be treated as deleted text.</del></p>
        <p><s>This line of text is meant to be treated as no longer accurate.</s></p>
        <p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
        <p><u>This line of text will render as underlined</u></p>
        <p><small>This line of text is meant to be treated as fine print.</small></p>
        <p><strong>This line rendered as bold text.</strong></p>
        <p><em>This line rendered as italicized text.</em></p>
      </card>

      <card :title="'Blockquotes'">
        <p>For quoting blocks of content from another source within your document. Wrap <code>&lt;blockquote class="blockquote"&gt;</code> around any <abbr title="HyperText Markup Language">HTML</abbr> as the quote.</p>
        <blockquote class="blockquote">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
          <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
        </blockquote>

        <blockquote class="blockquote blockquote-reverse">
          <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
          <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
        </blockquote>
      </card>

      <card :title="'Lists'">
        <div class="row">
          <div class="col-md-6">
            <ul>
              <li>Lorem ipsum dolor sit amet</li>
              <li>Consectetur adipiscing elit</li>
              <li>Integer molestie lorem at massa</li>
              <li>Facilisis in pretium nisl aliquet</li>
              <li>Nulla volutpat aliquam velit
                <ul>
                  <li>Phasellus iaculis neque</li>
                  <li>Purus sodales ultricies</li>
                  <li>Vestibulum laoreet porttitor sem</li>
                  <li>Ac tristique libero volutpat at</li>
                </ul>
              </li>
              <li>Faucibus porta lacus fringilla vel</li>
              <li>Aenean sit amet erat nunc</li>
              <li>Eget porttitor lorem</li>
            </ul>
          </div>
          <div class="col-md-6">
            <ol>
              <li>Lorem ipsum dolor sit amet</li>
              <li>Consectetur adipiscing elit</li>
              <li>Integer molestie lorem at massa</li>
              <li>Facilisis in pretium nisl aliquet</li>
              <li>Nulla volutpat aliquam velit
                <ol>
                  <li>Phasellus iaculis neque</li>
                  <li>Purus sodales ultricies</li>
                  <li>Vestibulum laoreet porttitor sem</li>
                  <li>Ac tristique libero volutpat at</li>
                </ol>
              </li>
              <li>Faucibus porta lacus fringilla vel</li>
              <li>Aenean sit amet erat nunc</li>
              <li>Eget porttitor lorem</li>
            </ol>
          </div>
        </div>
      </card>

      <card :title="'Text alignment'">
        <p>Easily realign text to components with text alignment classes.</p>
        <p class="text-left">Left aligned text on all viewport sizes.</p>
        <p class="text-center">Center aligned text on all viewport sizes.</p>
        <p class="text-right">Right aligned text on all viewport sizes.</p>
      </card>

      <card :title="'Text transform'" class="mb-0">
        <p>Transform text in components with text capitalization classes.</p>
        <p class="text-lowercase">Lowercased text.</p>
        <p class="text-uppercase">Uppercased text.</p>
        <p class="text-capitalize">CapiTaliZed text.</p>
      </card>
    </v-app>
</template>

<script>
import card from '../card/card'
export default {
  name: 'typography',
  components: {
    card
  }
}
</script>

<style scoped>

</style>
