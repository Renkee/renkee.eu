<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang="scss">
@font-face {
  font-family: 'Space Grotesk';
  font-style: normal;
  font-weight: 300 700;
  src: url('/main_font.woff2') format('woff2');
}

@font-face {
  font-family: 'Space Mono';
  src: url('/mono_font.ttf') format('truetype');
}

/* http://meyerweb.com/eric/tools/css/reset/
   v2.0 | 20110126
   License: none (public domain)
*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
body {
  line-height: 1;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: '';
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
// Own css
body {
  font-family: 'Space Grotesk', sans-serif !important;
  color: #333;
}
h1 {
  font-size: 3.5rem;
  font-weight: 600;
  margin-bottom: 1.5rem;
}
h2 {
  font-size: 2.5rem;
  font-weight: 550;
  margin-bottom: 0.5rem;
}
h3 {
  font-size: 1.8rem;
  font-weight: 450;
  margin-bottom: 0.75rem;
}
h4 {
  font-size: 1rem;
  font-weight: 300;
  margin-bottom: 0.25rem;
  font-family: 'Space Mono', monospace;
}
p {
  font-size: 1.4rem;
  font-weight: 420;
  line-height: calc(1.7rem + 0.2vw);
  margin-bottom: 0.65rem;
}
.section-container {
  max-width: 900px;
  margin: 0 auto;
  padding: 4rem 1rem;
}
a {
  color: #9b59b6;
}
a:hover {
  color: #582d69;
}
video {
  /* override other styles to make responsive */
  width: 100% !important;
  height: auto !important;
}
</style>
