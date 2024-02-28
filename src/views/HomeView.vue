<template>
  <PrimaryHeader style="margin-bottom: 80px;" />
  <main>
    <section class="hero wrapper">
      <div class="hero__content">
        <h2 class="hero__title">
          Organize your <br> task more easily <br> with us
        </h2>
        <p class="hero__description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. At eum rerum voluptate quas, nisi eveniet similique sint quasi iusto 
          a maxime blanditiis impedit laudantium ut vel expedita? Aperiam, magnam fuga!
        </p>
        <div class="hero__buttons">
          <a class="hero__btn primary-btn">Get Started</a>
          <a class="hero__btn primary-btn primary-btn--link">How It Works?</a>
        </div>
      </div>
      <div class="hero__illustration">
        <TaskProgress />
        <div class="team">
          <div class="title-block">
            <h2 class="title-block__title">Our Team</h2>
            <p class="title-block__subtitle">Team members</p>
          </div>
          <div class="team__icons-wrapper">
            <div class="team__icon"></div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import PrimaryHeader from '@/components/ui/primary-header/PrimaryHeader.vue'
import TaskProgress from '@/components/ui/task-progress/TaskProgress.vue'

export default {
  components: {
    PrimaryHeader,
    TaskProgress
  },
  mounted() {
    const blackAccent = '#080402'
    document.body.style.background = blackAccent
    document.body.style.color = '#fff'
  }
}
</script>

<style scoped>
.hero {
  display: flex;
}

.hero__content {
  width: 50%;
}

.hero__title {
  margin-bottom: 20px;
  font-weight: 600;
  font-size: var(--fs-900);
  text-transform: capitalize;
}
</style>