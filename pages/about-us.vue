<template>
  <div class="container is-fullhd">
    <section class="hero">
      <div class="hero-body">
        <h1 class="title is-1 has-text-right">
          داستان ما
        </h1>
        <b-image
          :src="require('~/assets/images/relyonit-about-banner.jpg')"
          alt="About RelyOnIt Theam"
          ratio="10by5"
        ></b-image>
      </div>
    </section>
    <div class="columns is-mobile is-centered">
      <div class="column is-half has-text-right">
        <p class="has-text-weight-light">
           رقابت در فضای کسب و کار های در بستر اینترنت روز به روز گسترده تر می شود و این رشد روز افزون، بدون کاهش ریسک های سازمان، پایدار نیست
           یکی از نقاط پر ریسک و حیاتی برای کسب و کار، دیتا ها و زیرساخت آن است که تیم ریلیونیت در صدد پایدارتر کردن و بهبود آن هاست
           همچنین با اتوماسیون فرایند توسعه ی نرم افزار تا حد ممکن، در تلاش است تا تاثیر عوامل خطای انسانی را در پایداری نرم افزار به حداقل برساند
        </p>
      </div>
    </div>
    <section class="section is-medium mb-5 has-text-centered">
      <h1 class="title is-2">تیم ما</h1>
      <h2 class="subtitle is-5">
        اعضای اصلی تیم ریلیونیت
      </h2>
      <div class="columns">
        <div class="column is-flex is-flex-direction-column">
          <figure class="image is-128x128 is-align-self-center mb-3">
            <img
              :src="require('~/assets/images/team-sadeghmohebbi.jpg')"
              alt="Ali MohammadAliRajab"
              class="is-rounded" />
          </figure>
          <p class="is-size-3">صادق محبی</p>
          <p>
            <a href="https://github.com/sadeghmohebbi" target="_blank" rel="noopener noreferrer" class="has-text-link">گیت هاب</a> | <a href="https://www.linkedin.com/in/sadegh-mohebbi-172476179/" target="_blank" rel="noopener noreferrer" class="has-text-link">لینکدین</a>
          </p>
        </div>
        <div class="column is-flex is-flex-direction-column">
          <figure class="image is-128x128 is-align-self-center mb-3">
            <img
              :src="require('~/assets/images/team-alimommadalirajab.jpg')"
              alt="Ali MohammadAliRajab"
              class="is-rounded" />
          </figure>
          <p class="is-size-3">علی محمدعلی رجب</p>
          <p>
            <a href="https://github.com/mohammadalirajab" target="_blank" rel="noopener noreferrer" class="has-text-link">گیت هاب</a> | <a href="https://www.linkedin.com/in/ali-mohammadalirajab-0aa542201/" target="_blank" rel="noopener noreferrer" class="has-text-link">لینکدین</a>
          </p>
        </div>
      </div>
    </section>
    <contact-us-section></contact-us-section>
  </div>
</template>