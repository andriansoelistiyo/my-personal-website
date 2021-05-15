<template>
  <div class="experience_group mt-16">
    <div v-for="item in items" :key="item.id" class="a-experience">
      <div class="d-flex">
        <div class="flex-shrink-0 mr-32">
          <img
            class="company-logo img-fluid rounded"
            width="48"
            height="48"
            :src="item.logo"
            :alt="item.company"
          />
        </div>
        <div class="flex-grow-1">
          <div class="head-content">
            <div class="body-text">
              <span class="fw-bold">{{ item.company }}</span>
              • {{ item.type }} •
              <a :href="item.website" target="_blank"
                >See Website <i class="fas fa-external-link-alt"></i
              ></a>
            </div>
            <div class="body-text text-info">
              {{ item.occupation }}
            </div>
            <div class="body-text">
              {{ item.start_date }} - {{ item.end_date }}
            </div>
          </div>
          <div class="mt-16">
            <div class="row">
              <div class="col-6">
                <ul class="body-text">
                  <li v-if="item.task_1 !== null && item.task_1 !== ''">
                    {{ item.task_1 }}
                  </li>
                  <li
                    v-if="item.task_3 !== null && item.task_3 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_3 }}
                  </li>
                  <li
                    v-if="item.task_5 !== null && item.task_5 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_5 }}
                  </li>
                  <li
                    v-if="item.task_7 !== null && item.task_7 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_7 }}
                  </li>
                  <li
                    v-if="item.task_9 !== null && item.task_9 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_9 }}
                  </li>
                  <li
                    v-if="item.task_11 !== null && item.task_11 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_11 }}
                  </li>
                  <li
                    v-if="item.task_13 !== null && item.task_13 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_13 }}
                  </li>
                </ul>
              </div>
              <div class="col-6">
                <ul class="body-text">
                  <li v-if="item.task_2 !== null && item.task_2 !== ''">
                    {{ item.task_2 }}
                  </li>
                  <li
                    v-if="item.task_4 !== null && item.task_4 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_4 }}
                  </li>
                  <li
                    v-if="item.task_6 !== null && item.task_6 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_6 }}
                  </li>
                  <li
                    v-if="item.task_8 !== null && item.task_8 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_8 }}
                  </li>
                  <li
                    v-if="item.task_10 !== null && item.task_10 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_10 }}
                  </li>
                  <li
                    v-if="item.task_12 !== null && item.task_12 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_12 }}
                  </li>
                  <li
                    v-if="item.task_14 !== null && item.task_14 !== ''"
                    class="mt-8"
                  >
                    {{ item.task_14 }}
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ExperienceGroup',
  props: {
    items: {
      type: Array,
      required: true,
    },
  },
}
</script>

<style scoped>
.company-logo {
  width: 48px;
  height: 48px;
}
.a-experience:first-child {
  margin-bottom: 32px;
}
.a-experience {
  margin-bottom: 32px;
}
.a-experience:last-child {
  margin-bottom: 0;
}
</style>
