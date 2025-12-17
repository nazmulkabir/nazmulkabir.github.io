---
layout: page
title: projects
permalink: /projects/
description:
nav: true
nav_order: 5
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

<div class="row">
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="focus-card h-100">
      <div class="focus-icon">
        <i class="fas fa-shield-alt"></i>
      </div>
      <h4>Cybersecurity & AI Assurance</h4>
      <p>AI-driven security solutions for critical infrastructure and cyber-physical systems</p>
      <div class="focus-projects mb-3">
        <h6 class="text-muted mb-2">Featured Projects:</h6>
        <div class="project-links">
          <a href="{{ site.baseurl }}/projects/2_project/" class="project-link">
            <i class="fas fa-water"></i> DeepH2O
          </a>
          <a href="{{ site.baseurl }}/projects/4_project/" class="project-link">
            <i class="fas fa-shield-alt"></i> MAA Framework
          </a>
        </div>
      </div>
      <div class="focus-technologies">
        <span class="tech-tag">Deep Learning</span>
        <span class="tech-tag">Anomaly Detection</span>
        <span class="tech-tag">HCAE</span>
        <span class="tech-tag">TGCN</span>
      </div>
    </div>
  </div>
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="focus-card h-100">
      <div class="focus-icon">
        <i class="fas fa-water"></i>
      </div>
      <h4>Water Systems Intelligence</h4>
      <p>Smart water distribution and wastewater treatment optimization using AI</p>
      <div class="focus-projects mb-3">
        <h6 class="text-muted mb-2">Featured Projects:</h6>
        <div class="project-links">
          <a href="{{ site.baseurl }}/projects/1_project/" class="project-link">
            <i class="fas fa-chart-line"></i> DC Water
          </a>
          <a href="{{ site.baseurl }}/projects/3_project/" class="project-link">
            <i class="fas fa-tachometer-alt"></i> P2O Dashboard
          </a>
          <a href="{{ site.baseurl }}/projects/6_project/" class="project-link">
            <i class="fas fa-brain"></i> cP2O Context-Aware
          </a>
          <a href="{{ site.baseurl }}/projects/7_project/" class="project-link">
            <i class="fas fa-trophy"></i> IWS Challenge
          </a>
        </div>
      </div>
      <div class="focus-technologies">
        <span class="tech-tag">LSTM</span>
        <span class="tech-tag">Forecasting</span>
        <span class="tech-tag">Time Series</span>
      </div>
    </div>
  </div>
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="focus-card h-100">
      <div class="focus-icon">
        <i class="fas fa-seedling"></i>
      </div>
      <h4>Precision Agriculture</h4>
      <p>AI-driven precision farming and agricultural production optimization</p>
      <div class="focus-projects mb-3">
        <h6 class="text-muted mb-2">Featured Projects:</h6>
        <div class="project-links">
          <a href="{{ site.baseurl }}/projects/5_project/" class="project-link">
            <i class="fas fa-leaf"></i> DeepAg System
          </a>
        </div>
      </div>
      <div class="focus-technologies">
        <span class="tech-tag">Computer Vision</span>
        <span class="tech-tag">IoT Sensors</span>
        <span class="tech-tag">Outlier Detection</span>
      </div>
    </div>
  </div>
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="focus-card h-100">
      <div class="focus-icon">
        <i class="fas fa-exclamation-triangle"></i>
      </div>
      <h4>Anomaly Detection & Assurance</h4>
      <p>Advanced outlier detection methods for ensuring AI system reliability and trustworthiness</p>
      <div class="focus-projects mb-3">
        <h6 class="text-muted mb-2">Cross-Domain Applications:</h6>
        <div class="project-links">
          <a href="{{ site.baseurl }}/projects/4_project/" class="project-link">
            <i class="fas fa-check-circle"></i> Model Agnostic Methods
          </a>
          <a href="{{ site.baseurl }}/projects/2_project/" class="project-link">
            <i class="fas fa-water"></i> Water System Detection
          </a>
          <a href="{{ site.baseurl }}/projects/5_project/" class="project-link">
            <i class="fas fa-seedling"></i> Agricultural Outliers
          </a>
        </div>
      </div>
      <div class="focus-technologies">
        <span class="tech-tag">Machine Learning</span>
        <span class="tech-tag">Pattern Recognition</span>
        <span class="tech-tag">AI Assurance</span>
      </div>
    </div>
  </div>
