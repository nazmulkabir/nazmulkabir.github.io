---
layout: page
permalink: /resources/
title: resources
description: Curated collection of tools, datasets, and learning materials for AI research and cybersecurity
nav: true
nav_order: 7
---

<div class="resources-header">
  <div class="header-content">
    <h1>Research Resources</h1>
    <p>Curated tools, datasets, and learning materials for AI research and cybersecurity</p>
    <div class="resource-stats">
      <span class="stat"><strong>50+</strong> Tools</span>
      <span class="stat"><strong>25+</strong> Datasets</span>
      <span class="stat"><strong>30+</strong> Learning Resources</span>
    </div>
  </div>
</div>

<!-- Animated News Section -->
<div class="animated-news-section">
  <div class="news-header">
    <h2><i class="fas fa-newspaper"></i> Latest Research News</h2>
    <p>Stay updated with the latest developments in AI research and cybersecurity</p>
  </div>
  
  <div class="news-carousel-container">
    <div class="news-carousel">
      <!-- News Item 1 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/ai-breakthrough.jpg' | relative_url }}" alt="AI Breakthrough" onerror="this.src='https://via.placeholder.com/300x200/3498db/white?text=AI+Research'">
        </div>
        <div class="news-content">
          <span class="news-date">October 10, 2025</span>
          <h4>Revolutionary AI Model Achieves 99% Accuracy in Cybersecurity Threat Detection</h4>
          <p>New deep learning architecture shows unprecedented performance in identifying sophisticated cyber attacks...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      
      <!-- News Item 2 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/water-systems.jpg' | relative_url }}" alt="Water Systems Security" onerror="this.src='https://via.placeholder.com/300x200/2ecc71/white?text=Water+Security'">
        </div>
        <div class="news-content">
          <span class="news-date">October 8, 2025</span>
          <h4>Smart Water Systems Defense: ML-Powered Anomaly Detection Framework</h4>
          <p>Our latest research introduces an innovative machine learning approach for protecting critical water infrastructure...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      
      <!-- News Item 3 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/agriculture-ai.jpg' | relative_url }}" alt="Agriculture AI" onerror="this.src='https://via.placeholder.com/300x200/f39c12/white?text=AgriTech+AI'">
        </div>
        <div class="news-content">
          <span class="news-date">October 5, 2025</span>
          <h4>Precision Agriculture: AI-Driven Crop Monitoring System Launches</h4>
          <p>Breakthrough IoT and machine learning integration for real-time agricultural monitoring and optimization...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      
      <!-- News Item 4 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/conference.jpg' | relative_url }}" alt="Research Conference" onerror="this.src='https://via.placeholder.com/300x200/9b59b6/white?text=Conference+2025'">
        </div>
        <div class="news-content">
          <span class="news-date">October 1, 2025</span>
          <h4>International Cybersecurity Conference 2025: Keynote Presentation</h4>
          <p>Presenting cutting-edge research on explainable AI for cybersecurity at the prestigious international conference...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      
      <!-- News Item 5 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/publication.jpg' | relative_url }}" alt="Research Publication" onerror="this.src='https://via.placeholder.com/300x200/e74c3c/white?text=Publication'">
        </div>
        <div class="news-content">
          <span class="news-date">September 28, 2025</span>
          <h4>New Research Paper Published in IEEE Transactions on Cybersecurity</h4>
          <p>Latest work on adaptive machine learning for dynamic threat detection accepted in top-tier journal...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
      
      <!-- News Item 6 -->
      <div class="news-item">
        <div class="news-thumbnail">
          <img src="{{ '/assets/img/news/collaboration.jpg' | relative_url }}" alt="Research Collaboration" onerror="this.src='https://via.placeholder.com/300x200/34495e/white?text=Collaboration'">
        </div>
        <div class="news-content">
          <span class="news-date">September 25, 2025</span>
          <h4>New Research Collaboration with Leading Tech Companies Announced</h4>
          <p>Exciting partnership to develop next-generation AI security solutions for critical infrastructure protection...</p>
          <a href="#" class="news-link">Read More <i class="fas fa-arrow-right"></i></a>
        </div>
      </div>
    </div>
    
    <!-- Navigation Controls -->
    <div class="news-controls">
      <button class="news-control prev" onclick="moveCarousel(-1)">
        <i class="fas fa-chevron-left"></i>
      </button>
      <button class="news-control next" onclick="moveCarousel(1)">
        <i class="fas fa-chevron-right"></i>
      </button>
    </div>
    
    <!-- Progress Indicators -->
    <div class="news-indicators">
      <span class="indicator active" onclick="goToSlide(0)"></span>
      <span class="indicator" onclick="goToSlide(1)"></span>
      <span class="indicator" onclick="goToSlide(2)"></span>
      <span class="indicator" onclick="goToSlide(3)"></span>
      <span class="indicator" onclick="goToSlide(4)"></span>
      <span class="indicator" onclick="goToSlide(5)"></span>
    </div>
  </div>
