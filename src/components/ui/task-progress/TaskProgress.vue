<template>
    <div class="task-progress">
        <div class="title-block">
            <h2 class="title-block__title">Task Progress</h2>
            <p class="title-block__subtitle">Recent all kind of running tasks</p>
        </div>
      <div class="task-progress__bars-wrapper">
        <div v-for="progress in progresses" :key="progress.progress" class="task-progress__bar-wrapper">
            <div class="task-progress__bar-header">
                <h3 class="task-progress__bar-title">{{ progress.name }}</h3>
                <span class="task-progress__bar-count">{{ progress.progress }}/10</span>
            </div>
          <div class="task-progress__bar">
            <div class="task-progress__bar-progress" :style="{width: (progress.progress * 10) + '%'}"></div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            progresses: [
                {
                    name: 'Web Ui Design',
                    progress: 5
                },
                {
                    name: 'Mobile App Design',
                    progress: 8
                },
                {
                    name: 'Web App Design',
                    progress: 7
                }
            ]
        }
    }
}
</script>

<style scoped>
.task-progress {
    background: var(--clr-black-500);
    border-radius: 10px;
    padding: 25px;
}

.task-progress__bar {
    position: relative;
    width: 100%;
    height: 10px;
    background: #faf5f5;
    margin: 5px 0;
    border-radius: 10px;
}

.task-progress__bar-progress {
    content: '';
    position: absolute;
    height: 100%;
    width: 50%;
    background: var(--clr-yellow-400);
    border-radius: 10px;
}

.task-progress__bar-header {
    display: flex;
    justify-content: space-between;
}

.task-progress__bar-count {
    opacity: 0.5;
}
</style>