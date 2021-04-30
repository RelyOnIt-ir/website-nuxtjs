<template>
  <div class="container is-fullhd">
    <!-- Hero del producto -->
    <section class="hero is-white is-fullheight-with-navbar">
      <div class="hero-body">
        <div class="inner-container">
          <div class="columns is-vcentered">

            <div data-aos="fade-right" class="column
            is-10-mobile is-offset-1-mobile
            is-10-tablet is-offset-1-tablet
            is-4-desktop is-offset-1-desktop
            is-4-widescreen is-offset-1-widescreen
            is-4-fullhd is-offset-1-fullhd">
              <figure class="image is-square">
                <img :src="require('~/assets/images/undraw_Server_re_twwj.svg')">
              </figure>
            </div>

            <div class="column
            is-10-mobile is-offset-1-mobile
            is-10-tablet is-offset-1-tablet
            is-5-desktop is-offset-1-desktop
            is-5-widescreen is-offset-1-widescreen
            is-5-fullhd is-offset-1-fullhd" data-aos="fade-down">
              <h1 class="title is-1 mb-6 has-text-right">
                <span class="has-text-weight-bold">ریلیونیت</span> <br>
                به زیرساخت خود تکیه کنید
              </h1>
              <h2 class="subtitle has-text-grey is-4 has-text-weight-normal has-text-right">
                ما با بهره گیری از تکنولوژی های جدید و تجربه های متعدد، پایداری سیستم های نرم افزاری و سرعت توسعه تان را بهبود می دهیم
              </h2>
              <div class="buttons">
                <a class="button is-success" href="#contact-us">ارتباط با ما</a>
                <a class="button" href="#contact-us">درخواست مشاوره</a>
              </div>
            </div>

          </div>
        </div>
      </div>
    </section>

    <skill-hero-section 
      title="پیاده سازی DevOps"
      description="سرعت توسعه ی نرم افزار خود و بروزرسانی را با اتوماتیک کردن فرایند آن، بهبود داده و احتمال بروز خطاها را به حداقل کاهش دهید. تیم ریلیونیت در این مسیر همراه شماست"
      :image-src="require('~/assets/images/undraw_Project_completed_re_pqqq.svg')">
    </skill-hero-section>
    <skill-hero-section
      title="امنیت" 
      description="بسیاری از مشکلات امنیتی نرم افزار ها با راهکار های ساده ای قابل پیشگیری است. تیم ریلیونیت این موارد را تا حد امکان پیش بینی کرده و در صدد رفع آن ها برخواهد آمد" 
      :image-src="require('~/assets/images/undraw_Secure_server_re_8wsq.svg')">
    </skill-hero-section>
    <skill-hero-section
      title="حفاظت از داده ها" 
      description="پشتیبان گیری مطمئن و خودکار از داده ها بسیار حیاتی است. در کنار تیم ریلیونیت آن را محقق کنید" 
      :image-src="require('~/assets/images/undraw_folder_files_nweq.svg')">
    </skill-hero-section>
    <skill-hero-section
      title="مانیتورینگ و الرتینگ" 
      description="شاخص های سلامت سیستم شما در دستان شماست و زودتر از هر کسی از پیشامد های ناگهانی خبردار شوید و در صدد رفع آن درآیید. تیم ریلیونیت در این مسیر همراه شماست" 
      :image-src="require('~/assets/images/undraw_All_the_data_re_hh4w.svg')">
    </skill-hero-section>

    <section class="hero is-medium has-text-centered" id="testomonials">
      <h1 class="title is-2 mb-6">
        مشتریان ما
      </h1>
      <b-carousel data-aos="zoom-in-up">
          <b-carousel-item v-for="(testomonial, i) in testomonials" :key="i">
              <section class="hero is-medium">
                  <div class="hero-body has-text-centered rtl">
                      <p class="m-3 is-size-4 has-text-weight-light"> {{testomonial.text}} </p>
                      <p class="is-italic">
                        <a :href="testomonial.link" target="_blank" rel="noopener noreferrer" class="has-text-link">{{ testomonial.name }}</a> {{ testomonial.role }} <a :href="testomonial.website" target="_blank" rel="noopener noreferrer" class="has-text-link">{{ testomonial.brand }}</a>
                      </p>
                  </div>
              </section>
          </b-carousel-item>
      </b-carousel>
    </section>

    <contact-us-section></contact-us-section>
  </div>
</template>
<script>
import sample from 'lodash.sample'

export default {
  data: () => ({
    testomonials: [
      {
        text: sample([
          'همیشه این نگرانی تو بخش فنی استارتاپ مون داشتیم که چه کسی کارهای SysAdmin و برامون انجام بده تا تیم relyonit پیدا کردیم که تو سختترین لحظات به ما پشتیبانی دادن و باعث بهبود پایداری و زیر ساخت های فنی ما شدن.',
          'این روزها که تکنولوژی ها و لایه های مختلفی در تولید و توسعه اپلیکیشن و نرم افزارها هست، اهمیت بخش DevOps خیلی بیشتر شده تیم Relyonit فرآیندها و وظایف Devops رو تا حد زیادی برای شما به بهترین نحو انجام میده.',
          'حتما شما هم شنیدید که کلی از سایت ها چند وقت پیش بخاطر یک نفوذ و حمله سایبری دچار از دست رفتن اطلاعات شون شدن و متاسفانه خیلی هاشون حتی پلن backup گیری نداشتن که لطمات جبران ناپذیری بهشون وارد شد. تیم relyonit به بهترین شکل پلن های backup گیری رو برای ما اجرایی کرد و امروز خیالمون راحته که هر اتفاقی بیفته backup مطمئنی در دسترس مون هست.',
          'اسم این تیم خیلی درست انتخاب شده واقعا در بخش زیرساختی برای ما تکیه گاه بودن و در سخت ترین شرایط میشد روی همراهی شون حساب کرد.'
        ]),
        name: 'آرش خرسند',
        link: 'https://www.linkedin.com/in/arashkhorsand',
        role: 'هم بنیان گذار و مدیرعامل',
        brand: 'رومیتا',
        website: 'https://roomita.com'
      }
    ]
  })
}
</script>
