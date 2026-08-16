---
title: "Scientific Illustrations Portfolio"
url: "/gallery/scientific-illustrations-portfolio/"
summary: "Feel free to use my scientific illustartions for any academic purpose! Enjoy! 💙"
date: 2025-09-18
tags:
  - Featured
  - Featured Illustration
  - Illustrations
  - Ferroptosis
  - Metabolic Disorders
show_date: false
show_time: false
show_read_time: false
reading_time: false
image:
  filename: "featured.png"
  focal_point: "center"
  preview_only: true
---

<p class="portfolio-subtitle"><em>Feel free to use my scientific illustartions for any academic purpose! Enjoy! 💙</em></p>

<div class="portfolio-container">
  <div id="portfolioGrid" class="portfolio-grid"></div>
</div>

<!-- Lightbox Modal Popup -->
<div id="illustrationModal" class="sci-modal-overlay" role="dialog" aria-modal="true" aria-labelledby="sciModalTitle">
  <div class="sci-modal-container">
    <button class="sci-modal-close" onclick="closeSciModal()" aria-label="Close modal">&times;</button>
    <div class="sci-modal-header">
      <h2 id="sciModalTitle" class="sci-modal-title"></h2>
      <div class="sci-modal-meta">
        <span id="sciModalDate" class="sci-modal-date"></span>
        <div id="sciModalTags" class="sci-modal-tags"></div>
      </div>
    </div>
    <div class="sci-modal-body">
      <div class="sci-modal-img-frame">
        <img id="sciModalImg" src="" alt="Scientific Illustration Preview" />
      </div>
      <p id="sciModalDesc" class="sci-modal-desc"></p>
    </div>
    <div class="sci-modal-footer">
      <a id="sciModalFullView" href="#" target="_blank" rel="noopener noreferrer" class="sci-btn sci-btn-secondary">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
          <polyline points="15 3 21 3 21 9"></polyline>
          <line x1="10" y1="14" x2="21" y2="3"></line>
        </svg>
        Full View
      </a>
      <a id="sciModalDownload" href="#" download class="sci-btn sci-btn-primary">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
          <polyline points="7 10 12 15 17 10"></polyline>
          <line x1="12" y1="15" x2="12" y2="3"></line>
        </svg>
        Download
      </a>
    </div>
  </div>
</div>

<style>
/* Hide default page-level metadata headers & date stamps */
time,
.article-metadata,
.article-meta,
.page-header-metadata,
.article-date,
.reading-time,
.article-header,
.article-featured-image,
.featured-image-wrapper,
.page-wrapper > article > img,
.hugo-blox-article-header,
.hugo-blox-featured-image,
div[class*="article-meta"],
span[class*="article-meta"],
div[class*="featured-image"],
[itemprop="datePublished"] {
  display: none !important;
}

.portfolio-subtitle {
  font-style: italic;
  font-size: 1.05rem;
  color: var(--color-footer-fg, #8b949e);
  margin-top: 0.5rem;
  margin-bottom: 2.25rem;
  line-height: 1.5;
}

.portfolio-container {
  width: 100%;
  margin: 1.5rem 0 3.5rem 0;
}

.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.75rem;
}

@media (max-width: 1023px) {
  .portfolio-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 639px) {
  .portfolio-grid {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }
}