</div>

<div class="resources-container">
  
  <!-- Quick Navigation -->
  <div class="resource-nav">
    <a href="#ml-tools" class="nav-link"><i class="fas fa-brain"></i> ML Tools</a>
    <a href="#cybersecurity" class="nav-link"><i class="fas fa-shield-alt"></i> Security Tools</a>
    <a href="#datasets" class="nav-link"><i class="fas fa-database"></i> Datasets</a>
    <a href="#learning" class="nav-link"><i class="fas fa-graduation-cap"></i> Learning</a>
    <a href="#development" class="nav-link"><i class="fas fa-code"></i> Development</a>
  </div>

  <!-- Machine Learning Tools -->
  <div id="ml-tools" class="resource-section">
    <h2><i class="fas fa-brain"></i> Machine Learning & AI</h2>
    
    <div class="tool-grid">
      <div class="tool-item">
        <div class="tool-header">
          <i class="fab fa-python"></i>
          <h4>PyTorch</h4>
        </div>
        <p>Deep learning framework for research and production</p>
        <div class="tool-tags">
          <span class="tag">Deep Learning</span>
          <span class="tag">Research</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-code"></i>
          <h4>TensorFlow</h4>
        </div>
        <p>End-to-end machine learning platform</p>
        <div class="tool-tags">
          <span class="tag">Production</span>
          <span class="tag">Scalable</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-chart-line"></i>
          <h4>Scikit-learn</h4>
        </div>
        <p>Machine learning library for Python</p>
        <div class="tool-tags">
          <span class="tag">Classical ML</span>
          <span class="tag">Python</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-sync"></i>
          <h4>XGBoost</h4>
        </div>
        <p>Gradient boosting framework</p>
        <div class="tool-tags">
          <span class="tag">Boosting</span>
          <span class="tag">Tabular</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-search"></i>
          <h4>SHAP</h4>
        </div>
        <p>Explainable AI and model interpretation</p>
        <div class="tool-tags">
          <span class="tag">Explainability</span>
          <span class="tag">Interpretability</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-flask"></i>
          <h4>MLflow</h4>
        </div>
        <p>ML lifecycle management platform</p>
        <div class="tool-tags">
          <span class="tag">MLOps</span>
          <span class="tag">Tracking</span>
        </div>
      </div>
    </div>
  </div>

  <!-- Cybersecurity Tools -->
  <div id="cybersecurity" class="resource-section">
    <h2><i class="fas fa-shield-alt"></i> Cybersecurity & Network Analysis</h2>
    
    <div class="tool-grid">
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-network-wired"></i>
          <h4>Wireshark</h4>
        </div>
        <p>Network protocol analyzer and packet capture</p>
        <div class="tool-tags">
          <span class="tag">Network Analysis</span>
          <span class="tag">Packet Capture</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-bug"></i>
          <h4>Metasploit</h4>
        </div>
        <p>Penetration testing framework</p>
        <div class="tool-tags">
          <span class="tag">Penetration Testing</span>
          <span class="tag">Exploitation</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-eye"></i>
          <h4>Suricata</h4>
        </div>
        <p>High performance IDS/IPS and security monitoring</p>
        <div class="tool-tags">
          <span class="tag">IDS/IPS</span>
          <span class="tag">Monitoring</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-search-plus"></i>
          <h4>Nessus</h4>
        </div>
        <p>Vulnerability assessment scanner</p>
        <div class="tool-tags">
          <span class="tag">Vulnerability</span>
          <span class="tag">Assessment</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-sitemap"></i>
          <h4>MITRE ATT&CK</h4>
        </div>
        <p>Adversarial tactics and techniques framework</p>
        <div class="tool-tags">
          <span class="tag">Framework</span>
          <span class="tag">Threat Intelligence</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-terminal"></i>
          <h4>Splunk</h4>
        </div>
        <p>SIEM and security analytics platform</p>
        <div class="tool-tags">
          <span class="tag">SIEM</span>
          <span class="tag">Analytics</span>
        </div>
      </div>
    </div>
  </div>
  
  <!-- Datasets -->
  <div id="datasets" class="resource-section">
    <h2><i class="fas fa-database"></i> Research Datasets</h2>
    
    <div class="tool-grid">
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-globe"></i>
          <h4>KDD Cup 1999</h4>
        </div>
        <p>Network intrusion detection benchmark dataset</p>
        <div class="tool-tags">
          <span class="tag">Network Security</span>
          <span class="tag">Benchmark</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-shield-alt"></i>
          <h4>NSL-KDD</h4>
        </div>
        <p>Improved version of KDD Cup dataset</p>
        <div class="tool-tags">
          <span class="tag">IDS</span>
          <span class="tag">Anomaly Detection</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-water"></i>
          <h4>BATADAL</h4>
        </div>
        <p>Water distribution system attack detection dataset</p>
        <div class="tool-tags">
          <span class="tag">Water Systems</span>
          <span class="tag">Cyber-Physical</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-industry"></i>
          <h4>SWaT</h4>
        </div>
        <p>Secure Water Treatment testbed dataset</p>
        <div class="tool-tags">
          <span class="tag">Industrial Control</span>
          <span class="tag">SCADA</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-leaf"></i>
          <h4>PlantVillage</h4>
        </div>
        <p>Plant disease detection image dataset</p>
        <div class="tool-tags">
          <span class="tag">Agriculture</span>
          <span class="tag">Computer Vision</span>
        </div>
      </div>
      
      <div class="tool-item">
        <div class="tool-header">
          <i class="fas fa-satellite"></i>
          <h4>Crop Monitoring</h4>
        </div>
        <p>Satellite imagery for precision agriculture</p>
        <div class="tool-tags">
          <span class="tag">Remote Sensing</span>
          <span class="tag">Agriculture</span>
        </div>
      </div>
    </div>
  </div>

  <!-- Learning Resources -->
  <div class="resource-category">
    <div class="category-header">
      <h2><i class="fas fa-graduation-cap"></i> Learning Resources</h2>
      <p>Educational materials, courses, and books for advancing research skills</p>
    </div>
    
    <div class="resource-grid">
      <div class="resource-card featured">
        <div class="resource-icon">
          <i class="fas fa-book"></i>
        </div>
        <div class="resource-content">
          <h4>Hands-On Machine Learning</h4>
          <p>Comprehensive guide by Aurélien Géron covering practical ML techniques and implementation.</p>
          <div class="resource-tags">
            <span class="tag book">Book</span>
            <span class="tag practical">Practical</span>
          </div>
          <div class="resource-links">
            <a href="https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> O'Reilly
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-video"></i>
        </div>
        <div class="resource-content">
          <h4>Andrew Ng's ML Course</h4>
          <p>Foundational machine learning course covering essential algorithms and mathematical foundations.</p>
          <div class="resource-tags">
            <span class="tag course">Online Course</span>
            <span class="tag foundations">Foundations</span>
          </div>
          <div class="resource-links">
            <a href="https://www.coursera.org/learn/machine-learning" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> Coursera
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-shield-alt"></i>
        </div>
        <div class="resource-content">
          <h4>Cybersecurity Fundamentals</h4>
          <p>SANS Institute resources for cybersecurity professionals and researchers.</p>
          <div class="resource-tags">
            <span class="tag cybersecurity">Cybersecurity</span>
            <span class="tag certification">Certification</span>
          </div>
          <div class="resource-links">
            <a href="https://www.sans.org/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> SANS
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-brain"></i>
        </div>
        <div class="resource-content">
          <h4>Deep Learning Specialization</h4>
          <p>Comprehensive deep learning course series covering neural networks, CNNs, RNNs, and more.</p>
          <div class="resource-tags">
            <span class="tag deep-learning">Deep Learning</span>
            <span class="tag specialization">Specialization</span>
          </div>
          <div class="resource-links">
            <a href="https://www.coursera.org/specializations/deep-learning" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> Coursera
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-journal-whills"></i>
        </div>
        <div class="resource-content">
          <h4>Arxiv Papers</h4>
          <p>Latest research papers in AI, ML, and cybersecurity from the leading preprint repository.</p>
          <div class="resource-tags">
            <span class="tag papers">Research Papers</span>
            <span class="tag latest">Latest Research</span>
          </div>
          <div class="resource-links">
            <a href="https://arxiv.org/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> ArXiv
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-code"></i>
        </div>
        <div class="resource-content">
          <h4>GitHub ML Projects</h4>
          <p>Curated collection of open-source machine learning and cybersecurity projects.</p>
          <div class="resource-tags">
            <span class="tag opensource">Open Source</span>
            <span class="tag projects">Projects</span>
          </div>
          <div class="resource-links">
            <a href="https://github.com/topics/machine-learning" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> GitHub
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Development Tools -->
  <div id="development" class="resource-category">
    <div class="category-header">
      <h2><i class="fas fa-code"></i> Development & Deployment</h2>
      <p>Essential tools for research development, experimentation, and deployment</p>
    </div>
    
    <div class="resource-grid">
      <div class="resource-card featured">
        <div class="resource-icon">
          <i class="fab fa-docker"></i>
        </div>
        <div class="resource-content">
          <h4>Docker</h4>
          <p>Containerization platform for reproducible research environments and scalable deployments.</p>
          <div class="resource-tags">
            <span class="tag containerization">Containerization</span>
            <span class="tag deployment">Deployment</span>
          </div>
          <div class="resource-links">
            <a href="https://www.docker.com/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> Official Site
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-book-open"></i>
        </div>
        <div class="resource-content">
          <h4>Jupyter Lab</h4>
          <p>Interactive development environment for data science and machine learning research.</p>
          <div class="resource-tags">
            <span class="tag notebook">Notebooks</span>
            <span class="tag interactive">Interactive</span>
          </div>
          <div class="resource-links">
            <a href="https://jupyter.org/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> Jupyter
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fab fa-git-alt"></i>
        </div>
        <div class="resource-content">
          <h4>Git & GitHub</h4>
          <p>Version control system and collaborative platform for research code and reproducibility.</p>
          <div class="resource-tags">
            <span class="tag version-control">Version Control</span>
            <span class="tag collaboration">Collaboration</span>
          </div>
          <div class="resource-links">
            <a href="https://github.com/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> GitHub
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-cloud"></i>
        </div>
        <div class="resource-content">
          <h4>AWS</h4>
          <p>Cloud computing platform for scalable ML model training and deployment.</p>
          <div class="resource-tags">
            <span class="tag cloud">Cloud Computing</span>
            <span class="tag scalable">Scalable</span>
          </div>
          <div class="resource-links">
            <a href="https://aws.amazon.com/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> AWS
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-terminal"></i>
        </div>
        <div class="resource-content">
          <h4>VS Code</h4>
          <p>Powerful code editor with excellent support for Python, R, and research workflows.</p>
          <div class="resource-tags">
            <span class="tag editor">Code Editor</span>
            <span class="tag research">Research</span>
          </div>
          <div class="resource-links">
            <a href="https://code.visualstudio.com/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> VS Code
            </a>
          </div>
        </div>
      </div>
      
      <div class="resource-card">
        <div class="resource-icon">
          <i class="fas fa-chart-bar"></i>
        </div>
        <div class="resource-content">
          <h4>Weights & Biases</h4>
          <p>Experiment tracking and model management platform for ML research and development.</p>
          <div class="resource-tags">
            <span class="tag tracking">Experiment Tracking</span>
            <span class="tag mlops">MLOps</span>
          </div>
          <div class="resource-links">
            <a href="https://wandb.ai/" target="_blank" class="btn-link">
              <i class="fas fa-external-link-alt"></i> W&B
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="contribution-section">
  <div class="contribution-content">
    <h2><i class="fas fa-plus-circle text-primary"></i> Contribute to Resources</h2>
    <p>Found a useful tool, dataset, or resource that should be included? I'm always looking to expand this collection with high-quality resources for the research community.</p>
    <div class="contribution-actions">
      <a href="mailto:nazmul@vt.edu" class="btn btn-primary">
        <i class="fas fa-envelope"></i> Suggest a Resource
      </a>
      <a href="https://github.com/nazmulkabir" target="_blank" class="btn btn-outline">
        <i class="fab fa-github"></i> View on GitHub
      </a>
    </div>
  </div>
