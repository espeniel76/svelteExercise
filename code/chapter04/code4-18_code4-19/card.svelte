<style>
.contact-card {
    width: 300px;
    border: 1px solid #aaa;
    border-radius: 2px;
    box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
    padding: 1em;
  }

  h2 {
    padding: 0 0 0.2em 0;
    margin: 0 0 1em 0;
    border-bottom: 1px solid #ff3e00;
  }

  .address, .email {
    padding: 0 0 0 1.5em;
    background:  0 50% no-repeat;
    background-size: 1em 1em;
    margin: 0 0 0.5em 0;
    line-height: 1.2;
  }

  .address { background-image: url(tutorial/icons/map-marker.svg) }
  .email   { background-image: url(tutorial/icons/email.svg) }
  .missing { color: #999 }
</style>

<article class="contact-card">
  <h2>
    <slot name="name">
      <span class="missing">이름 미입력</span>
    </slot>
  </h2>

  <div class="address">
    <slot name="address">
      <span class="missing">주소 미입력</span>
    </slot>
  </div>

  <div class="email">
    <slot name="email">
      <span class="missing">이메일 미입력</span>
    </slot>
  </div>
</article>
