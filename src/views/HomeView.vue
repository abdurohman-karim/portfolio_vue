<script>
export default {
  data() {
    return {
      isDarkMode: false,
    };
  },
  mounted() {
    this.setInitialTheme();
  },
  methods: {
    setInitialTheme() {
      this.isDarkMode = localStorage.getItem('darkMode') === 'enabled';
      console.log('Initial theme set:', this.isDarkMode);
      this.updateTheme();
    },
    toggleDarkMode() {
      this.isDarkMode = !this.isDarkMode;
      console.log('Theme toggled:', this.isDarkMode);
      this.updateTheme();
      localStorage.setItem('darkMode', this.isDarkMode ? 'enabled' : 'disabled');
    },
    updateTheme() {
      const root = document.documentElement;
      root.classList.toggle('dark-theme', this.isDarkMode);
      console.log('Theme updated');
      this.updateThemeIcon();
      // Other logic as needed
      // ...
    },
    updateThemeIcon() {
      console.log('Theme icon updated');
      const themeIcon = document.getElementById('themeIcon');
      if (themeIcon) {
        const sunSVG = `<svg ...> <!-- Your sun SVG code here --> </svg>`;
        const moonSVG = `<svg ...> <!-- Your moon SVG code here --> </svg>`;
        themeIcon.innerHTML = this.isDarkMode ? sunSVG : moonSVG;
      }
    },
  },
};
</script>