</div>

<style>
/* Animated News Section Styling */
.animated-news-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 4rem 2rem;
  margin: 2rem 0 4rem;
  border-radius: 1rem;
  position: relative;
  overflow: hidden;
}

.animated-news-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="newsgrid" width="20" height="20" patternUnits="userSpaceOnUse"><path d="M 20 0 L 0 0 0 20" fill="none" stroke="rgba(255,255,255,0.05)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23newsgrid)"/></svg>');
  opacity: 0.3;
}

.news-header {
  text-align: center;
  margin-bottom: 3rem;
  position: relative;
  z-index: 2;
}

.news-header h2 {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 1rem;
  color: white;
}

.news-header p {
  font-size: 1.2rem;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto;
}

.news-carousel-container {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
  z-index: 2;
}

.news-carousel {
  display: flex;
  transition: transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  gap: 2rem;
}

.news-item {
  flex: 0 0 350px;
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  border-radius: 1rem;
  overflow: hidden;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
  transition: all 0.4s ease;
  color: #2c3e50;
}

.news-item:hover {
  transform: translateY(-10px) scale(1.02);
  box-shadow: 0 16px 48px rgba(0, 0, 0, 0.3);
}

.news-thumbnail {
  width: 100%;
  height: 200px;
  overflow: hidden;
  position: relative;
}

