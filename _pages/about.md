---
layout: about
title: about
permalink: /
subtitle: Research Assistant Professor in <a href='https://www.odu.edu/cyber'>Cybersecurity</a>. Old Dominion University.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p><i class="fas fa-envelope"></i> msikder@odu.edu</p>
    <p><i class="fas fa-envelope"></i> nazmulkabir@vt.edu</p>
    <p><i class="fas fa-map-marker-alt"></i> Norfolk, VA</p>
    <p><i class="fas fa-calendar-alt"></i> <a href="https://calendly.com/nazmulkabir-vt/30min">Schedule a meeting with me</a></p>

news: true # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

<div class="about-intro">
  <div class="intro-content">
    <h2>AI Research Scientist & Cybersecurity Expert</h2>
    <p class="intro-text">I am a <strong>Research Assistant Professor</strong> at Old Dominion University's <a href="https://covacci.org/" target="_blank">Commonwealth Cyber Initiative Coastal Virginia</a>, where I am exploring emerging research directions in cybersecurity. Previously, I was a <a href="https://www.research.vt.edu/about/postdoctoral-associates/virginia-tech-presidential-postdoctoral-fellowships/current-fellows/sikder-nazmul.html" target="_blank">Presidential Postdoctoral Fellow</a> at Virginia Tech. My expertise spans AI assurance, machine learning for cyberattack detection, and securing cyber-physical systems, with proven real-world applications in critical infrastructure including water distribution and agricultural networks.</p>
    
    <div class="intro-highlights">
      <div class="highlight-item">
        <span class="highlight-number">15+</span>
        <span class="highlight-label">Publications</span>
      </div>
      <div class="highlight-item">
        <span class="highlight-number">5+</span>
        <span class="highlight-label">Years Research</span>
      </div>
      <div class="highlight-item">
        <span class="highlight-number">10+</span>
        <span class="highlight-label">AI Projects</span>
      </div>
    </div>
  </div>
</div>