</div>

</div>

<style>
/* Projects Page Enhanced Styling */

/* Simple, clean project sections - no complex hiding */
.simple-project-section {
  margin-bottom: 3rem;
  padding: 1rem 0;
}

.simple-category-header {
  font-size: 2rem;
  font-weight: 700;
  color: var(--global-text-color);
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 3px solid transparent;
  border-image: linear-gradient(90deg, var(--global-theme-color) 0%, #764ba2 100%) 1;
}

.simple-category-description {
  max-width: 800px;
}

.simple-category-description .lead {
  font-size: 1.1rem;
  color: #6c757d;
  line-height: 1.7;
}

/* Hero Section */
.projects-hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 4rem 2rem;
  border-radius: 1rem;
  margin-bottom: 3rem;
  position: relative;
  overflow: hidden;
}

.projects-hero-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grid" width="10" height="10" patternUnits="userSpaceOnUse"><path d="M 10 0 L 0 0 0 10" fill="none" stroke="rgba(255,255,255,0.1)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23grid)"/></svg>');
  opacity: 0.3;
}

.hero-content {
  position: relative;
  z-index: 2;
}

.hero-title {
  font-size: 3rem;
  font-weight: 800;
  margin-bottom: 1rem;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.hero-subtitle {
  font-size: 1.3rem;
  opacity: 0.95;
  max-width: 800px;
  margin: 0 auto 2rem;
  line-height: 1.6;
}

.stat-card {
  background: rgba(255,255,255,0.1);
  padding: 1.5rem;
  border-radius: 1rem;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
  transition: all 0.3s ease;
  position: relative;
}

.stat-card.clickable {
  cursor: pointer;
}

.stat-card.clickable:hover {
  transform: translateY(-8px);
  background: rgba(255,255,255,0.2);
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

.stat-card:hover {
  transform: translateY(-5px);
  background: rgba(255,255,255,0.15);
}

.stat-arrow {
  position: absolute;
  bottom: 0.5rem;
  right: 0.75rem;
  font-size: 0.75rem;
  opacity: 0.7;
  transition: opacity 0.3s ease;
}

.stat-card.clickable:hover .stat-arrow {
  opacity: 1;
}

.stat-number {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
  color: #fff;
}

.stat-label {
  margin: 0;
  opacity: 0.9;
  font-weight: 600;
}

/* Research Focus Section */
.research-focus-section {
  padding: 2rem 0;
}

.section-title {
  font-size: 2.5rem;
  font-weight: 700;
  color: var(--global-text-color);
  margin-bottom: 3rem;
}

.focus-card {
  background: var(--global-card-bg-color);
  padding: 2rem;
  border-radius: 1rem;
  text-align: center;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  border: 1px solid var(--global-divider-color);
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  overflow: hidden;
}

.focus-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, #667eea 0%, #764ba2 100%);
  transform: scaleX(0);
  transition: transform 0.3s ease;
}

.focus-card:hover::before {
  transform: scaleX(1);
}

.focus-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 40px rgba(0,0,0,0.15);
}

.focus-icon {
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 1.5rem;
  font-size: 2rem;
  color: white;
  transition: all 0.3s ease;
}

.focus-card:hover .focus-icon {
  transform: scale(1.1) rotate(5deg);
}

.focus-card h4 {
  font-size: 1.4rem;
  font-weight: 700;
  margin-bottom: 1rem;
  color: #2c3e50;
}