.news-thumbnail img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.4s ease;
}

.news-item:hover .news-thumbnail img {
  transform: scale(1.1);
}

.news-content {
  padding: 1.5rem;
}

.news-date {
  display: inline-block;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.3rem 0.8rem;
  border-radius: 1rem;
  font-size: 0.8rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.news-content h4 {
  font-size: 1.2rem;
  font-weight: 700;
  line-height: 1.4;
  margin-bottom: 0.8rem;
  color: #2c3e50;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.news-content p {
  color: #6c757d;
  font-size: 0.9rem;
  line-height: 1.6;
  margin-bottom: 1rem;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.news-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  color: #667eea;
  text-decoration: none;
  font-weight: 600;
  font-size: 0.9rem;
  transition: all 0.3s ease;
}

.news-link:hover {
  color: #764ba2;
  transform: translateX(5px);
  text-decoration: none;
}

/* Navigation Controls */
.news-controls {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 100%;
  display: flex;
  justify-content: space-between;
  pointer-events: none;
  z-index: 3;
}

.news-control {
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(10px);
  border: none;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #667eea;
  font-size: 1.2rem;
  cursor: pointer;
  transition: all 0.3s ease;
  pointer-events: auto;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
}

.news-control:hover {
  background: white;
  transform: scale(1.1);
  color: #764ba2;
}

.news-control.prev {
  margin-left: -25px;
}

.news-control.next {
  margin-right: -25px;
}

/* Progress Indicators */
.news-indicators {
  display: flex;
  justify-content: center;
  gap: 0.8rem;
  margin-top: 2rem;
  z-index: 2;
  position: relative;
}

.indicator {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.4);
  cursor: pointer;
  transition: all 0.3s ease;
}