<template>
  <div>
    <!-- hero start -->
    <div class="section hero" id="home" :style="{ 'background-image': sectionBackgroundImage }">
        <div class="container">
            <div class="hero__banner">
                <p>echo <i class="shine">"Welcome!"</i>;</p>
            </div>
            <div class="hero__ellipse">
                <img src="../assets/images/ellipse.png">
            </div>
            <p class="hero__author">Abdurohman Karim</p>
            <p class="hero__title job">
                <span aria-hidden="true"></span>
            </p>
            <a href="#" class="hero__button">Apply</a>
        </div>
    </div>
    <!-- hero end -->

    <!-- heading start -->
    <div class="heading" id="about">
        <div class="container">
            <div class="heading__icon">
                <img src="../assets/images/bar-chart.png">
            </div>
            <p class="heading__title">$_GET(<i>'About'</i>)</p>
            <p class="heading__text">
                Utility classes help you work within the constraints of a system instead of littering your stylesheets with arbitrary values. They make it easy to be consistent with color choices, spacing, typography, shadows, and everything else that makes up a well-engineered design system.
            </p>
        </div>
    </div>
    <!-- heading end -->

    <!-- about start -->
    <div class="section about">
        <div class="container">
            <div class="stat_row">
                <div class="about__stat-card">
                    <p class="stat-number">20+</p>
                    <p class="stat-text">Projects</p>
                </div>
                <div class="about__stat-card">
                    <p class="stat-number">100+</p>
                    <p class="stat-text">Clients</p>
                </div>
                <div class="about__stat-card">
                    <p class="stat-number">15+</p>
                    <p class="stat-text">Co. Members</p>
                </div>
                <div class="about__stat-card">
                    <p class="stat-number">5+</p>
                    <p class="stat-text">CRM Systems</p>
                </div>
            </div>
            <div class="info_row">
                <div class="ic-info about__info-card">
                    <p class="info-card__title">Why do you never see elephants hiding in trees?</p>
                    <p class="info-card__text">
                        Because they're so good at it. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat. Because the pee is silent. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat. Because the pee is silent. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat. Because the pee is silent. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat.
                    </p>
                </div>
                <div class="ic-unique about__info-card">
                    <div class="ic-systems">
                        <div class="system-container">
                            <p class="system-name">CMS</p>
                            <a href="#" class="system wow" id="system1"></a>
                        </div>
                        <div class="system-container">
                            <p class="system-name">CRM</p>
                            <a href="#" class="system wow" id="system2"></a>
                        </div>
                        <div class="system-container">
                            <p class="system-name">ERP</p>
                            <a href="#" class="system wow" id="system3"></a>
                        </div>
                    </div>
                    <p class="ic-system__title">Control System and Static Websites, with us!</p>
                </div>
            </div>
        </div>
    </div>
    <!-- about end -->

    <!-- heading start -->
    <div class="heading" id="skills">
        <div class="container">
            <div class="heading__icon">
                <img src="../assets/images/cube.png">
            </div>
            <p class="heading__title">print(<i>'Skills'</i>)</p>
            <p class="heading__text">
                Utility classes help you work within the constraints of a system instead of littering your stylesheets with arbitrary values. They make it easy to be consistent with color choices, spacing, typography, shadows, and everything else that makes up a well-engineered design system.
            </p>
        </div>
    </div>
    <!-- heading end -->

    <!-- skills start -->
    <div class="section skills">
        <div class="container">
            <div class="skills-card">
                <img src="../assets/images/skills.png" class="skills-card__img">
                <div class="skills-card__items">
                    <a href="#" class="item">
                        HTML
                    </a>
                    <a href="#" class="item">
                        CSS
                    </a>
                    <a href="#" class="item">
                        JavaScript
                    </a>
                    <a href="#" class="item">
                        PHP
                    </a>
                    <a href="#" class="item">
                        Laravel
                    </a>
                    <a href="#" class="item">
                        Bootstap
                    </a>
                    <a href="#" class="item">
                        Tailwind CSS
                    </a>
                    <a href="#" class="item">
                        SASS
                    </a>
                    <a href="#" class="item">
                        JQuery
                    </a>
                </div>
            </div>
        </div>
    </div>
    <!-- skills end -->

    <!-- heading start -->
    <div class="heading" id="projects">
        <div class="container">
            <div class="heading__icon">
                <img src="../assets/images/code-branch.png">
            </div>
            <p class="heading__title">console.log(<i>'Projects'</i>)</p>
            <p class="heading__text">
                Utility classes help you work within the constraints of a system instead of littering your stylesheets with arbitrary values. They make it easy to be consistent with color choices, spacing, typography, shadows, and everything else that makes up a well-engineered design system.
            </p>
        </div>
    </div>
    <!-- heading end -->

    <!-- projects start -->
    <div class="section projects">
        <div class="container">
            <div class="projects__section">
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
                <a href="#" class="projects__card" data-tilt data-tilt-glare data-tilt-max-glare="0.8">
                    <img src="../assets/images/project.png" class="projects__img">
                </a>
            </div>
            <div class="projects__pagination">
                <div class="pagination">
                    <a href="#" class="page-sliders prev">
                        <svg width="5.000000" height="10.000000" viewBox="0 0 5 10" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                            <path id="Vector" d="M5 0.673828L5 9.32617C5 9.92529 4.36133 10.2253 3.98779 9.80164L0.173584 5.47546C-0.0578613 5.21289 -0.0578613 4.78711 0.173584 4.52454L3.98779 0.198364C4.36133 -0.225342 5 0.074707 5 0.673828Z" fill="#E8E8E8" fill-opacity="1.000000" fill-rule="nonzero"/>
                        </svg>                    
                    </a>
                    <ul class="pages">
                        <li class="page">
                            <a href="#">1</a>
                        </li>
                        <li class="page">
                            <a href="#" class="active">2</a>
                        </li>
                        <li class="page">
                            <a href="#">3</a>
                        </li>
                    </ul>
                    <a href="#" class="page-sliders next">
                        <svg width="5.000000" height="10.000000" viewBox="0 0 5 10" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                            <path id="Vector" d="M0 9.32617L0 0.673828C0 0.074707 0.638672 -0.225342 1.01221 0.198364L4.82642 4.52454C5.05786 4.78711 5.05786 5.21289 4.82642 5.47546L1.01221 9.80164C0.638672 10.2253 0 9.92529 0 9.32617Z" fill="#E8E8E8" fill-opacity="1.000000" fill-rule="nonzero"/>
                        </svg>
                    </a>
                </div>
            </div>
        </div>
    </div>
    <!-- projects end -->

    <!-- heading start -->
    <div class="heading" id="questions">
        <div class="container">
            <div class="heading__icon">
                <img src="../assets/images/development.png">
            </div>
            <p class="heading__title">return <i>'Questions'</i>;</p>
            <p class="heading__text">
                Utility classes help you work within the constraints of a system instead of littering your stylesheets with arbitrary values. They make it easy to be consistent with color choices, spacing, typography, shadows, and everything else that makes up a well-engineered design system.
            </p>
        </div>
    </div>
    <!-- heading end -->

    <!-- questions start -->
    <div class="section questions">
        <div class="container">
            <div class="questions__cards">
                <div class="questions__card">

                </div>
                <div class="qc-unique questions__card">
                    <p class="card__title">Why realise with me?</p>
                    <img src="../assets/images/laptop.png" >
                </div>
            </div>
        </div>
    </div>
    <!-- questions end -->
  </div>
</template>
