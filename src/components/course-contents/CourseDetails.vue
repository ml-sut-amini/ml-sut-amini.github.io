<script setup>
</script>

<script>
export default {
  name: "Syllabus",
  data() {
    return {
      presentations: [
        {
          title: "1. Introduction",
          description: "Supervised & Unsupervised Learning, Unconditional & Conditional Generative Models, Discriminative & Generative Classification",
          link: "/assets/presentation-slides/DGM_Presentation-1_Introduction.pdf"
        },
        {
          title: "2. Foundation",
          description: "Notions, Probability & Statistics, Foundational Mathematical and Theoretical Concepts",
          link: "/path/to/DGM_Presentation-2_Foundation.pdf"
        },
        {
          title: "3. Deep Autoregressive Models",
          description: "Fully visible Sigmoid Belief Network (FVSBN), Neural Autoregressive Density Estimation (NADE), Masked Autoencoder for Distribution Estimation (MADE), Recurrent Neural Networks (RNN), Conditional Generation",
          link: "/path/to/DGM_Presentation-3_Deep_Autoregressive_Models.pdf"
        },
        {
          title: "4. Variational Autoencoders",
          description: "Guassian Mixture Model (GMM), Model Specification, Casting Likelihood Calculation as Expectation, Importance Sampling, Evidence Lower Bound, ELBO, Reparameterization Trick, Amortizationm, Revisiting Objective Function, Attribute Vectors in Code Space",
          link: "/path/to/DGM_Presentation-4_Variational_Autoencoders.pdf"
        },
        {
          title: "5. Flow Models",
          description: "Change of Variable Theorem, Normalizing Flow Models, Nonlinear Independent Component Estimation (NICE), Real-valued Non-volume Preserving Transformations (RealNVP), Masked Autoregressive Flows, Inverse Autoregressive Flows",
          link: "/path/to/DGM_Presentation-5_Flow_Models.pdf"
        },
        {
          title: "6. GANs",
          description: "Training Algorithm, Deep Convolutional GAN, Mode Collapse, f-GAN, Bidirectional Generative Adversarial Networks, CycleGAN",
          link: "/path/to/DGM_Presentation-6_GAN.pdf"
        },
        {
          title: "7. Energy-Based Models",
          description: "Sampling EBM, Contrastive Divergence, Score Matching, Noise Conditional Score Networks (NCSN)",
          link: "/path/to/DGM_Presentation-7_Energy_Based_Models.pdf"
        },
        {
          title: "8. Diffusion Models",
          description: "Markovian Hierarchical Variational Autoencoders, Variational Diffusion Models, Denoising Matching",
          link: "/path/to/DGM_Presentation-8_Diffusion_Models.pdf"
        }
      ]
    };
  }
};
</script>

<template>
    <div class="sub-section">
      <div class="sub-section-content">
        <div class="sub-title">Prerequisites</div>
        <div class="sub-content">
          <ul class="prerequisites">
            <li>A solid understanding of probability, statistics, and linear algebra is essential.</li>
            <li>Prior knowledge of machine learning from courses such as AI, Machine Learning, or Deep Learning is expected.</li>
            <li>Proficiency in Python programming is required.</li>
            <li>Familiarity with computational and mathematical models, including calculus, will be beneficial for working on advanced topics in this course.</li>
          </ul>
        </div>
      </div>
      <div class="sub-section-content">
        <div class="sub-title">Syllabus</div>
        <div class="sub-content syllabus">
          <ul>
            <li v-for="(presentation, index) in presentations" :key="index">
              <a :href="presentation.link" target="_blank" class="font-bold">{{ presentation.title }}:</a>
              <p>{{ presentation.description }}</p>
            </li>
          </ul>
        </div>
      </div>
    </div>
</template>

<style scoped>
.font-bold {
  font-weight: 700;
}

.syllabus ul {
  list-style-type: none;
  padding: 0;
}

.syllabus > ul > li {
  margin: 10px 0;
  padding-left: 0;
}

.syllabus > ul > li::before {
  content: "";
}

.syllabus a {
  text-decoration: none;
  color: #1e88e5;
}

.syllabus a:hover {
  text-decoration: underline;
}

@media (max-width: 450px) {
  .sub-section-content .sub-content {
    padding-left: 0 !important;
  }
}
</style>