<div class="research-focus">
  <h3>Research Focus Areas</h3>
  
  <div class="research-container">
    <!-- Research Area Cards on Left -->
    <div class="research-areas-list">
      <article class="research-card" data-area="cybersecurity" onclick="showResearchDetails('cybersecurity')">
        <div class="card-content">
          <div class="card-header">
            <div class="card-icon">🛡️</div>
            <div class="card-meta">
              <span class="card-category cybersecurity">Cybersecurity</span>
              <span class="research-badge"><i class="fas fa-award"></i> 6 Publications</span>
            </div>
          </div>
          <h4>AI-Driven Cybersecurity</h4>
          <p>Developing advanced ML models for real-time threat detection in critical infrastructure</p>
        </div>
      </article>
      
      <article class="research-card" data-area="water" onclick="showResearchDetails('water')">
        <div class="card-content">
          <div class="card-header">
            <div class="card-icon">💧</div>
            <div class="card-meta">
              <span class="card-category water">Water Systems</span>
              <span class="research-badge"><i class="fas fa-award"></i> 3 Publications</span>
            </div>
          </div>
          <h4>Smart Water Systems</h4>
          <p>AI-powered solutions for monitoring and protecting water distribution networks</p>
        </div>
      </article>
      
      <article class="research-card" data-area="agriculture" onclick="showResearchDetails('agriculture')">
        <div class="card-content">
          <div class="card-header">
            <div class="card-icon">🌾</div>
            <div class="card-meta">
              <span class="card-category agriculture">AgriTech</span>
              <span class="research-badge"><i class="fas fa-award"></i> 3 Publications</span>
            </div>
          </div>
          <h4>Precision Agriculture</h4>
          <p>Machine learning for crop health monitoring and sustainable farming practices</p>
        </div>
      </article>
      
      <article class="research-card" data-area="assurance" onclick="showResearchDetails('assurance')">
        <div class="card-content">
          <div class="card-header">
            <div class="card-icon">✓</div>
            <div class="card-meta">
              <span class="card-category research">AI Assurance</span>
              <span class="research-badge"><i class="fas fa-award"></i> 3 Publications</span>
            </div>
          </div>
          <h4>AI Assurance & Reliability</h4>
          <p>Ensuring trustworthy, explainable, and safe AI systems in critical applications</p>
        </div>
      </article>
    </div>
    
    <!-- Details Panel on Right (Sticky) -->
    <div class="research-details-panel">
    
    <!-- Cybersecurity Details -->
    <div class="research-detail-content" id="detail-cybersecurity" style="display: none;">
      <div class="detail-header">
        <div class="detail-icon">🛡️</div>
        <h4>AI-Driven Cybersecurity</h4>
      </div>
      <p class="detail-description">Developing advanced machine learning models for real-time threat detection and response in critical infrastructure. My work focuses on creating scalable, deployable solutions that bridge the gap between academic research and industrial applications.</p>
      <h5>Key Publications</h5>
      <ul class="publication-detail-list">
              <li>
                <a href="https://www.sciencedirect.com/science/article/abs/pii/S2214714423000855" target="_blank">
                  <strong>Deep H2O: Cyber attacks detection in water distribution systems using deep learning</strong>
                  <span class="pub-venue">Journal of Water Process Engineering (2023)</span>
                </a>
              </li>
              <li>
                <a href="https://ascelibrary.org/doi/abs/10.1061/JOEEDU.EEENG-7266" target="_blank">
                  <strong>P2O: AI-Driven Framework for Managing and Securing Wastewater Treatment Plants</strong>
                  <span class="pub-venue">Journal of Environmental Engineering (2023)</span>
                </a>
              </li>
              <li>
                <a href="https://ieeexplore.ieee.org/abstract/document/9951019" target="_blank">
                  <strong>Model-agnostic scoring methods for artificial intelligence assurance</strong>
                  <span class="pub-venue">IEEE STC (2022)</span>
                </a>
              </li>
      </ul>
    </div>
    
    <!-- Water Systems Details -->
    <div class="research-detail-content" id="detail-water" style="display: none;">
      <div class="detail-header">
        <div class="detail-icon">💧</div>
        <h4>Smart Water Systems</h4>
      </div>
      <p class="detail-description">Pioneering AI-powered solutions for monitoring and protecting water distribution networks. My research has been deployed in operational water systems, demonstrating practical impact in safeguarding critical water infrastructure.</p>
      <h5>Key Publications</h5>
      <ul class="publication-detail-list">
              <li>
                <a href="https://dl.acm.org/doi/10.1145/3744350" target="_blank">
                  <strong>Context-driven Deep Learning Forecasting for Wastewater Treatment Plants</strong>
                  <span class="pub-venue">ACM TCPS (2025)</span>
                </a>
              </li>
              <li>
                <a href="https://ieeexplore.ieee.org/abstract/document/11028129" target="_blank">
                  <strong>Assessing the Impact of Cyber Attacks on Water Distribution Systems</strong>
                  <span class="pub-venue">IEEE Access (2023)</span>
                </a>
              </li>
              <li>
                <a href="https://www.waterrf.org/sites/default/files/file/2022-11/2022_IWS-Challenge-Solution_Virginia-Tech.pdf" target="_blank">
                  <strong>Realtime management of wastewater treatment plants using AI</strong>
                  <span class="pub-venue">International Water Symposium (2022)</span>
                </a>
        </li>
      </ul>
    </div>
    
    <!-- Agriculture Details -->
    <div class="research-detail-content" id="detail-agriculture" style="display: none;">
      <div class="detail-header">
        <div class="detail-icon">🌾</div>
        <h4>Precision Agriculture</h4>
      </div>
      <p class="detail-description">Applying machine learning to optimize agricultural practices, from crop health monitoring to irrigation management. My work combines computer vision and IoT technologies to enhance food security and resource efficiency.</p>
      <h5>Key Publications</h5>
      <ul class="publication-detail-list">
              <li>
                <a href="https://ieeexplore.ieee.org/abstract/document/9659921" target="_blank">
                  <strong>DeepAg: Deep learning approach for measuring the effects of outlier events</strong>
                  <span class="pub-venue">IEEE SSCI (2021)</span>
                </a>
              </li>
              <li>
                <a href="https://www.sciencedirect.com/science/article/abs/pii/B9780323919197000299" target="_blank">
                  <strong>The application of artificial intelligence assurance in precision farming</strong>
                  <span class="pub-venue">AI Assurance Book Chapter (2022)</span>
                </a>
              </li>
              <li>
                <a href="https://scholar.archive.org/work/x4nad4ffdrgprittlkqyu7paki/access/wayback/https://journals.flvc.org/FLAIRS/article/download/128497/130068" target="_blank">
                  <strong>Applications of machine learning for precision agriculture and smart farming</strong>
                  <span class="pub-venue">FLAIRS (2021)</span>
                </a>
              </li>
      </ul>
    </div>
    
    <!-- AI Assurance Details -->
    <div class="research-detail-content" id="detail-assurance" style="display: none;">
      <div class="detail-header">
        <div class="detail-icon">✓</div>
        <h4>AI Assurance & Reliability</h4>
      </div>
      <p class="detail-description">Advancing the field of trustworthy AI through research on explainability, safety, and ethical considerations. My book on AI Assurance serves as a comprehensive resource for developing reliable AI systems.</p>
      <h5>Key Publications</h5>
      <ul class="publication-detail-list">
              <li>
                <a href="https://vtechworks.lib.vt.edu/server/api/core/bitstreams/ddafd734-9641-4011-9bba-f5d4f8756bbe/content" target="_blank">
                  <strong>AI Methods for Anomaly Detection in Cyber-Physical Systems</strong>
                  <span class="pub-venue">PhD Dissertation, Virginia Tech (2025)</span>
                </a>
              </li>
              <li>
                <a href="https://www.sciencedirect.com/science/article/abs/pii/B9780323919197000202" target="_blank">
                  <strong>Outlier detection using AI: a survey</strong>
                  <span class="pub-venue">AI Assurance Book Chapter (2023)</span>
                </a>
              </li>
              <li>
                <a href="https://www.sciencedirect.com/book/9780323919197/ai-assurance" target="_blank">
                  <strong>AI Assurance: Towards Trustworthy, Explainable, Safe, and Ethical AI</strong>
                  <span class="pub-venue">Academic Press (2022)</span>
                </a>
        </li>
      </ul>
    </div>
    
  </div>
