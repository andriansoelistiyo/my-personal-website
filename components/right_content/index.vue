<template>
  <div class="a-card p-16">
    <div class="content_group">
      <h2 class="h2-text">Skills</h2>
      <LazyPillGroup :items="skills" />
    </div>
    <hr />
    <div class="content_group mt-16">
      <h2 class="h2-text">Tools</h2>
      <LazyPillGroup :items="tools" />
    </div>
    <hr />
    <div class="content_group mt-16">
      <h2 class="h2-text">Portofolio and case study</h2>
      <div class="link_group mt-16">
        <div class="body-text mb-8">
          <i class="fab fa-medium mr-8"></i>
          <a href="https://andriansoelistiyo.medium.com/" target="_blank"
            >andriansoelistiyo.medium.com/</a
          >
        </div>
        <div class="body-text mb-8">
          <i class="fab fa-behance-square mr-8"></i>
          <a href="https://www.behance.net/andriansoelist" target="_blank"
            >behance.net/andriansoelist/</a
          >
        </div>
        <div class="body-text">
          <i class="fab fa-github-square mr-8"></i>
          <a href="https://github.com/andriansoelistiyo" target="_blank"
            >github.com/andriansoelistiyo/</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RightContent',
  data() {
    return {
      skills: [
        {
          id: 1,
          value: 'User Research',
        },
        {
          id: 2,
          value: 'Affinity Map',
        },
        {
          id: 3,
          value: 'Information Architecture',
        },
        {
          id: 4,
          value: 'User Flow',
        },
        {
          id: 5,
          value: 'Wireflow',
        },
        {
          id: 6,
          value: 'Wireframe',
        },
        {
          id: 7,
          value: 'Lo-Fi Design',
        },
        {
          id: 8,
          value: 'Hi-Fi Design',
        },
        {
          id: 9,
          value: 'Prototyping',
        },
        {
          id: 10,
          value: 'Usability Testing',
        },
        {
          id: 11,
          value: 'A/B Testing',
        },
        {
          id: 12,
          value: 'HTML',
        },
        {
          id: 13,
          value: 'CSS',
        },
        {
          id: 14,
          value: 'JavaScript',
        },
        {
          id: 15,
          value: 'Vue JS',
        },
        {
          id: 16,
          value: 'Nuxt JS',
        },
      ],
      tools: [
        {
          id: 1,
          value: 'Figma',
        },
        {
          id: 2,
          value: 'Adobe XD',
        },
        {
          id: 3,
          value: 'Overflow',
        },
        {
          id: 4,
          value: 'Draw.io',
        },
        {
          id: 5,
          value: 'Mural',
        },
        {
          id: 6,
          value: 'Miro',
        },
        {
          id: 7,
          value: 'Maze',
        },
        {
          id: 8,
          value: 'Lookback',
        },
        {
          id: 9,
          value: 'Visual Studio Code',
        },
        {
          id: 10,
          value: 'Github',
        },
        {
          id: 11,
          value: 'Gitlab',
        },
        {
          id: 12,
          value: 'Google Analytics',
        },
        {
          id: 13,
          value: 'Google Optimize',
        },
        {
          id: 14,
          value: 'Google Data Studio',
        },
      ],
    }
  },
}
</script>