.indicator.active,
.indicator:hover {
  background: white;
  transform: scale(1.2);
}

/* Animation Classes */
@keyframes slideInRight {
  from {
    opacity: 0;
    transform: translateX(100px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-100px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.news-item.slide-in-right {
  animation: slideInRight 0.6s ease-out;
}

.news-item.slide-in-left {
  animation: slideInLeft 0.6s ease-out;
}

/* Responsive Design for News Section */
@media (max-width: 768px) {
  .animated-news-section {
    padding: 2rem 1rem;
    margin: 1rem 0 2rem;
  }
  
  .news-header h2 {
    font-size: 2rem;
  }
  
  .news-header p {
    font-size: 1rem;
  }
  
  .news-item {
    flex: 0 0 280px;
  }
  
  .news-content {
    padding: 1rem;
  }
  
  .news-content h4 {
    font-size: 1.1rem;
  }
  
  .news-controls {
    display: none;
  }
  
  .news-carousel {
    overflow-x: auto;
    scroll-snap-type: x mandatory;
    -webkit-overflow-scrolling: touch;
    scrollbar-width: none;
    -ms-overflow-style: none;
  }
  
  .news-carousel::-webkit-scrollbar {
    display: none;
  }
  
  .news-item {
    scroll-snap-align: start;
  }
}

@media (max-width: 480px) {
  .news-item {
    flex: 0 0 250px;
  }
  
  .news-thumbnail {
    height: 150px;
  }
  
  .news-header h2 {
    font-size: 1.7rem;
  }
}

/* Professional Resources Page Styling */
.resources-header {
  background: linear-gradient(135deg, #34495e 0%, #2c3e50 100%);
  color: white;
  padding: 2.5rem 2rem;
  border-radius: 12px;
  margin-bottom: 2rem;
  text-align: center;
}

.header-content h1 {
  font-size: 2rem;
  font-weight: 700;
  margin: 0 0 0.5rem 0;
}

.header-content p {
  font-size: 1.1rem;
  margin: 0 0 1rem 0;
  opacity: 0.9;
}

.resource-stats {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.stat {
  font-size: 0.9rem;
  opacity: 0.8;
}

.resources-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

/* Navigation */
.resource-nav {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-bottom: 2rem;
  padding: 1rem;
  background: var(--global-card-bg-color);
  border-radius: 10px;
  flex-wrap: wrap;
}

.nav-link {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  background: white;
  color: #2c3e50;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 500;
  transition: all 0.3s ease;
  border: 1px solid #e9ecef;
  font-size: 0.9rem;
}

.nav-link:hover {
  background: #3498db;
  color: white;
  text-decoration: none;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(52, 152, 219, 0.3);
}

/* Resource Sections */
.resource-section {
  margin-bottom: 3rem;
}

.resource-section h2 {
  font-size: 1.5rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e9ecef;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.resource-section h2 i {
  color: #3498db;
  font-size: 1.3rem;
}

/* Tool Grid */
.tool-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1rem;
}

.tool-item {
  background: white;
  padding: 1.25rem;
  border-radius: 10px;
  border: 1px solid #e9ecef;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  transition: all 0.3s ease;
}

.tool-item:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}

.tool-header {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  margin-bottom: 0.75rem;
}

.tool-header i {
  font-size: 1.5rem;
  color: #3498db;
  width: 24px;
  text-align: center;
}

.tool-header h4 {
  font-size: 1.1rem;
  font-weight: 600;
  color: #2c3e50;
  margin: 0;
}

.tool-item p {
  font-size: 0.9rem;
  color: #6c757d;
  margin: 0 0 1rem 0;
  line-height: 1.5;
}

.tool-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
}

.tag {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
  padding: 0.2rem 0.6rem;
  border-radius: 15px;
  font-size: 0.75rem;
  font-weight: 500;
  white-space: nowrap;
}

/* Resource Categories (for learning and development sections) */
.resource-category {
  margin-bottom: 4rem;
}

.category-header {
  text-align: center;
  margin-bottom: 3rem;
}

.category-header h2 {
  font-size: 2rem;
  font-weight: 700;
  color: #2c3e50;
  margin-bottom: 1rem;
}

.category-header p {
  font-size: 1.1rem;
  color: #6c757d;
  max-width: 600px;
  margin: 0 auto;
}

.resource-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.resource-card {
  background: white;
  border-radius: 1rem;
  padding: 2rem;
  box-shadow: 0 4px 15px rgba(0,0,0,0.08);
  border: 1px solid rgba(0,0,0,0.05);
  transition: all 0.3s ease;
  position: relative;
}

.resource-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 30px rgba(0,0,0,0.15);
}

.resource-card.featured {
  border-left: 4px solid #3498db;
}

.resource-card.featured::before {
  content: 'Featured';
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
  padding: 0.3rem 0.8rem;
  border-radius: 1rem;
  font-size: 0.8rem;
  font-weight: 600;
}

.resource-icon {
  width: 60px;
  height: 60px;
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  border-radius: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 1.8rem;
  margin-bottom: 1.5rem;
}

.resource-content h4 {
  font-size: 1.4rem;
  font-weight: 700;
  color: #2c3e50;
  margin-bottom: 1rem;
}

.resource-content p {
  color: #6c757d;
  line-height: 1.6;
  margin-bottom: 1.5rem;
}

.resource-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.8rem;
  margin-bottom: 1.5rem;
}

.resource-links {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.btn-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  background: #f8f9fa;
  color: #3498db;
  text-decoration: none;
  border-radius: 0.5rem;
  font-size: 0.9rem;
  font-weight: 600;
  transition: all 0.3s ease;
  border: 1px solid #e9ecef;
}

.btn-link:hover {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
  transform: translateY(-2px);
  text-decoration: none;
}

/* Contribution Section */
.contribution-section {
  background: white;
  padding: 4rem 2rem;
  border-radius: 1rem;
  text-align: center;
  margin-top: 4rem;
  border: 1px solid #e9ecef;
  box-shadow: 0 4px 15px rgba(0,0,0,0.08);
}

.contribution-content h2 {
  font-size: 2rem;
  font-weight: 700;
  color: #2c3e50;
  margin-bottom: 1rem;
}

.contribution-content p {
  font-size: 1.1rem;
  color: #6c757d;
  max-width: 600px;
  margin: 0 auto 2rem;
}

.contribution-actions {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 1rem 2rem;
  border-radius: 0.8rem;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.3s ease;
  border: 2px solid transparent;
}

.btn-primary {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
}

.btn-primary:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(52, 152, 219, 0.3);
  text-decoration: none;
  color: white;
}

