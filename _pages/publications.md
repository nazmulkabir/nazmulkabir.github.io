---
layout: page
permalink: /publications/
title: publications
description: Research publications in AI assurance, cybersecurity, and machine learning for critical infrastructure
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->
<div class="publications">

<!-- Publication Statistics Section -->
<div class="publication-stats-section mb-5">
  <div class="row">
    <div class="col-md-12">
      <div class="card border-0 shadow-sm">
        <div class="card-body text-center">
          <h4 class="card-title mb-4"><i class="fas fa-chart-bar text-primary"></i> Publication Metrics</h4>
          <div class="row">
            <div class="col-md-3">
              <div class="stat-item">
                <h3 class="text-primary mb-1">{% bibliography_count -f {{site.scholar.bibliography}} %}</h3>
                <p class="text-muted mb-0">Total Publications</p>
              </div>
            </div>
            <div class="col-md-3">
              <div class="stat-item">
                <h3 class="text-success mb-1">{% bibliography_count -f {{site.scholar.bibliography}} -q @phdthesis %}</h3>
                <p class="text-muted mb-0">PhD Thesis</p>
              </div>
            </div>
            <div class="col-md-3">
              <div class="stat-item">
                <h3 class="text-info mb-1">{% bibliography_count -f {{site.scholar.bibliography}} -q @article %}</h3>
                <p class="text-muted mb-0">Journal Articles</p>
              </div>
            </div>
            <div class="col-md-3">
              <div class="stat-item">
                <h3 class="text-warning mb-1">{% bibliography_count -f {{site.scholar.bibliography}} -q @inproceedings %}</h3>
                <p class="text-muted mb-0">Conference Papers</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Research Areas Section -->
<div class="research-areas-section mb-5">
  <div class="row">
    <div class="col-md-12">
      <h3 class="section-title text-center mb-4">
        <i class="fas fa-brain text-primary"></i> Research Areas
      </h3>
      <div class="row">
        <div class="col-md-3 mb-3">
          <div class="card h-100 border-0 shadow-sm research-area-card">
            <div class="card-body text-center">
              <i class="fas fa-shield-alt text-primary mb-3" style="font-size: 2.5rem;"></i>
              <h5 class="card-title">Cybersecurity</h5>
              <p class="card-text text-muted">AI-driven security for critical infrastructure and cyber-physical systems</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-3">
          <div class="card h-100 border-0 shadow-sm research-area-card">
            <div class="card-body text-center">
              <i class="fas fa-water text-info mb-3" style="font-size: 2.5rem;"></i>
              <h5 class="card-title">Water Systems</h5>
              <p class="card-text text-muted">Smart water distribution and wastewater treatment optimization</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-3">
          <div class="card h-100 border-0 shadow-sm research-area-card">
            <div class="card-body text-center">
              <i class="fas fa-seedling text-success mb-3" style="font-size: 2.5rem;"></i>
              <h5 class="card-title">Agriculture</h5>
              <p class="card-text text-muted">AI assurance in precision farming and agricultural production</p>
            </div>
          </div>
        </div>
        <div class="col-md-3 mb-3">
          <div class="card h-100 border-0 shadow-sm research-area-card">
            <div class="card-body text-center">
              <i class="fas fa-exclamation-triangle text-warning mb-3" style="font-size: 2.5rem;"></i>
              <h5 class="card-title">Anomaly Detection</h5>
              <p class="card-text text-muted">Outlier detection and AI assurance methodologies</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Google Scholar Profile Section -->
<div class="scholar-profile-section mb-5">
  <div class="row justify-content-center">
    <div class="col-md-8">
      <div class="card border-0 shadow-sm">
        <div class="card-body text-center">
          <h4 class="card-title mb-3">
            <i class="ai ai-google-scholar text-primary"></i> Google Scholar Profile
          </h4>
          <p class="card-text mb-3">For the most up-to-date citation metrics and additional publications, visit my Google Scholar profile.</p>
          <a href="https://scholar.google.com/citations?user={{site.scholar_userid}}" 
             class="btn btn-primary btn-lg" 
             target="_blank" 
             rel="noopener noreferrer">
            <i class="ai ai-google-scholar"></i> View Google Scholar
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Publications Section -->
<div class="publications-list-section">
  <div class="row">
    <div class="col-md-12">
      <h3 class="section-title text-center mb-4">
        <i class="fas fa-file-alt text-primary"></i> Publications by Year
      </h3>
      
      <!-- Search and Filter Options -->
      <div class="publication-controls mb-4">
        <div class="row">
          <div class="col-md-6 mb-3">
            <div class="input-group">
              <span class="input-group-text"><i class="fas fa-search"></i></span>
              <input type="text" id="publication-search" class="form-control" placeholder="Search publications...">
            </div>
          </div>
          <div class="col-md-6 mb-3">
            <select class="form-select" id="publication-filter">
              <option value="">All Publication Types</option>
              <option value="phdthesis">PhD Thesis</option>
              <option value="article">Journal Articles</option>
              <option value="inproceedings">Conference Papers</option>
              <option value="book">Books</option>
              <option value="inbook">Book Chapters</option>
            </select>
          </div>
        </div>
      </div>

      <!-- Publications List -->
      <div id="publications-container">
        {% bibliography %}
      </div>
    </div>
  </div>
