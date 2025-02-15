<script setup>
const sampleTitle = 'Schedule';
</script>

<script>
export default {
  data() {
    return {
      sessions: [
        {
          event: 'normal',
          number: 1,
          date: '1403/07/01',
          topics: [
            {topic: 'Logistics', link: '/files/presentation-slides/DGM_Presentation-0_Logistics.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 2,
          date: '1403/07/03',
          topics: [
            {topic: 'Introduction', link: '/files/presentation-slides/DGM_Presentation-1_Introduction.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 3,
          date: '1403/07/08',
          topics: [
            {topic: 'Foundations', link: '/files/presentation-slides/DGM_Presentation-2_Foundation.pdf'},
          ],
          coursework: 'HW 1 Released',
          homework: '/files/assignments/DGM_HW1.zip',
          deadline: ''
        },
        {
          event: 'normal',
          number: 4,
          date: '1403/07/10',
          topics: [
            {topic: 'Deep Autoregressive Models', link: '/files/presentation-slides/DGM_Presentation-3_Deep Autoregressive Models.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 5,
          date: '1403/07/15',
          topics: [
            {topic: 'Deep Autoregressive Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 6,
          date: '1403/07/17',
          topics: [
            {topic: 'Deep Autoregressive Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 7,
          date: '1403/07/22',
          topics: [
            {topic: 'Deep Variational Autoencoders', link: '/files/presentation-slides/DGM_Presentation-4_Variational Autoencoders.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 8,
          date: '1403/07/24',
          topics: [
            {topic: 'Deep Variational Autoencoders', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'deadline',
          number: '',
          date: 'Thu 1403/07/26',
          topics: [
            {topic: '', link: ''},
          ],
          coursework: 'HW 2 Release',
          homework: '/files/assignments/DGM_HW2.zip',
          deadline: 'HW 1 Deadline'
        },
        {
          event: 'normal',
          number: 9,
          date: '1403/07/29',
          topics: [
            {topic: 'Deep Variational Autoencoders', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 10,
          date: '1403/08/01',
          topics: [
            {topic: 'Deep Variational Autoencoders', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 11,
          date: '1403/08/06',
          topics: [
            {topic: 'Normalizing Flow Models', link: '/files/presentation-slides/DGM_Presentation-5_Flow Models.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 12,
          date: '1403/08/08',
          topics: [
            {topic: 'Normalizing Flow Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'deadline',
          number: '',
          date: 'Thu 1403/08/10',
          topics: [
            {topic: '', link: ''},
          ],
          coursework: 'HW 3 Release',
          homework: '/files/assignments/DGM_HW3.zip',
          deadline: 'HW 2 Deadline'
        },
        {
          event: 'normal',
          number: 13,
          date: '1403/08/13',
          topics: [
            {topic: 'Normalizing Flow Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'exam',
          number: 14,
          date: '1403/08/15',
          topics: [
            {topic: 'Midterm Exam 1 (Autoregressive, VAE)', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 15,
          date: '1403/08/20',
          topics: [
            {topic: 'Normalizing Flow Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 16,
          date: '1403/08/22',
          topics: [
            {topic: 'Generative Adversarial Nets', link: '/files/presentation-slides/DGM_Presentation-6_GAN.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 17,
          date: '1403/08/27',
          topics: [
            {topic: 'Generative Adversarial Nets', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 18,
          date: '1403/08/29',
          topics: [
            {topic: 'Generative Adversarial Nets', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 19,
          date: '1403/09/04',
          topics: [
            {topic: 'Generative Adversarial Nets', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 20,
          date: '1403/09/06',
          topics: [
            {topic: 'Energy-Based Models', link: '/files/presentation-slides/DGM_Presentation-7_Energy Based Models.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'deadline',
          number: '',
          date: 'Thu 1403/09/08',
          topics: [
            {topic: '', link: ''},
          ],
          coursework: '',
          deadline: 'HW 3 Deadline'
        },
        {
          event: 'normal',
          number: 21,
          date: '1403/09/11',
          topics: [
            {topic: 'Energy-Based Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'exam',
          number: 22,
          date: '1403/09/13',
          topics: [
            {topic: 'Midterm Exam 2 (Flow Models, GAN)', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 23,
          date: '1403/09/18',
          topics: [
            {topic: 'Energy-Based Models', link: ''},
          ],
          coursework: 'HW 4 Release',
          homework: '/files/assignments/DGM_HW4.zip',
          deadline: ''
        },
        {
          event: 'normal',
          number: 24,
          date: '1403/09/20',
          topics: [
            {topic: 'Energy-Based Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 25,
          date: '1403/09/25',
          topics: [
            {topic: 'Diffusion Models', link: '/files/presentation-slides/DGM_Presentation-8_Diffusion Models.pdf'},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 26,
          date: '1403/09/27',
          topics: [
            {topic: 'Diffusion Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 27,
          date: '1403/09/02',
          topics: [
            {topic: 'Diffusion Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 28,
          date: '1403/09/04',
          topics: [
            {topic: 'Diffusion Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 29,
          date: '1403/10/09',
          topics: [
            {topic: 'Diffusion Models', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'normal',
          number: 30,
          date: '1403/10/11',
          topics: [
            {topic: 'Evaluation Methods', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        {
          event: 'deadline',
          number: '',
          date: 'Fri 1403/10/14',
          topics: [
            {topic: '', link: ''},
          ],
          coursework: '',
          deadline: 'HW 4 Deadline'
        },
        {
          event: 'exam',
          number: '',
          date: '1403/11/03',
          topics: [
            {topic: 'Final Exam 15:00', link: ''},
          ],
          coursework: '',
          deadline: ''
        },
        // Add more sessions as needed
      ]
    }
  },
  methods: {
    rowClass(event) {
      switch (event) {
        case 'normal':
          return 'bg-gray-100';
        case 'deadline':
          return 'bg-red-100';
        case 'exam':
          return 'bg-yellow-100';
        case 'off':
          return '';
        default:
          return '';
      }
    }
  }
}
</script>

<template>
  <div class="section">
    <div class="section-content">
      <div class="title">{{ sampleTitle }}</div>
<!--      <div class="content text-gray-600 text-md">{{ shortDescription }}</div>-->
      <div class="container">
<!--        <h2 class="text-2xl font-bold mb-4 text-center">Lecture Schedule</h2>-->
        <div class="table-container">
          <table class="table-class">
            <thead>
            <tr class="table-head-row">
              <th class="table-head-item">Session</th>
              <th class="table-head-item">Date</th>
              <th class="table-head-item">Lecture Topics</th>
              <th class="table-head-item">Events</th>
              <th class="table-head-item">Deadline</th>
            </tr>
            </thead>
            <tbody>
            <tr v-for="(session, index) in sessions" :key="index" :class="rowClass(session.event)" class="table-body-row transition-colors">
              <td>{{ session.number }}</td>
              <td>{{ session.date }}</td>
              <td class="lecture-topics">
                <template v-for="(item, i) in session.topics" :key="i">
                  <p>{{ item.topic }}
                  <span v-if="item.link !== ''">
                    [<a style="width: fit-content; color: blue;" :href="item.link" target="_blank">Slide</a>]
                  </span>
                  <span v-if="i !== session.topics.length - 1">, </span>
                  </p>
                </template>
              </td>
              <td class="event">
                <a v-if="'homework' in session" style="text-decoration: underline;" :href="session.homework" target="_blank" download>
                  {{ session.coursework }}
                </a>
                <p v-else>{{ session.coursework }}</p>
              </td>
              <td class="deadline">{{ session.deadline }}</td>
            </tr>
            </tbody>
          </table>
        </div>
      </div>
      <div class="sub-section">
        <div class="sub-section-content">
          <div class="sub-title">Additional Materials</div>
          <div class="sub-content">
            <ul>
              <li><a class="any-link" href="http://yang-song.github.io/blog/2021/score/">Generative Modeling by Estimating Gradients of the Data Distribution.</a> Yang Song. Blog post on score-based generative models, May 2021.</li>
              <li><a class="any-link" href="https://arxiv.org/abs/2101.03288">How to Train Your Energy-Based Models.</a> Yang Song and Diederik P. Kingma. February 2021. </li>
              <li><a class="any-link" href="https://ermongroup.github.io/generative-models/">Tutorial on Deep Generative Models.</a> Aditya Grover and Stefano Ermon. International Joint Conference on Artificial Intelligence, July 2018.</li>
              <li><a class="any-link" href="https://sites.google.com/view/cvpr2018tutorialongans/">Tutorial on Generative Adversarial Networks.</a> Computer Vision and Pattern Recognition, June 2018.</li>
              <li><a class="any-link" href="https://www.youtube.com/watch?v=JrO5fSskISY">Tutorial on Deep Generative Models.</a> Shakir Mohamed and Danilo Rezende. Uncertainty in Artificial Intelligence, July 2017.</li>
              <li><a class="any-link" href="https://www.youtube.com/watch?v=AJVyzd0rqdc">Tutorial on Generative Adversarial Networks.</a> Ian Goodfellow. Neural Information Processing Systems, December 2016.</li>
              <li><a class="any-link" href="https://www.cs.cmu.edu/~rsalakhu/papers/annrev.pdf">Learning deep generative models.</a> Ruslan Salakhutdinov. Annual Review of Statistics and Its Application, April 2015.</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.event > p, a {
  font-weight: bold;
  color: #181e4b;
}

.event > a {
  cursor: pointer;
}

.deadline {
  color: red;
  font-weight: bold;
}

.container {
  margin-bottom: 50px;
}

.table-container {
  border-radius: 0.5rem;
  overflow-x: auto;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.table-class {
  background-color: rgb(255 255 255);
  border-color: rgb(229 231 235);
  border-width: 1px;
  min-width: 100%;
  text-indent: 0;
}

.table-head-row {
  text-align: left;
  color: rgb(255 255 255);
}

.table-head-item {
  font-weight: 600;
  font-size: 0.875rem;
  line-height: 1.6;
}

.table-body-row {
  border-bottom: 1px solid var(--border-color);
}

table {
  border-collapse: collapse;
}
th, td {
  padding: 12px;
  height: fit-content;
  font-size: 0.875rem;
  line-height: 1.6;
  border-left: 1px solid var(--border-color);
  text-align: center;
  min-height: 50px;
}
thead {
  background-color: var(--secondary-color);
  color: white;
}

.sub-section .sub-title {
  margin-bottom: 10px;
}

.lecture-topics {
  display: flex;
  justify-content: space-evenly;
  color: #181e4b;
  font-weight: 500;
}

.any-link {
  text-decoration: none;
  color: #1e88e5;
}

.any-link:hover {
  text-decoration: underline;
}

.transition-colors {
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

.bg-gray-100 {
  background-color: #f5f5f5;
}

.bg-yellow-100 {
  background-color: rgb(254 249 195);
}

.bg-red-100 {
  background-color: rgb(254 226 226);
}

.bg-gray-100:hover {
  background-color: var(--vt-c-white-mute);
}

.bg-yellow-100:hover {
  background-color: rgb(254 239 175);
}

.bg-red-100:hover {
  background-color: rgb(254 206 206);
}

@media (max-width: 1024px) {
  .lecture-topics {
    flex-direction: column;
  }
}
</style>