.focus-card p {
  color: #6c757d;
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.focus-technologies {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tech-tag {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.3rem 0.8rem;
  border-radius: 1rem;
  font-size: 0.8rem;
  font-weight: 600;
  transition: all 0.3s ease;
}

.tech-tag:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
}

/* Focus Projects Links */
.focus-projects {
  margin-bottom: 1rem;
  text-align: left;
}

.focus-projects h6 {
  font-size: 0.85rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: #495057;
}

.project-links {
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}

.project-link {
  display: flex;
  align-items: center;
  padding: 0.4rem 0.6rem;
  background: rgba(102, 126, 234, 0.1);
  border-radius: 8px;
  text-decoration: none;
  color: #667eea;
  font-size: 0.8rem;
  font-weight: 500;
  transition: all 0.3s ease;
  border-left: 3px solid #667eea;
}

.project-link:hover {
  background: rgba(102, 126, 234, 0.2);
  color: #4a5eb8;
  text-decoration: none;
  transform: translateX(3px);
}

.project-link i {
  margin-right: 0.5rem;
  font-size: 0.9rem;
}

/* Project Controls */
.project-controls-section {
  background: var(--global-card-bg-color);
  padding: 2rem;
  border-radius: 1rem;
  border: 1px solid var(--global-divider-color);
}

.controls-container {
  max-width: 800px;
  margin: 0 auto;
}

.search-container {
  position: relative;
}

.search-icon {
  position: absolute;
  left: 1rem;
  top: 50%;
  transform: translateY(-50%);
  color: #6c757d;
  z-index: 5;
}

.search-input {
  padding-left: 3rem;
  border-radius: 2rem;
  border: 2px solid #e9ecef;
  font-size: 1rem;
  transition: all 0.3s ease;
}

.search-input:focus {
  border-color: #667eea;
  box-shadow: 0 0 0 0.2rem rgba(102, 126, 234, 0.25);
}

.filter-select {
  border-radius: 2rem;
  border: 2px solid #e9ecef;
  font-size: 1rem;
  transition: all 0.3s ease;
}

.filter-select:focus {
  border-color: #667eea;
  box-shadow: 0 0 0 0.2rem rgba(102, 126, 234, 0.25);
}

/* Category Headers */
.project-category-section {
  margin-bottom: 3rem;
  min-height: 200px;
  padding: 1rem 0;
}

.category-header {
  font-size: 2rem;
  font-weight: 700;
  color: var(--global-text-color);
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 3px solid transparent;
  border-image: linear-gradient(90deg, var(--global-theme-color) 0%, #764ba2 100%) 1;
  display: block;
  width: 100%;
}

.category-description {
  max-width: 800px;
}

.category-description .lead {
  font-size: 1.1rem;
  color: #6c757d;
  line-height: 1.7;
}

/* Project Cards Enhancement */
.row .col {
  margin-bottom: 2rem;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-title {
    font-size: 2rem;
  }
  
  .hero-subtitle {
    font-size: 1.1rem;
  }
  
  .section-title {
    font-size: 2rem;
  }
  
  .focus-card {
    padding: 1.5rem;
  }
  
  .focus-icon {
    width: 60px;
    height: 60px;
    font-size: 1.5rem;
  }
  
  .project-controls-section {
    padding: 1.5rem;
  }
}


/* Compact GitHub section */
.github-compact-section {
  background: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 1rem;
  padding: 1.25rem;
}

.github-compact-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.75rem;
}

@media (max-width: 1200px) {
  .github-compact-grid { grid-template-columns: repeat(3, 1fr); }
}
@media (max-width: 768px) {
  .github-compact-grid { grid-template-columns: repeat(2, 1fr); }
}
@media (max-width: 480px) {
  .github-compact-grid { grid-template-columns: 1fr; }
}

/* Tighten repo include images inside this page */
.github-compact-section .repo {
  padding: 0.25rem !important;
}
.github-compact-section .repo-img-light,
.github-compact-section .repo-img-dark {
  border-radius: 0.5rem;
  border: 1px solid #eef1f4;
  box-shadow: 0 2px 10px rgba(0,0,0,0.04);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}
.github-compact-section a:hover .repo-img-light,
.github-compact-section a:hover .repo-img-dark {
  transform: translateY(-3px);
  box-shadow: 0 8px 18px rgba(0,0,0,0.08);
}
</style>

<script>
// Simple smooth scroll - no filtering or animations
document.addEventListener('DOMContentLoaded', function() {
  // Smooth scroll for anchor links
  document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
      const targetSelector = this.getAttribute('href');
      if (!targetSelector || targetSelector === '#') {
        return;
      }

      e.preventDefault();
      const target = document.querySelector(targetSelector);
      if (target) {
        target.scrollIntoView({
          behavior: 'smooth',
          block: 'start'
        });
      }
    });
  });

  // Stats card navigation
  document.querySelectorAll('.stat-card.clickable').forEach(card => {
    card.addEventListener('click', function() {
      const target = this.dataset.target || '';

      if (target.startsWith('/')) {
        window.location.href = target;
        return;
      }

      const targetElement = document.getElementById(target);
      if (targetElement) {
        targetElement.scrollIntoView({
          behavior: 'smooth',
          block: 'start'
        });
      }
    });
  });
});
</script>
