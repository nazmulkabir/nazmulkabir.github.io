---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->
<div class="publications">

<!-- Publications Section -->
<div class="publications-list-section">
  <div class="row">
    <div class="col-md-12">

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
  background: var(--global-card-bg-color);
  padding: 1.5rem;
  border-radius: 0.75rem;
  border: 1px solid var(--global-divider-color);
}

.publications .bibliography .row {
  margin-bottom: 2rem;
  padding: 1.5rem;
  background: var(--global-card-bg-color);
  border-radius: 0.75rem;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 1px solid var(--global-divider-color);
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

<style>
/* Compact Stats Styling */
.stats-compact {
  text-align: center;
  max-width: 800px;
  margin: 0 auto;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.stat-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1rem;
  background: var(--global-card-bg-color);
  border-radius: 0.75rem;
  border: 1px solid var(--global-divider-color);
  transition: transform 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-2px);
}

.stat-number {
  font-size: 2rem;
  font-weight: 700;
  color: var(--global-theme-color);
  margin-bottom: 0.25rem;
}

.stat-label {
  font-size: 0.875rem;
  color: var(--global-text-color-light);
  font-weight: 500;
}

.publication-highlights {
  margin-top: 1.5rem;
}

.publication-highlights h6 {
  color: var(--global-text-color-light);
  font-weight: 600;
  margin-bottom: 0.75rem;
}

.venue-tags {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 0.5rem;
}

.venue-tag {
  background: rgba(102, 126, 234, 0.1);
  color: var(--global-theme-color);
  padding: 0.375rem 0.75rem;
  border-radius: 1rem;
  font-size: 0.75rem;
  font-weight: 500;
  border: 1px solid rgba(102, 126, 234, 0.2);
}

@media (max-width: 768px) {
  .stats-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }
  
  .stat-number {
    font-size: 1.5rem;
  }
}
</style>
