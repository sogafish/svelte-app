<script lang="ts">
  import Header from './components/Header.svelte';
  import Counter from './components/Counter.svelte';
  import Button from './components/Button.svelte';

  let count = 0;

  const incrementCount = () => {
    count += 1;
  };
</script>

<svelte:head>
</svelte:head>

<div>
<Header />
  <div class="contents-container">
    <Counter
      count={count}
    />
    <Button
      onClick={incrementCount} text='OnClick'
    />
  </div>
</div>

<style>
  .contents-container {
  padding-top: 50px;
}
:global(html, body, div, span, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
abbr, address, cite, code,
del, dfn, em, img, ins, kbd, q, samp,
small, strong, sub, sup, var,
b, i,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, figcaption, figure,
footer, header, hgroup, menu, nav, section, summary,
time, mark, audio, video) {
  margin:0;
  padding:0;
  border:0;
  outline:0;
  font-size:100%;
  vertical-align:baseline;
  background:transparent;
}

:global(body) {
  line-height:1;
}

:global(article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section) {
  display:block;
}

:global(nav ul) {
  list-style:none;
}

:global(blockquote, q) {
  quotes:none;
}

:global(blockquote:before, blockquote:after,
q:before, q:after) {
  content:'';
  content:none;
}

:global(a) {
  margin:0;
  padding:0;
  font-size:100%;
  vertical-align:baseline;
  background:transparent;
}

/* change colours to suit your needs */
:global(ins) {
  background-color:#ff9;
  color:#000;
  text-decoration:none;
}

/* change colours to suit your needs */
:global(mark) {
  background-color:#ff9;
  color:#000;
  font-style:italic;
  font-weight:bold;
}

:global(del) {
  text-decoration: line-through;
}

:global(abbr[title], dfn[title]) {
  border-bottom:1px dotted;
  cursor:help;
}

:global(table) {
  border-collapse:collapse;
  border-spacing:0;
}

/* change border colour to suit your needs */
:global(hr) {
  display:block;
  height:1px;
  border:0;
  border-top:1px solid #cccccc;
  margin:1em 0;
  padding:0;
}

:global(input, select) {
  vertical-align:middle;
}
</style>