/* Stylistic Card Design conforming to site theme */
.sci-card {
  background: var(--color-header-bg, #161b22);
  border: 1px solid var(--color-border, rgba(255, 255, 255, 0.12));
  border-radius: var(--hb-radius, 16px);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  cursor: pointer;
  box-shadow: 0 6px 24px rgba(0, 0, 0, 0.2);
  transition: transform 0.35s cubic-bezier(0.16, 1, 0.3, 1), box-shadow 0.35s cubic-bezier(0.16, 1, 0.3, 1), border-color 0.3s ease;
  position: relative;
  height: 100%;
}

.sci-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 16px 36px rgba(56, 189, 248, 0.22), 0 0 20px rgba(56, 189, 248, 0.1);
  border-color: var(--color-primary-500, #38bdf8);
}

/* Image fills top portion edge-to-edge with no padding */
.sci-card-img-wrapper {
  width: 100%;
  height: 240px;
  background: radial-gradient(circle at center, rgba(30, 41, 59, 0.6) 0%, rgba(2, 6, 23, 0.95) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
  border-bottom: 1px solid var(--color-border, rgba(255, 255, 255, 0.08));
  padding: 0 !important;
  margin: 0 !important;
}

.sci-card-img-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
}

.sci-card:hover .sci-card-img-wrapper img {
  transform: scale(1.05);
}

/* Hover Preview Overlay & Badge */
.sci-card-hover-overlay {
  position: absolute;
  inset: 0;
  background: rgba(13, 17, 23, 0.72);
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: opacity 0.3s ease;
  z-index: 5;
}

.sci-card:hover .sci-card-hover-overlay {
  opacity: 1;
}

.sci-preview-badge {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  background: linear-gradient(135deg, var(--color-primary-500, #38bdf8), #0284c7);
  color: #0f172a;
  font-size: 0.85rem;
  font-weight: 700;
  padding: 0.5rem 1.15rem;
  border-radius: 24px;
  box-shadow: 0 4px 18px rgba(56, 189, 248, 0.4);
  transform: translateY(8px) scale(0.95);
  transition: transform 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  letter-spacing: 0.4px;
}

.sci-card:hover .sci-preview-badge {
  transform: translateY(0) scale(1);
}

.sci-card-body {
  padding: 1.35rem;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

.sci-card-top-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 0.5rem;
}

.sci-card-fig-num {
  font-size: 0.72rem;
  font-weight: 800;
  color: var(--color-primary-500, #38bdf8);
  letter-spacing: 1px;
  text-transform: uppercase;
  background: rgba(56, 189, 248, 0.1);
  border: 1px solid rgba(56, 189, 248, 0.22);
  padding: 2px 8px;
  border-radius: 6px;
}

.sci-card-date {
  font-size: 0.78rem;
  color: var(--color-footer-fg, #8b949e);
  font-weight: 500;
}

.sci-card-title {
  font-size: 1.05rem;
  font-weight: 700;
  color: var(--color-foreground, #f8fafc);
  margin: 0.25rem 0 0.45rem 0;
  line-height: 1.35;
}

.sci-card-desc {
  font-size: 0.86rem;
  color: var(--color-footer-fg, #94a3b8);
  line-height: 1.5;
  margin: 0 0 1.1rem 0;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.sci-card-footer {
  margin-top: auto;
  padding-top: 0.85rem;
  border-top: 1px solid var(--color-border, rgba(255, 255, 255, 0.07));
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.sci-card-tag {
  font-size: 0.75rem;
  font-weight: 600;
  color: var(--color-footer-fg, #94a3b8);
}

.sci-card-action {
  font-size: 0.82rem;
  font-weight: 700;
  color: var(--color-primary-500, #38bdf8);
  display: flex;
  align-items: center;
  gap: 4px;
  transition: gap 0.25s ease;
}

.sci-card:hover .sci-card-action {
  gap: 8px;
}

.sci-arrow {
  transition: transform 0.25s ease;
}

.sci-card:hover .sci-arrow {
  transform: translateX(3px);
}

.sci-tag-pill {
  background: rgba(56, 189, 248, 0.12);
  color: var(--color-primary-500, #38bdf8);
  border: 1px solid rgba(56, 189, 248, 0.25);
  font-size: 0.72rem;
  font-weight: 600;
  padding: 2px 8px;
  border-radius: 12px;
  letter-spacing: 0.3px;
}

/* Modal Popup Styles */
.sci-modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(5, 10, 20, 0.85);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  z-index: 99999;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem;
  opacity: 0;
  visibility: hidden;
  transition: opacity 0.25s ease, visibility 0.25s ease;
}

.sci-modal-overlay.active {
  opacity: 1;
  visibility: visible;
}

.sci-modal-container {
  background: var(--color-background, #0d1117);
  border: 1px solid var(--color-border, rgba(255, 255, 255, 0.15));
  border-radius: 16px;
  width: 100%;
  max-width: 900px;
  max-height: 90vh;
  display: flex;
  flex-direction: column;
  position: relative;
  box-shadow: 0 25px 60px rgba(0, 0, 0, 0.6);
  transform: scale(0.95);
  transition: transform 0.25s ease;
  overflow: hidden;
}

.sci-modal-overlay.active .sci-modal-container {
  transform: scale(1);
}

.sci-modal-close {
  position: absolute;
  top: 12px;
  right: 14px;
  background: rgba(255, 255, 255, 0.1);
  border: none;
  color: var(--color-foreground, #ffffff);
  width: 36px;
  height: 36px;
  border-radius: 50%;
  font-size: 1.25rem;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 10;
  transition: background 0.2s ease, transform 0.2s ease;
}

.sci-modal-close:hover {
  background: rgba(239, 68, 68, 0.85);
  color: #fff;
}

.sci-modal-header {
  padding: 1.25rem 3.5rem 0.75rem 1.5rem;
  border-bottom: 1px solid var(--color-border, rgba(255, 255, 255, 0.1));
}

.sci-modal-title {
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--color-foreground, #ffffff);
  margin: 0;
  line-height: 1.35;
}

.sci-modal-meta {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-top: 6px;
}

.sci-modal-date {
  font-size: 0.82rem;
  color: var(--color-footer-fg, #8b949e);
  font-weight: 500;
}

.sci-modal-tags {
  display: flex;
  gap: 6px;
  flex-wrap: wrap;
}

.sci-modal-body {
  padding: 1.25rem;
  overflow-y: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  flex-grow: 1;
}

.sci-modal-img-frame {
  width: 100%;
  max-height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(0, 0, 0, 0.35);
  border-radius: 10px;
  padding: 0.5rem;
  overflow: hidden;
}

.sci-modal-img-frame img {
  max-width: 100%;
  max-height: 55vh;
  object-fit: contain;
  border-radius: 6px;
}

.sci-modal-desc {
  font-size: 0.95rem;
  line-height: 1.55;
  color: var(--color-footer-fg, #8b949e);
  background: rgba(255, 255, 255, 0.03);
  padding: 0.85rem 1rem;
  border-radius: 8px;
  border-left: 3px solid var(--color-primary-500, #38bdf8);
  margin: 0;
}

.sci-modal-footer {
  padding: 1rem 1.5rem;
  border-top: 1px solid var(--color-border, rgba(255, 255, 255, 0.1));
  display: flex;
  gap: 0.75rem;
  justify-content: flex-end;
  background: var(--color-header-bg, #161b22);
}

.sci-btn {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 0.55rem 1.2rem;
  border-radius: 8px;
  font-size: 0.875rem;
  font-weight: 600;
  text-decoration: none !important;
  cursor: pointer;
  transition: all 0.2s ease;
}

.sci-btn-primary {
  background: #2563eb;
  color: #ffffff !important;
  border: 1px solid #3b82f6;
}

.sci-btn-primary:hover {
  background: #1d4ed8;
  box-shadow: 0 4px 12px rgba(37, 99, 235, 0.35);
}

.sci-btn-secondary {
  background: rgba(255, 255, 255, 0.08);
  color: var(--color-foreground, #c9d1d9) !important;
  border: 1px solid var(--color-border, rgba(255, 255, 255, 0.15));
}

.sci-btn-secondary:hover {
  background: rgba(255, 255, 255, 0.16);
  border-color: rgba(255, 255, 255, 0.3);
}

@media (max-width: 639px) {
  .sci-modal-container {
    max-height: 95vh;
    border-radius: 12px;
  }
  .sci-modal-header {
    padding: 1rem 3rem 0.5rem 1rem;
  }
  .sci-modal-title {
    font-size: 1.05rem;
  }
  .sci-modal-body {
    padding: 0.75rem;
  }
  .sci-modal-img-frame img {
    max-height: 45vh;
  }
  .sci-modal-footer {
    flex-direction: column;
    padding: 0.75rem;
  }
  .sci-btn {
    width: 100%;
    justify-content: center;
  }
}
</style>

<script>
const scientificIllustrations = [
  {
    id: "fig-1",
    title: "Metabolic Disorders, Autonomic Immune Dysfunction, and Ferroptosis",
    date: "Sept 2025",
    tags: ["Illustrations", "Ferroptosis", "Metabolic"],
    image: "featured.png",
    download: "featured.png",
    description: "Integrative molecular signaling map illustrating how chronic nutrient overload, visceral white adipose tissue (vWAT) inflammation, and autonomic nerve impairment interact to drive iron-dependent ferroptosis across metabolic organs."
  },
  {
    id: "fig-2",
    title: "Visceral Adipose Tissue (vWAT) Inflammation",
    date: "Aug 2025",
    tags: ["Illustrations", "Adipose", "Inflammation"],
    image: "vwat-inflammation.png",
    download: "vwat-inflammation.png",
    description: "Pro-inflammatory signaling dynamics within visceral white adipose tissue during chronic nutrient surplus, featuring M1 macrophage activation, CD8+ T-cell infiltration, and cytokine secretion cascades."
  },
  {
    id: "fig-3",
    title: "SLC7A11 / GPX4 Lipid Peroxidation Axis",
    date: "July 2025",
    tags: ["Illustrations", "Lipid Peroxidation", "GPX4"],
    image: "gpx4-axis.png",
    download: "gpx4-axis.png",
    description: "Detailed cellular pathway of antioxidant breakdown, Nrf2/SLC7A11 suppression, and glutathione peroxidase 4 (GPX4) depletion leading to toxic lipid peroxidation."
  },
  {
    id: "fig-4",
    title: "Autonomic Nervous System & Vagal Tone",
    date: "June 2025",
    tags: ["Illustrations", "Neuro-Immune", "Vagal Tone"],
    image: "autonomic-dysregulation.png",
    download: "autonomic-dysregulation.png",
    description: "Neuro-immune axis highlighting sympathetic hyperreactivity and vagal anti-inflammatory pathway impairment in systemic metabolic dysfunction."
  }
];

function renderPortfolioGrid() {
  const container = document.getElementById('portfolioGrid');
  if (!container) return;
  
  container.innerHTML = scientificIllustrations.map((item, idx) => `
    <div class="sci-card" onclick="openSciModal(${idx})" role="button" tabindex="0" aria-label="View ${item.title}" onkeydown="if(event.key==='Enter'||event.key===' '){event.preventDefault();openSciModal(${idx});}">
      <div class="sci-card-img-wrapper">
        <img src="${item.image}" alt="${item.title}" loading="lazy" />
        <div class="sci-card-hover-overlay">
          <span class="sci-preview-badge">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="11" cy="11" r="8"></circle>
              <line x1="21" y1="21" x2="16.65" y2="16.65"></line>
              <line x1="11" y1="8" x2="11" y2="14"></line>
              <line x1="8" y1="11" x2="14" y2="11"></line>
            </svg>
            Expand Preview
          </span>
        </div>
      </div>
      <div class="sci-card-body">
        <div class="sci-card-top-bar">
          <span class="sci-card-fig-num">FIG 0${idx + 1}</span>
          <span class="sci-card-date">${item.date}</span>
        </div>
        <h3 class="sci-card-title">${item.title}</h3>
        <p class="sci-card-desc">${item.description}</p>
        <div class="sci-card-footer">
          <span class="sci-card-tag">${item.tags && item.tags[0] ? item.tags[0] : 'Illustration'}</span>
          <span class="sci-card-action">View Figure <span class="sci-arrow">&rarr;</span></span>
        </div>
      </div>
    </div>
  `).join('');
}

function openSciModal(index) {
  const item = scientificIllustrations[index];
  if (!item) return;

  const modalTitle = document.getElementById('sciModalTitle');
  const modalDate = document.getElementById('sciModalDate');
  const modalTags = document.getElementById('sciModalTags');
  const modalImg = document.getElementById('sciModalImg');
  const modalDesc = document.getElementById('sciModalDesc');
  const fullViewBtn = document.getElementById('sciModalFullView');
  const downloadBtn = document.getElementById('sciModalDownload');
  const modalOverlay = document.getElementById('illustrationModal');

  if (modalTitle) modalTitle.innerText = item.title;
  if (modalDate) modalDate.innerText = item.date || '';
  if (modalTags) {
    modalTags.innerHTML = (item.tags || []).map(tag => `<span class="sci-tag-pill">${tag}</span>`).join('');
  }

  if (modalImg) {
    modalImg.src = item.image;
    modalImg.alt = item.title;
  }
  if (modalDesc) modalDesc.innerText = item.description || '';

  if (fullViewBtn) {
    fullViewBtn.href = item.image;
  }
  if (downloadBtn) {
    downloadBtn.href = item.download || item.image;
    downloadBtn.setAttribute('download', item.download ? item.download.split('/').pop() : item.image.split('/').pop());
  }

  if (modalOverlay) {
    modalOverlay.classList.add('active');
  }
  document.body.style.overflow = 'hidden';
}

function closeSciModal() {
  const modalOverlay = document.getElementById('illustrationModal');
  if (modalOverlay) {
    modalOverlay.classList.remove('active');
  }
  document.body.style.overflow = '';
}

document.addEventListener('DOMContentLoaded', function() {
  renderPortfolioGrid();
  
  const modalOverlay = document.getElementById('illustrationModal');
  if (modalOverlay) {
    modalOverlay.addEventListener('click', function(e) {
      if (e.target === modalOverlay) {
        closeSciModal();
      }
    });
  }
});

document.addEventListener('keydown', function(e) {
  if (e.key === 'Escape') {
    closeSciModal();
  }
});

if (document.readyState === 'interactive' || document.readyState === 'complete') {
  renderPortfolioGrid();
}
</script>