.btn-outline {
  background: transparent;
  color: #3498db;
  border-color: #3498db;
}

.btn-outline:hover {
  background: #3498db;
  color: white;
  transform: translateY(-3px);
  text-decoration: none;
}

/* Responsive Design */
@media (max-width: 768px) {
  .resources-header {
    padding: 2rem 1.5rem;
  }
  
  .header-content h1 {
    font-size: 1.7rem;
  }
  
  .resource-stats {
    gap: 1rem;
  }
  
  .resource-nav {
    gap: 0.5rem;
  }
  
  .nav-link {
    font-size: 0.8rem;
    padding: 0.4rem 0.8rem;
  }
  
  .tool-grid, .resource-grid {
    grid-template-columns: 1fr;
  }
  
  .tool-item, .resource-card {
    padding: 1rem;
  }
  
  .category-header h2 {
    font-size: 1.7rem;
  }
  
  .contribution-actions {
    flex-direction: column;
    align-items: center;
  }
  
  .btn {
    width: 100%;
    max-width: 300px;
  }
}

@media (max-width: 480px) {
  .header-content h1 {
    font-size: 1.5rem;
  }
  
  .resource-nav {
    flex-direction: column;
    align-items: center;
  }
  
  .nav-link {
    width: 100%;
    justify-content: center;
  }
  
  .category-header h2 {
    font-size: 1.5rem;
  }
}
</style>

