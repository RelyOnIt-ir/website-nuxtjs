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

    <section class="hero is-medium has-text-centered" id="contact-us">
      <div class="hero-body">
        <div class="inner-container">
          <div class="columns is-centered">
            <div data-aos="zoom-in-up" class="column is-8">
              <h1 class="title is-2 mb-6">
                یک قدم تا نگهداری و بهبود زیرساخت نرم افزاری شما
              </h1>
              <h2 class="subtitle">
                <p class="is-size-5 is-centered my-2">جهت مشاوره با ما تماس بگیرید</p>
                <b-tag type="is-success" size="is-large" class="p-5 has-text-weight-normal rtl">
                  تلفن تماس: <span class="is-size-4 has-text-weight-bold">۰۲۱۲۸۴۲۹۱۸۲</span>
                  <a href="tel:02128429182"><b-icon icon="phone" size="is-small" type="is-white" class="m-1"></b-icon></a>
                </b-tag>
              </h2>
            </div>
          </div>

        </div>
      </div>
    </section>
  </div>
</template>
