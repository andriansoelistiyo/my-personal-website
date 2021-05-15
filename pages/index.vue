<template>
  <div v-if="$device.isDesktop">
    <div class="container">
      <div class="py-32">
        <LazyBio />
        <div class="row">
          <div class="col-8">
            <LazyWorkExperiences class="mt-32" />
            <LazyPersonalProjects class="mt-32" />
            <LazyEducation class="mt-32" />
          </div>
          <div class="col-4">
            <LazyRightContent class="mt-32" />
          </div>
        </div>
        <div class="body-text text-center mt-32">
          Copyright © {{ new Date().getFullYear() }}, designed by
          <a href="https://andriansoelistiyo.netlify.app/" target="_blank"
            >Andrian Soelistiyo</a
          >
        </div>
      </div>
    </div>
  </div>
  <div v-else-if="$device.isMobile">
    <div class="container text-center">
      <img
        class="img-fluid mt-32"
        src="https://cdn.dribbble.com/users/308895/screenshots/2598725/no-results.gif"
        alt="no content"
      />
    </div>
  </div>
</template>

<script>
import ogImage from '@/assets/img/logo/nuxt.png'
export default {
  head() {
    return {
      title: 'Andrian Soelistiyo - My personal website',
      meta: [
        {
          name: 'keywords',
          content:
            'curriculum vitae, biodata, work experiences, personal projects, education, skills, tools, portofolio, case study',
        },
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            'My personal website that serve you informations about curriculum vitae, biodata, work experiences, personal projects, education, skills, tools, portofolio, case study',
        },
        {
          name: 'fb:app_id',
          property: 'fb:app_id',
          content: '100001006063938',
        },
        {
          name: 'og:image',
          property: 'og:image',
          content: 'https://andriansoelistiyo.netlify.app' + ogImage,
        },
        {
          name: 'og:title',
          property: 'og:title',
          content: 'Andrian Soelistiyo - Personal website',
        },
        {
          name: 'og:site_name',
          property: 'og:site_name',
          content: 'Andrian Soelistiyo - Personal website',
        },
        {
          name: 'og:url',
          property: 'og:url',
          content: 'https://andriansoelistiyo.netlify.app/',
        },
        {
          name: 'og:description',
          property: 'og:description',
          content:
            'My personal website that serve you informations about curriculum vitae, biodata, work experiences, personal projects, education, skills, tools, portofolio, case study',
        },
        { name: 'og:locale', property: 'og:locale', content: 'id_ID' },
        {
          name: 'og:image:secure_url',
          property: 'og:image:secure_url',
          content: 'https://andriansoelistiyo.netlify.app' + ogImage,
        },
        { name: 'og:type', property: 'og:type', content: 'article' },
        { name: 'twitter:card', content: 'summary_large_image' },
        {
          name: 'twitter:title',
          content: 'Andrian Soelistiyo - Personal website',
        },
        { name: 'twitter:site', content: '@andriantweets' },
        {
          name: 'twitter:url',
          content: 'https://andriansoelistiyo.netlify.app/',
        },
        {
          name: 'twitter:description',
          content:
            'My personal website that serve you informations about curriculum vitae, biodata, work experiences, personal projects, education, skills, tools, portofolio, case study',
        },
        {
          name: 'twitter:image',
          content: 'https://andriansoelistiyo.netlify.app' + ogImage,
        },
      ],
      link: [
        {
          rel: 'canonical',
          href: 'https://andriansoelistiyo.netlify.app/',
        },
      ],
    }
  },
}
</script>