<script>
// Animated News Carousel Functionality
class NewsCarousel {
  constructor() {
    this.carousel = document.querySelector('.news-carousel');
    this.items = document.querySelectorAll('.news-item');
    this.indicators = document.querySelectorAll('.indicator');
    this.totalItems = this.items.length;
    this.currentIndex = 0;
    this.itemWidth = 350; // Width of each news item + gap
    this.itemsPerView = this.getItemsPerView();
    this.isAnimating = false;
    this.autoPlayInterval = null;
    
    this.init();
  }
  
  init() {
    if (!this.carousel || this.totalItems === 0) return;
    
    // Set initial position
    this.updateCarouselPosition();
    
    // Start auto-play
    this.startAutoPlay();
    
    // Pause auto-play on hover
    this.carousel.parentElement.addEventListener('mouseenter', () => {
      this.stopAutoPlay();
    });
    
    this.carousel.parentElement.addEventListener('mouseleave', () => {
      this.startAutoPlay();
    });
    
    // Handle window resize
    window.addEventListener('resize', () => {
      this.itemsPerView = this.getItemsPerView();
      this.updateCarouselPosition();
    });
    
    // Touch/swipe support for mobile
    this.addTouchSupport();
  }
  
  getItemsPerView() {
    const containerWidth = this.carousel.parentElement.offsetWidth;
    if (containerWidth < 480) return 1;
    if (containerWidth < 768) return 1.2;
    if (containerWidth < 1024) return 2;
    return 3;
  }
  
  updateCarouselPosition(animate = true) {
    if (!this.carousel) return;
    
    const maxIndex = Math.max(0, this.totalItems - Math.floor(this.itemsPerView));
    this.currentIndex = Math.min(this.currentIndex, maxIndex);
    
    const translateX = -(this.currentIndex * (this.itemWidth + 32)); // 32px for gap
    
    if (animate) {
      this.carousel.style.transition = 'transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94)';
    } else {
      this.carousel.style.transition = 'none';
    }
    
    this.carousel.style.transform = `translateX(${translateX}px)`;
    
    // Update indicators
    this.updateIndicators();
    
    // Add animation classes to visible items
    this.addItemAnimations();
  }
  