</div>

</div>

<style>
.publication-stats-section .stat-item {
  padding: 1rem;
  border-radius: 0.5rem;
  transition: transform 0.3s ease;
}

.publication-stats-section .stat-item:hover {
  transform: translateY(-5px);
}

.research-area-card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: pointer;
}

.research-area-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15) !important;
}

.section-title {
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 2rem;
}

.publication-controls {
  background: #f8f9fa;
  padding: 1.5rem;
  border-radius: 0.75rem;
  border: 1px solid #e9ecef;
}

.publications .bibliography .row {
  margin-bottom: 2rem;
  padding: 1.5rem;
  background: #ffffff;
  border-radius: 0.75rem;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 1px solid #e9ecef;
}

.publications .bibliography .row:hover {
  transform: translateY(-3px);
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.15);
}

.publications .bibliography .title {
  font-size: 1.2rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 0.5rem;
  line-height: 1.4;
}

.publications .bibliography .author {
  color: #6c757d;
  margin-bottom: 0.5rem;
  font-size: 0.95rem;
}

.publications .bibliography .author em {
  color: #007bff;
  font-weight: 600;
}

.publications .bibliography .venue {
  color: #28a745;
  font-weight: 500;
  margin-bottom: 0.5rem;
}

.publications .bibliography .year {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 0.25rem 0.75rem;
  border-radius: 1rem;
  font-size: 0.85rem;
  font-weight: 600;
  display: inline-block;
  margin-bottom: 0.5rem;
}

/* Custom button styles */
.btn-outline-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 123, 255, 0.3);
}

/* Badge enhancements */
.badge {
  font-size: 0.8rem;
  padding: 0.5rem 0.75rem;
}

/* Animation for statistics */
@keyframes countUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.stat-item h3 {
  animation: countUp 0.8s ease-out;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .publication-stats-section .row > div {
    margin-bottom: 1rem;
  }
  
  .research-area-card {
    margin-bottom: 1rem;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Search functionality
  const searchInput = document.getElementById('publication-search');
  const filterSelect = document.getElementById('publication-filter');
  const publicationsContainer = document.getElementById('publications-container');
  const publications = publicationsContainer.querySelectorAll('.bibliography > .row');

  function filterPublications() {
    const searchTerm = searchInput.value.toLowerCase();
    const filterType = filterSelect.value;

    publications.forEach(pub => {
      const title = pub.querySelector('.title')?.textContent.toLowerCase() || '';
      const author = pub.querySelector('.author')?.textContent.toLowerCase() || '';
      const venue = pub.querySelector('.venue')?.textContent.toLowerCase() || '';
      const abstract = pub.querySelector('.abstract')?.textContent.toLowerCase() || '';
      
      const matchesSearch = !searchTerm || 
        title.includes(searchTerm) || 
        author.includes(searchTerm) || 
        venue.includes(searchTerm) ||
        abstract.includes(searchTerm);
      
      const matchesFilter = !filterType || pub.id.includes(filterType);
      
      pub.style.display = (matchesSearch && matchesFilter) ? 'block' : 'none';
    });
  }

  searchInput.addEventListener('input', filterPublications);
  filterSelect.addEventListener('change', filterPublications);

  // Smooth scroll for research area cards
  document.querySelectorAll('.research-area-card').forEach(card => {
    card.addEventListener('click', function() {
      const publicationsSection = document.querySelector('.publications-list-section');
      publicationsSection.scrollIntoView({ behavior: 'smooth' });
    });
  });
});
</script>