</div>
</div>

<style>
/* Research Focus Section */
.research-focus {
  margin-bottom: 4rem;
}

.research-focus h3 {
  font-size: 1.8rem;
  font-weight: 700;
  color: var(--global-text-color);
  margin-bottom: 2rem;
}

/* Two Column Layout */
.research-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  align-items: start;
}

/* Research Cards List (Horizontal) */
.research-areas-list {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.25rem;
}

/* Research Card */
.research-card {
  background: var(--global-bg-color);
  border-radius: 1rem;
  border: 2px solid var(--global-divider-color);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  transition: all 0.3s ease;
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.research-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, var(--global-theme-color), transparent);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.research-card:hover {
  transform: translateX(4px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
  border-color: var(--global-theme-color);
}

.research-card:hover::before {
  opacity: 1;
}

.research-card.active {
  border-color: var(--global-theme-color);
  border-width: 2px;
  box-shadow: 0 4px 16px rgba(52, 152, 219, 0.2);
  transform: translateX(8px);
}

.research-card.active::before {
  opacity: 1;
  height: 6px;
}

.card-content {
  padding: 1.5rem;
}

.card-header {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  margin-bottom: 0.75rem;
  gap: 1rem;
}

.card-icon {
  font-size: 2.5rem;
  line-height: 1;
  transition: transform 0.3s ease;
}

.research-card:hover .card-icon {
  transform: scale(1.1) rotate(-5deg);
}

.research-card.active .card-icon {
  transform: scale(1.15);
}

.card-meta {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  gap: 0.4rem;
}

.card-category {
  padding: 0.35rem 0.85rem;
  border-radius: 1rem;
  font-size: 0.7rem;
  font-weight: 600;
  color: white;
  white-space: nowrap;
}

.card-category.cybersecurity {
  background: linear-gradient(135deg, #e74c3c 0%, #c0392b 100%);
}

.card-category.water {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
}

.card-category.agriculture {
  background: linear-gradient(135deg, #2ecc71 0%, #27ae60 100%);
}

.card-category.research {
  background: linear-gradient(135deg, #9b59b6 0%, #8e44ad 100%);
}

.research-badge {
  font-size: 0.7rem;
  color: var(--global-text-color-light);
  display: flex;
  align-items: center;
  gap: 0.25rem;
}

.card-content h4 {
  font-size: 1.25em;
  font-weight: 600;
  color: var(--global-text-color);
  margin-bottom: 0.6rem;
  line-height: 1.3;
}

.card-content p {
  color: var(--global-text-color-light);
  line-height: 1.6;
  font-size: 17px;
  margin: 0;
}

/* Research Details Panel */
.research-details-panel {
  width: 100%;
  margin-top: 1.5rem;
}

.details-placeholder {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 3rem 2rem;
  text-align: center;
  color: var(--global-text-color-light);
  background: var(--global-code-bg-color);
  border-radius: 1rem;
  border: 2px dashed var(--global-divider-color);
  min-height: 300px;
}

.details-placeholder i {
  font-size: 3rem;
  margin-bottom: 1rem;
  opacity: 0.5;
}

.details-placeholder p {
  font-size: 1rem;
  font-style: italic;
}

.research-detail-content {
  display: none;
  padding: 2rem;
  background: var(--global-bg-color);
  border: 2px solid var(--global-theme-color);
  border-radius: 1rem;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
  animation: fadeSlideIn 0.4s ease;
}

@keyframes fadeSlideIn {
  0% {
    opacity: 0;
    transform: translateX(20px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.detail-header {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1.25rem;
  padding-bottom: 1rem;
  border-bottom: 2px solid var(--global-divider-color);
}

.detail-icon {
  font-size: 2.25rem;
}

.research-detail-content h4 {
  color: var(--global-theme-color);
  margin: 0;
  font-size: 1.75em;
  font-weight: 600;
}

.research-detail-content h5 {
  color: var(--global-text-color);
  margin: 1.25rem 0 0.9rem 0;
  font-size: 1.25em;
  font-weight: 600;
}

.detail-description {
  color: var(--global-text-color);
  line-height: 1.65;
  font-size: 18px;
  margin-bottom: 1.25rem;
}

/* Publication List */
.publication-detail-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: grid;
  gap: 0.85rem;
}

.publication-detail-list li {
  padding: 1rem;
  background: var(--global-code-bg-color);
  border-radius: 0.65rem;
  border-left: 4px solid var(--global-theme-color);
  transition: all 0.3s ease;
}

.publication-detail-list li:hover {
  transform: translateX(6px);
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
  background: var(--global-bg-color);
}

.publication-detail-list a {
  color: var(--global-text-color);
  text-decoration: none;
  display: block;
}

.publication-detail-list a:hover {
  color: var(--global-theme-color);
}

.publication-detail-list strong {
  display: block;
  margin-bottom: 0.4rem;
  font-size: 17px;
  line-height: 1.4;
  color: var(--global-text-color);
  font-weight: 600;
}

.publication-detail-list .pub-venue {
  display: block;
  font-size: 16px;
  color: var(--global-text-color-light);
  font-style: italic;
  margin-top: 0.2rem;
}

/* Responsive Design */
@media (max-width: 991px) {
  .research-areas-list {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .research-details-panel {
    position: relative;
    top: 0;
    max-height: none;
    overflow-y: visible;
  }
  
  .research-card:hover,
  .research-card.active {
    transform: translateX(0);
  }
}

@media (max-width: 768px) {
  .research-areas-list {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 768px) {
  .card-content {
    padding: 1.25rem;
  }
  
  .card-icon {
    font-size: 2rem;
  }
  
  .research-detail-content {
    padding: 1.5rem;
  }
  
  .detail-icon {
    font-size: 1.85rem;
  }
  
  .research-detail-content h4 {
    font-size: 1.35rem;
  }
}

@media (max-width: 480px) {
  .card-header {
    flex-direction: column;
    align-items: flex-start;
  }
  
  .card-meta {
    align-items: flex-start;
    flex-direction: row;
    gap: 0.6rem;
  }
}
</style>

<script>
function showResearchDetails(area) {
  const allDetails = document.querySelectorAll('.research-detail-content');
  const allCards = document.querySelectorAll('.research-card');
  const placeholder = document.querySelector('.details-placeholder');
  const selectedCard = document.querySelector('.research-card[data-area="' + area + '"]');
  const selectedDetail = document.getElementById('detail-' + area);
  
  // Check if clicking the same card (toggle off)
  if (selectedCard.classList.contains('active')) {
    selectedCard.classList.remove('active');
    selectedDetail.style.display = 'none';
    if (placeholder) {
      placeholder.style.display = 'flex';
    }
    return;
  }
  
  // Remove active from all cards
  allCards.forEach(card => card.classList.remove('active'));
  
  // Hide all details
  allDetails.forEach(detail => {
    detail.style.display = 'none';
  });
  
  // Hide placeholder if it exists
  if (placeholder) {
    placeholder.style.display = 'none';
  }
  
  // Show selected detail with animation
  if (selectedDetail) {
    selectedDetail.style.display = 'block';
  }
  
  // Add active class to clicked card
  if (selectedCard) {
    selectedCard.classList.add('active');
  }
}
</script>

<style>
/* Typography - Academic Pages Style */
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  line-height: 1.6;
}

h1, h2, h3, h4, h5, h6 {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: 600;
  line-height: 1.3;
}

/* Scale down profile image */
.profile img {
  max-width: 70%;
  height: auto;
}

/* Professional About Page Styling */
.about-intro {
  background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);
  padding: 2rem;
  border-radius: 12px;
  margin-bottom: 2.5rem;
  border: 1px solid #e9ecef;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  grid-column: 1 / -1;
}

html[data-theme='dark'] .about-intro {
  background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
  border: 1px solid #404040;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}

/* Research Focus and other sections span full width */
.research-focus,
.background-section {
  grid-column: 1 / -1;
}

.intro-content h2 {
  font-size: 2em;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1rem;
  text-align: center;
}

html[data-theme='dark'] .intro-content h2 {
  color: #e8e8e8;
}

.intro-text {
  font-size: 18px;
  line-height: 1.65;
  color: #495057;
  margin-bottom: 1.5rem;
  text-align: center;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

html[data-theme='dark'] .intro-text {
  color: #c0c0c0;
}

.intro-highlights {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
  margin-top: 1.5rem;
}

.highlight-item {
  text-align: center;
  padding: 0.75rem;
}

.highlight-number {
  display: block;
  font-size: 2em;
  font-weight: 600;
  color: #3498db;
  margin-bottom: 0.25rem;
}

.highlight-label {
  font-size: 1em;
  color: #6c757d;
  font-weight: 500;
}

/* Research Focus Areas */
.research-focus {
  margin-bottom: 2.5rem;
}

.research-focus h3 {
  font-size: 1.75em;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1.5rem;
  text-align: center;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e9ecef;
}

html[data-theme='dark'] .research-focus h3 {
  color: #e8e8e8;
  border-bottom: 2px solid #404040;
}

.focus-areas {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}

.focus-area {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  background: white;
  padding: 1.25rem;
  border-radius: 10px;
  border: 1px solid #e9ecef;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .focus-area {
  background: #2d2d2d;
  border: 1px solid #404040;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}

.focus-area:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}

.focus-icon {
  flex-shrink: 0;
  width: 40px;
  height: 40px;
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 1.1rem;
}

.focus-content h4 {
  font-size: 1rem;
  font-weight: 600;
  color: #2c3e50;
  margin: 0 0 0.5rem 0;
}

html[data-theme='dark'] .focus-content h4 {
  color: #e8e8e8;
}

.focus-content p {
  font-size: 0.9rem;
  color: #6c757d;
  margin: 0 0 1rem 0;
  line-height: 1.5;
}

html[data-theme='dark'] .focus-content p {
  color: #b0b0b0;
}

/* Focus Papers Styling */
.focus-papers {
  margin-top: 1rem;
}

.focus-papers h6 {
  font-size: 0.85rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 0.75rem;
  border-bottom: 1px solid #e9ecef;
  padding-bottom: 0.25rem;
}

html[data-theme='dark'] .focus-papers h6 {
  color: #e8e8e8;
  border-bottom: 1px solid #404040;
}

.paper-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.paper-list li {
  margin-bottom: 0.75rem;
  padding: 0.5rem;
  background: #f8f9fa;
  border-radius: 6px;
  border-left: 3px solid #3498db;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .paper-list li {
  background: #1a1a1a;
  border-left: 3px solid #5dade2;
}

.paper-list li:hover {
  background: #e3f2fd;
  transform: translateX(3px);
}

html[data-theme='dark'] .paper-list li:hover {
  background: #2d4a5c;
}

.paper-list li a {
  font-size: 0.85rem;
  font-weight: 500;
  color: #2c3e50;
  text-decoration: none;
  line-height: 1.4;
  display: block;
  margin-bottom: 0.25rem;
}

html[data-theme='dark'] .paper-list li a {
  color: #e8e8e8;
}

.paper-list li a:hover {
  color: #3498db;
  text-decoration: none;
}

html[data-theme='dark'] .paper-list li a:hover {
  color: #5dade2;
}

.paper-list .journal {
  font-size: 0.75rem;
  color: #6c757d;
  font-style: italic;
  font-weight: 400;
}

html[data-theme='dark'] .paper-list .journal {
  color: #999999;
}

/* Background Section */
.background-section {
  margin-bottom: 2.5rem;
}

.background-section h3 {
  font-size: 1.4rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 1.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e9ecef;
}

html[data-theme='dark'] .background-section h3 {
  color: #e8e8e8;
  border-bottom: 2px solid #404040;
}

/* Timeline Styling */
.journey-timeline {
  position: relative;
  padding-left: 2.5rem;
}

.journey-timeline::before {
  content: '';
  position: absolute;
  left: 1rem;
  top: 0;
  bottom: 0;
  width: 2px;
  background: linear-gradient(180deg, #3498db 0%, #2980b9 100%);
}

.timeline-item {
  position: relative;
  margin-bottom: 2rem;
}

.timeline-marker {
  position: absolute;
  left: -2.5rem;
  top: 0.25rem;
  width: 2rem;
  height: 2rem;
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 0.9rem;
  box-shadow: 0 2px 8px rgba(52, 152, 219, 0.3);
}

.timeline-content {
  background: white;
  padding: 1.5rem;
  border-radius: 10px;
  border: 1px solid #e9ecef;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  transition: all 0.3s ease;
}

html[data-theme='dark'] .timeline-content {
  background: #2d2d2d;
  border: 1px solid #404040;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}

.timeline-content:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}

html[data-theme='dark'] .timeline-content:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.4);
}

.timeline-content h4 {
  color: #2c3e50;
  margin-bottom: 0.5rem;
  font-weight: 600;
  font-size: 1.1rem;
}

html[data-theme='dark'] .timeline-content h4 {
  color: #e8e8e8;
}

.institution {
  color: #3498db;
  font-weight: 500;
  margin-bottom: 0.75rem;
  font-size: 0.9rem;
}

html[data-theme='dark'] .institution {
  color: #5dade2;
}

.timeline-content p {
  color: #6c757d;
  font-size: 0.9rem;
  line-height: 1.6;
  margin-bottom: 0.75rem;
}

html[data-theme='dark'] .timeline-content p {
  color: #b0b0b0;
}

.achievement-badges {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.badge {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
  padding: 0.25rem 0.75rem;
  border-radius: 15px;
  font-size: 0.75rem;
  font-weight: 500;
}

/* Research Highlights Sidebar */
.research-highlights {
  background: white;
  padding: 1.5rem;
  border-radius: 10px;
  border: 1px solid #e9ecef;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  height: fit-content;
}

html[data-theme='dark'] .research-highlights {
  background: #2d2d2d;
  border: 1px solid #404040;
  box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}

.research-highlights h4 {
  color: #2c3e50;
  margin-bottom: 1.25rem;
  font-weight: 600;
  font-size: 1.1rem;
  text-align: center;
}

html[data-theme='dark'] .research-highlights h4 {
  color: #e8e8e8;
}

.highlight-stats {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.stat-item {
  text-align: center;
  padding: 0.75rem;
  background: #f8f9fa;
  border-radius: 8px;
  transition: all 0.3s ease;
}

html[data-theme='dark'] .stat-item {
  background: #1a1a1a;
}

.stat-item:hover {
  background: linear-gradient(135deg, #3498db 0%, #2980b9 100%);
  color: white;
  transform: translateY(-2px);
}

.stat-number {
  font-size: 1.3rem;
  font-weight: 700;
  color: #3498db;
  margin-bottom: 0.25rem;
}

html[data-theme='dark'] .stat-number {
  color: #5dade2;
}

.stat-item:hover .stat-number {
  color: white;
}

.stat-label {
  font-size: 0.8rem;
  color: #6c757d;
  font-weight: 500;
}

html[data-theme='dark'] .stat-label {
  color: #b0b0b0;
}

.stat-item:hover .stat-label {
  color: white;
}

.current-focus-box {
  background: #f8f9fa;
  padding: 1.25rem;
  border-radius: 8px;
  border: 1px solid #e9ecef;
}

html[data-theme='dark'] .current-focus-box {
  background: #1a1a1a;
  border: 1px solid #404040;
}

.current-focus-box h5 {
  color: #2c3e50;
  margin-bottom: 0.75rem;
  font-weight: 600;
  font-size: 1rem;
}

html[data-theme='dark'] .current-focus-box h5 {
  color: #e8e8e8;
}

.current-focus-box p {
  color: #6c757d;
  font-size: 0.9rem;
  line-height: 1.6;
  margin: 0;
}

html[data-theme='dark'] .current-focus-box p {
  color: #b0b0b0;
}

/* Collaboration Section */
.collaboration-section {
  background: linear-gradient(135deg, #34495e 0%, #2c3e50 100%);
  color: white;
  padding: 2.5rem 2rem;
  border-radius: 12px;
  text-align: center;
  margin-top: 2.5rem;
}

.cta-content h3 {
  font-size: 1.6rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.cta-content p {
  font-size: 1rem;
  margin-bottom: 2rem;
  opacity: 0.9;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.cta-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 1.5rem;
  border-radius: 8px;
  font-weight: 600;
  font-size: 0.9rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

.btn-primary {
  background: #3498db;
  color: white;
  border: 2px solid #3498db;
}

.btn-primary:hover {
  background: #2980b9;
  border-color: #2980b9;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(52, 152, 219, 0.4);
  text-decoration: none;
  color: white;
}

.btn-outline {
  background: transparent;
  color: white;
  border: 2px solid rgba(255,255,255,0.5);
}

.btn-outline:hover {
  background: rgba(255,255,255,0.1);
  border-color: rgba(255,255,255,0.8);
  transform: translateY(-2px);
  text-decoration: none;
  color: white;
}

/* Responsive Design */
@media (max-width: 768px) {
  .about-intro {
    padding: 1.5rem;
  }
  
  .intro-content h2 {
    font-size: 1.5rem;
  }
  
  .intro-text {
    font-size: 0.95rem;
  }
  
  .intro-highlights {
    gap: 1rem;
  }
  
  .highlight-number {
    font-size: 1.3rem;
  }
  
  .focus-areas {
    grid-template-columns: 1fr;
  }
  
  .focus-area {
    padding: 1rem;
  }
  
  .journey-timeline {
    padding-left: 2rem;
  }
  
  .timeline-marker {
    left: -2rem;
    width: 1.5rem;
    height: 1.5rem;
    font-size: 0.8rem;
  }
  
  .highlight-stats {
    grid-template-columns: 1fr;
  }
  
  .collaboration-section {
    padding: 2rem 1.5rem;
  }
  
  .cta-content h3 {
    font-size: 1.4rem;
  }
  
  .cta-buttons {
    flex-direction: column;
    align-items: center;
  }
  
  .btn {
    width: 100%;
    max-width: 250px;
    justify-content: center;
  }
}

@media (max-width: 480px) {
  .intro-content h2 {
    font-size: 1.3rem;
  }
  
  .intro-highlights {
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
  }
  
  .highlight-item {
    padding: 0.5rem;
  }
  
  .timeline-content {
    padding: 1rem;
  }
  
  .research-highlights {
    padding: 1rem;
  }
}
</style>
