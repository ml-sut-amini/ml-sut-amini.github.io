<script setup lang="ts">
</script>

<template>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Class Schedule</div>
      <div class="sub-content">
        <ul>
        <li>The class is scheduled for Sundays and Tuesdays from 12:00 to 13:30.</li>
        <li>Classes will be held <span class="font-bold">in person</span>;</li>
        <li>However, under special circumstances, the class might be held virtually with prior announcements.</li>
        <li>The virtual class link is:
          <a class="any-link" href="https://vc.sharif.edu/s-amini" target="_blank">
            https://vc.sharif.edu/s-amini
          </a>
        </li>
        </ul>
      </div>
    </div>
  </div>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Grading</div>
      <div class="sub-content">
        <p>Please be aware that grades will be calculated based on the following distribution:</p>
        <ul>
          <li><span class="font-bold">Project:</span> 20%</li>
          <li><span class="font-bold">Homework:</span> 30%</li>
          <li><span class="font-bold">Midterm:</span> 20%</li>
          <li><span class="font-bold">Final:</span> 30%</li>
          <li><span class="font-bold">Extra Credit:</span> Up to 5% for active class participation</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Exams</div>
      <div class="sub-content">
        <p>Students' performance will be evaluated through two Midterm Exams and one Final Exam:</p>
        <ul>
          <li><span class="font-bold">Midterm Exam 1:</span> 1403/08/15 during class time.</li>
          <li><span class="font-bold">Midterm Exam 2:</span> 1403/09/13 during class time.</li>
          <li><span class="font-bold">Final Exam:</span> 1403/11/03   15:00</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Homework</div>
      <div class="sub-content">
        <ul>
          <li>Four series of homework assignments will be given throughout this course.</li>
          <li>Homework assignments have to be submitted on <a class="any-link" href="https://cw.sharif.edu/" target="_blank">CW</a>.</li>
          <li>Late submissions will be accepted with no penalty up to 3 days for each assignment with a total delay of 10 days for all of them.</li>
          <li>Assignment grade reduces by 0.95 compounding factor for each day overdue beyond allowed late days.</li>
          <li>Solutions released 3 days post-deadline; homework not accepted afterward.</li>
          <li>To ensure fairness and consistency, we do not accept any requests for deadline extensions, as the delay policy is strictly enforced to maintain equal opportunities for all students.</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Project</div>
      <div class="sub-content">
        <p style="line-height: 1.6; margin-bottom: 15px;">
          This section outlines the pipeline for the course project, providing a structured approach to guide students through the different stages of their research work. The project is divided into three main steps: Project Setup, Literature Review, and Research and Execution.
          <u>Students are expected to continuously work on their project throughout the semester, ensuring steady progress and timely completion of each phase.</u>
        </p>

        <h4>Step 1: Project Setup</h4>
        <ol>
          <li>Relevant papers and research areas are suggested.</li>
          <li>Students select a research area and form groups (2 students per group).</li>
          <li>Group formations and chosen research areas are verified.</li>
          <li>Mentors are assigned to each group.</li>
          <li>Students draft and submit a project proposal.</li>
        </ol>

        <h4>Step 2: Literature Review</h4>
        <ol>
          <li>Students read related papers in the chosen research area.</li>
          <li>Prepare and present a literature review covering previous works.</li>
          <li>Identify a novel idea or problem to tackle based on the review.</li>
        </ol>

        <h4>Step 3: Research and Execution</h4>
        <ol>
          <li>Conduct research on the identified problem.</li>
          <li>Prove or simulate the solution and obtain results.</li>
          <li>Write a report (pseudo-paper) summarizing the work and prepare the final presentation.</li>
        </ol>
      </div>
    </div>
  </div>
  <div class="sub-section">
    <div class="sub-section-content">
      <div class="sub-title">Course Policies</div>
      <div class="sub-content">
        <h4>Late Submissions</h4>
        <ul>
          <li>You can use a total of 10 permissible late days for all homework assignments.</li>
          <li>Maximum extension of 3 days for any single homework.</li>
          <li>Assignment grade reduces by 0.95 compounding factor for each day overdue beyond allowed late days.</li>
          <li>Solutions released 3 days post-deadline; homework not accepted afterward.</li>
        </ul>
        
        <h4>Attendance</h4>
        <ul>
          <li>Attendance is essential for learning objectives due to extensive material coverage.</li>
          <li>No formal attendance mandate.</li>
        </ul>
      </div>
    </div>
  </div>
<!--  <div class="sub-section">-->
<!--    <div class="sub-section-content">-->
<!--      <div class="title font-bold text-2xl sm:text-2xl">Course Pages</div>-->
<!--      <div class="content text-black-600 text-md">-->
<!--        <ul style="padding-left: 20px;">-->
<!--          <li>GitHub</li>-->
<!--          <li>CW: <a class="any-link" href="https://cw.sharif.edu/" target="_blank">CW</a>.</li>-->
<!--        </ul>-->
<!--      </div>-->
<!--    </div>-->
<!--  </div>-->
</template>

<style scoped>
.font-bold {
  font-weight: 700;
}

.sub-content > p {
  margin-bottom: 15px;
}

.sub-content > h4 {
  margin-bottom: 10px;
  margin-top: 20px;
  font-weight: 600;
}

.sub-content > ol {
  line-height: 1.6;
}

.sub-content > ul > ul {
  list-style-type: none;
  padding-left: 30px;
}

.sub-content > ul > ul > li {
  padding-left: 20px;
  margin-bottom: 10px;
}

.sub-content > ul > ul > li::marker {
  content: "\2022";
  font-size: 20px;
  color: var(--dark-color);
  position: absolute;
  left: 0;
  top: 0;
}

.any-link {
  text-decoration: none;
  color: #1e88e5;
}

.any-link:hover {
  text-decoration: underline;
}

@media (max-width: 450px) {
  .sub-section-content .sub-content {
    padding-left: 0 !important;
  }
}
</style>