  updateIndicators() {
    this.indicators.forEach((indicator, index) => {
      indicator.classList.toggle('active', index === this.currentIndex);
    });
  }
  
  addItemAnimations() {
    this.items.forEach((item, index) => {
      item.classList.remove('slide-in-left', 'slide-in-right');
      
      if (index >= this.currentIndex && index < this.currentIndex + this.itemsPerView) {
        const animationClass = index === this.currentIndex ? 'slide-in-left' : 'slide-in-right';
        setTimeout(() => {
          item.classList.add(animationClass);
        }, (index - this.currentIndex) * 100);
      }
    });
  }
  
  moveCarousel(direction) {
    if (this.isAnimating) return;
    
    this.isAnimating = true;
    
    if (direction === 1) {
      // Move right
      const maxIndex = Math.max(0, this.totalItems - Math.floor(this.itemsPerView));
      if (this.currentIndex < maxIndex) {
        this.currentIndex++;
      } else {
        this.currentIndex = 0; // Loop back to start
      }
    } else {
      // Move left
      if (this.currentIndex > 0) {
        this.currentIndex--;
      } else {
        const maxIndex = Math.max(0, this.totalItems - Math.floor(this.itemsPerView));
        this.currentIndex = maxIndex; // Loop to end
      }
    }
    
    this.updateCarouselPosition();
    
    setTimeout(() => {
      this.isAnimating = false;
    }, 600);
  }
  
  goToSlide(index) {
    if (this.isAnimating || index === this.currentIndex) return;
    
    this.isAnimating = true;
    this.currentIndex = index;
    this.updateCarouselPosition();
    
    setTimeout(() => {
      this.isAnimating = false;
    }, 600);
  }
  
  startAutoPlay() {
    this.stopAutoPlay();
    this.autoPlayInterval = setInterval(() => {
      this.moveCarousel(1);
    }, 5000); // Change slide every 5 seconds
  }
  
  stopAutoPlay() {
    if (this.autoPlayInterval) {
      clearInterval(this.autoPlayInterval);
      this.autoPlayInterval = null;
    }
  }
  
  addTouchSupport() {
    let startX = 0;
    let startY = 0;
    let isDragging = false;
    
    this.carousel.addEventListener('touchstart', (e) => {
      startX = e.touches[0].clientX;
      startY = e.touches[0].clientY;
      isDragging = false;
      this.stopAutoPlay();
    });
    
    this.carousel.addEventListener('touchmove', (e) => {
      if (!startX) return;
      
      const currentX = e.touches[0].clientX;
      const currentY = e.touches[0].clientY;
      const diffX = startX - currentX;
      const diffY = startY - currentY;
      
      if (Math.abs(diffX) > Math.abs(diffY) && Math.abs(diffX) > 10) {
        isDragging = true;
        e.preventDefault();
      }
    });
    
    this.carousel.addEventListener('touchend', (e) => {
      if (!startX || !isDragging) return;
      
      const endX = e.changedTouches[0].clientX;
      const diff = startX - endX;
      
      if (Math.abs(diff) > 50) {
        if (diff > 0) {
          this.moveCarousel(1); // Swipe left - move right
        } else {
          this.moveCarousel(-1); // Swipe right - move left
        }
      }
      
      startX = 0;
      isDragging = false;
      this.startAutoPlay();
    });
  }
}

// Global functions for button controls
function moveCarousel(direction) {
  if (window.newsCarousel) {
    window.newsCarousel.moveCarousel(direction);
  }
}

function goToSlide(index) {
  if (window.newsCarousel) {
    window.newsCarousel.goToSlide(index);
  }
}

// Initialize carousel when DOM is loaded
document.addEventListener('DOMContentLoaded', function() {
  // Wait a bit for all elements to be rendered
  setTimeout(() => {
    window.newsCarousel = new NewsCarousel();
  }, 100);
});

// Reinitialize on page changes (for SPA behavior)
if (typeof window !== 'undefined') {
  window.addEventListener('load', function() {
    if (!window.newsCarousel) {
      setTimeout(() => {
        window.newsCarousel = new NewsCarousel();
      }, 200);
    }
  });
}
</script>