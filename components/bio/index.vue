<template>
  <div class="a-card p-16">
    <LazyBioContent :items="bio" />
  </div>
</template>

<script>
export default {
  name: 'Bio',
  data() {
    return {
      bio: [
        {
          id: 1,
          profile_image: require('~/assets/img/profile2.jpeg'),
          name: 'Andrian Soelistiyo',
          occupation: 'UX Designer',
          city: 'Kota Tangerang, Banten',
          about:
            'Hello, my name is Andrian Soelistiyo, live in Tangerang with my parents. Currently I’m 27 years old, I’ve been working for 3+ years as UX Designer and Front End Developer. I love help people with technology, build a product to solve their problem and make an impact for a better life.',
          whatsapp: '87788087738',
          email: 'andrian.socialmedia@gmail.com',
          linkedin: 'Andrian Soelistiyo',
          linkedin_link:
            'https://www.linkedin.com/in/andrian-soelistiyo-6a9324a1/',
          instagram: '@andrian.soelistiyo',
          instagram_link: 'https://www.instagram.com/andrian.soelistiyo/',
          twitter: '@andriantweets',
          twitter_link: 'https://twitter.com/andriantweets/',
        },
      ],
    }
  },
}
</script>
