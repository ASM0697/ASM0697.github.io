---
title: "Scientific Illustrations Portfolio"
url: "/gallery/scientific-illustrations-portfolio/"
summary: "Feel free to use my scientific illustartions for any academic purpose! Enjoy! 💙"
show_date: false
show_time: false
show_read_time: false
reading_time: false
image:
  filename: "featured.png"
  focal_point: "center"
  preview_only: true
---

{{< rawhtml >}}
<style>
/* THIS PAGE ONLY: Override ALL Hugo/Tailwind max-width constraints on parent elements */
.max-w-prose,
.max-w-3xl,
.max-w-4xl,
.max-w-5xl,
.max-w-6xl,
.max-w-7xl,
.max-w-screen-xl,
.article-container,
.article-style,
.prose,
main,
article,
section,
.page-body,
.universal-wrapper,
div.mx-auto {
  max-width: 100% !important;
  width: 100% !important;
  box-sizing: border-box !important;
}

/* Page Header spacing */
.article-header, article header, .page-header {
  margin-bottom: 0 !important;
  padding-bottom: 0 !important;
}
.article-title, article header h1, h1, h1.article-title, .page-header h1 {
  margin-bottom: 0 !important;
  padding-bottom: 0 !important;
}

/* Subtitle: SMALL tight space under Title, clear space above Card Blocks */
.portfolio-subtitle {
  margin-top: -1.2rem !important;
  margin-bottom: 2.5rem !important;
  padding-top: 0 !important;
  font-style: italic;
  font-size: 1.08rem;
  color: var(--color-footer-fg, #64748b);
  text-align: center;
}

/* COLLECTION CONTAINER: Full viewport breakout to maximize horizontal card width */
.portfolio-container, .collection-container {
  width: 98vw !important;
  max-width: 100% !important;
  margin-left: calc(50% - 49vw) !important;
  margin-right: calc(50% - 49vw) !important;
  margin-top: 1.5rem !important;
  margin-bottom: 3.5rem !important;
  padding-left: 0.5rem !important;
  padding-right: 0.5rem !important;
  box-sizing: border-box !important;
}

/* COLLECTION GRID: 5 Columns per row on desktop screens */
.collection, .portfolio-grid {
  display: grid !important;
  grid-template-columns: repeat(5, 1fr) !important;
  gap: 1rem !important;
  width: 100% !important;
}

@media (max-width: 1400px) and (min-width: 1080px) {
  .collection, .portfolio-grid {
    grid-template-columns: repeat(4, 1fr) !important;
    gap: 0.9rem !important;
  }
}

@media (max-width: 1079px) and (min-width: 720px) {
  .collection, .portfolio-grid {
    grid-template-columns: repeat(3, 1fr) !important;
    gap: 0.85rem !important;
  }
}

@media (max-width: 719px) and (min-width: 480px) {
  .collection, .portfolio-grid {
    grid-template-columns: repeat(2, 1fr) !important;
    gap: 0.75rem !important;
  }
}

@media (max-width: 479px) {
  .collection, .portfolio-grid {
    grid-template-columns: 1fr !important;
    gap: 0.75rem !important;
  }
}

/* THIS PAGE ONLY: Card Styling - Shorter, wider, sleek compact blocks */
.sci-card, .collection-card {
  display: flex !important;
  flex-direction: column !important;
  border-radius: 14px !important;
  overflow: hidden !important;
  box-sizing: border-box !important;
  background: #ffffff !important;
  border: 1px solid rgba(0, 0, 0, 0.08) !important;
  box-shadow: 0 4px 18px rgba(0, 0, 0, 0.05), 0 1px 3px rgba(0, 0, 0, 0.03) !important;
  transition: transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1), box-shadow 0.3s ease !important;
  width: 100% !important;
}

.dark .sci-card,
html.dark .sci-card,
body.dark .sci-card,
[data-wc-theme-default="dark"] .sci-card {
  background: #1e2535 !important;
  border: 1px solid rgba(255, 255, 255, 0.08) !important;
  box-shadow: 0 4px 18px rgba(0, 0, 0, 0.3) !important;
}

.sci-card:hover, .collection-card:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 10px 28px rgba(0, 0, 0, 0.1), 0 2px 5px rgba(0, 0, 0, 0.05) !important;
}

.dark .sci-card:hover,
html.dark .sci-card:hover,
body.dark .sci-card:hover {
  box-shadow: 0 10px 28px rgba(0, 0, 0, 0.5) !important;
}

/* THIS PAGE ONLY: Shorter Cover Image Height (~140px for sleek compact ratio) */
.sci-card-img-wrapper {
  position: relative !important;
  width: 100% !important;
  height: 140px !important;
  overflow: hidden !important;
  border-radius: 14px 14px 0 0 !important;
  margin: 0 !important;
  padding: 5px !important;
  box-sizing: border-box !important;
  transition: background 0.3s ease, border-color 0.3s ease;
  background: #f1f5f9 !important;
  border-bottom: 1px solid #e2e8f0 !important;
}

.dark .sci-card-img-wrapper,
html.dark .sci-card-img-wrapper,
body.dark .sci-card-img-wrapper,
[data-wc-theme-default="dark"] .sci-card-img-wrapper {
  background: #161b22 !important;
  border-bottom: 1px solid rgba(255, 255, 255, 0.12) !important;
}

.sci-card-img-wrapper img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  object-position: center !important;
  display: block !important;
  border-radius: 9px !important;
  margin: 0 !important;
  padding: 0 !important;
  box-sizing: border-box !important;
  border: 1px solid rgba(0, 0, 0, 0.06) !important;
}

.dark .sci-card-img-wrapper img,
html.dark .sci-card-img-wrapper img,
body.dark .sci-card-img-wrapper img {
  border: 1px solid rgba(255, 255, 255, 0.1) !important;
}

/* THIS PAGE ONLY: Shorter, Compact Card Body Padding & Elements */
.sci-card-body {
  padding: 0.75rem 0.9rem 0.9rem 0.9rem !important;
  display: flex !important;
  flex-direction: column !important;
  flex: 1 1 auto !important;
}

.sci-card-top-bar {
  display: flex !important;
  justify-content: space-between !important;
  align-items: center !important;
  margin-bottom: 0.35rem !important;
}

.sci-card-fig-num {
  font-size: 0.72rem !important;
  font-weight: 700 !important;
  padding: 0.15rem 0.5rem !important;
  border-radius: 5px !important;
  white-space: nowrap !important;
}

.sci-card-date {
  font-size: 0.75rem !important;
  white-space: nowrap !important;
}

.sci-card-title {
  font-size: 0.92rem !important;
  font-weight: 700 !important;
  line-height: 1.28 !important;
  margin-bottom: 0.35rem !important;
  display: -webkit-box !important;
  -webkit-line-clamp: 2 !important;
  -webkit-box-orient: vertical !important;
  overflow: hidden !important;
}

.sci-card-desc {
  font-size: 0.78rem !important;
  line-height: 1.35 !important;
  margin-bottom: 0.55rem !important;
  color: var(--color-footer-fg, #64748b) !important;
  display: -webkit-box !important;
  -webkit-line-clamp: 2 !important;
  -webkit-box-orient: vertical !important;
  overflow: hidden !important;
}

.sci-card-tags-list {
  display: flex !important;
  flex-wrap: wrap !important;
  gap: 0.25rem !important;
  margin-bottom: 0.55rem !important;
}

.sci-tag-pill {
  padding: 0.15rem 0.52rem !important;
  font-size: 0.68rem !important;
  border-radius: 999px !important;
}

.sci-card-footer {
  margin-top: auto !important;
  width: 100% !important;
}

.sci-preview-btn {
  width: 100% !important;
  padding: 0.4rem 0.8rem !important;
  font-size: 0.8rem !important;
  font-weight: 600 !important;
  display: flex !important;
  justify-content: center !important;
  align-items: center !important;
  gap: 0.35rem !important;
  border-radius: 8px !important;
}

/* THIS PAGE ONLY: Force footer to span 100% full width and center text matching rest of site */
body.page-wrapper footer, footer.site-footer, footer, .page-footer {
  width: 100% !important;
  max-width: 100% !important;
  margin-left: 0 !important;
  margin-right: 0 !important;
  padding-left: 0 !important;
  padding-right: 0 !important;
  text-align: center !important;
  box-sizing: border-box !important;
}

body.page-wrapper footer .container, footer .container, footer > div, .page-footer > div {
  max-width: 100% !important;
  width: 100% !important;
  margin: 0 auto !important;
  text-align: center !important;
  padding-left: 0 !important;
  padding-right: 0 !important;
}
</style>

<p class="portfolio-subtitle" style="text-align: center;"><em>Feel free to use my scientific illustartions for any academic purpose! Enjoy! 💙</em></p>

<div class="portfolio-container collection-container">
<div id="portfolioGrid" class="collection portfolio-grid">

<!-- Block 1 -->
<div class="sci-card collection-card" onclick="openSciModal(0)" role="button" tabindex="0" aria-label="View Metabolic Disorders, Autonomic Immune Dysfunction, and Ferroptosis">
<div class="sci-card-img-wrapper">
<img src="thumb_obesity.png" alt="Metabolic Disorders, Autonomic Immune Dysfunction, and Ferroptosis" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 01</span>
<span class="sci-card-date">Sept 2025</span>
</div>
<h3 class="sci-card-title">Metabolic Disorders, Autonomic Immune Dysfunction, and Ferroptosis</h3>
<p class="sci-card-desc">Integrative molecular signaling map illustrating how chronic nutrient overload, visceral white adipose tissue (vWAT) inflammation, and autonomic nerve impairment interact to drive iron-dependent ferroptosis across metabolic organs.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">Ferroptosis</span>
<span class="sci-tag-pill">Metabolic Disorders</span>
<span class="sci-tag-pill">Illustrations</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(0); event.stopPropagation();" aria-label="Preview Metabolic Disorders illustration">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

<!-- Block 2 -->
<div class="sci-card collection-card" onclick="openSciModal(1)" role="button" tabindex="0" aria-label="View Visceral Adipose Tissue (vWAT) Inflammation">
<div class="sci-card-img-wrapper">
<img src="ferroptosis_disufidptosis.jpg" alt="SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 02</span>
<span class="sci-card-date">Mar 2026</span>
</div>
<h3 class="sci-card-title">SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases</h3>
<p class="sci-card-desc">Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">SLC7A11</span>
<span class="sci-tag-pill">Ferroptosis</span>
<span class="sci-tag-pill">Disulfidptosis</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(1); event.stopPropagation();" aria-label="Preview Visceral Adipose Tissue illustration">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

<!-- Block 3 -->
<div class="sci-card collection-card" onclick="openSciModal(2)" role="button" tabindex="0" aria-label="View Betanin-Mediated Modulation of miRNA Signaling and Neuroinflammation in Inflammatory Pain">
<div class="sci-card-img-wrapper">
<img src="Betanin_proposed_analgesic_mechanism.png" alt="Betanin-Mediated Modulation of miRNA Signaling and Neuroinflammation in Inflammatory Pain" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 03</span>
<span class="sci-card-date">July 2025</span>
</div>
<h3 class="sci-card-title">Betanin-Mediated Modulation of miRNA Signaling and Neuroinflammation in Inflammatory Pain</h3>
<p class="sci-card-desc">Proposed molecular mechanism illustrating how betanin may attenuate inflammatory pain through modulation of miR-107/GLT-1 and miR-145/Akt signaling, with downstream effects on glutamate accumulation, oxidative stress, and inflammatory cytokines.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">Betanin</span>
<span class="sci-tag-pill">Pain</span>
<span class="sci-tag-pill">miRNA</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(2); event.stopPropagation();" aria-label="Preview Betanin-Mediated Modulation of miRNA Signaling and Neuroinflammation in Inflammatory Pain">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

<!-- Block 4 -->
<div class="sci-card collection-card" onclick="openSciModal(1)" role="button" tabindex="0" aria-label="View Visceral Adipose Tissue (vWAT) Inflammation">
<div class="sci-card-img-wrapper">
<img src="ferroptosis_disufidptosis.jpg" alt="SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 02</span>
<span class="sci-card-date">Mar 2026</span>
</div>
<h3 class="sci-card-title">SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases</h3>
<p class="sci-card-desc">Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">SLC7A11</span>
<span class="sci-tag-pill">Ferroptosis</span>
<span class="sci-tag-pill">Disulfidptosis</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(1); event.stopPropagation();" aria-label="Preview Visceral Adipose Tissue illustration">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

<!-- Block 5 -->
<div class="sci-card collection-card" onclick="openSciModal(1)" role="button" tabindex="0" aria-label="View Visceral Adipose Tissue (vWAT) Inflammation">
<div class="sci-card-img-wrapper">
<img src="ferroptosis_disufidptosis.jpg" alt="SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 02</span>
<span class="sci-card-date">Mar 2026</span>
</div>
<h3 class="sci-card-title">SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases</h3>
<p class="sci-card-desc">Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">SLC7A11</span>
<span class="sci-tag-pill">Ferroptosis</span>
<span class="sci-tag-pill">Disulfidptosis</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(1); event.stopPropagation();" aria-label="Preview Visceral Adipose Tissue illustration">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

<!-- Block 6 -->
<div class="sci-card" onclick="openSciModal(1)" role="button" tabindex="0" aria-label="View Visceral Adipose Tissue (vWAT) Inflammation">
<div class="sci-card-img-wrapper">
<img src="ferroptosis_disufidptosis.jpg" alt="SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases" loading="lazy" />
<div class="sci-card-hover-overlay">
<span class="sci-preview-badge">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</span>
</div>
</div>
<div class="sci-card-body">
<div class="sci-card-top-bar">
<span class="sci-card-fig-num">FIG 02</span>
<span class="sci-card-date">Mar 2026</span>
</div>
<h3 class="sci-card-title">SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases</h3>
<p class="sci-card-desc">Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases.</p>
<div class="sci-card-tags-list">
<span class="sci-tag-pill">SLC7A11</span>
<span class="sci-tag-pill">Ferroptosis</span>
<span class="sci-tag-pill">Disulfidptosis</span>
</div>
<div class="sci-card-footer">
<button class="sci-preview-btn" onclick="openSciModal(1); event.stopPropagation();" aria-label="Preview Visceral Adipose Tissue illustration">
<svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
<circle cx="11" cy="11" r="8"></circle>
<line x1="21" y1="21" x2="16.65" y2="16.65"></line>
<line x1="11" y1="8" x2="11" y2="14"></line>
<line x1="8" y1="11" x2="14" y2="11"></line>
</svg>
Preview
</button>
</div>
</div>
</div>

</div>
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
{{< /rawhtml >}}

<script>
const scientificIllustrations = [
  {
    id: "fig-1",
    title: "Metabolic Disorders, Autonomic Immune Dysfunction, and Ferroptosis",
    date: "Sept 2025",
    tags: ["Ferroptosis", "Metabolic Disorders", "Illustrations"],
    image: "featured.png",
    download: "featured.png",
    description: "Integrative molecular signaling map illustrating how chronic nutrient overload, visceral white adipose tissue (vWAT) inflammation, and autonomic nerve impairment interact to drive iron-dependent ferroptosis across metabolic organs."
  },
  {
    id: "fig-2",
    title: "SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases",
    date: "Aug 2025",
    tags: ["SLC7A11", "Ferroptosis", "Disulfidptosis"],
    image: "ferroptosis_disufidptosis.jpg",
    download: "ferroptosis_disufidptosis.jpg",
    description: "Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases."
  },
  {
    id: "fig-3",
    title: "Betanin-Mediated Modulation of miRNA Signaling and Neuroinflammation in Inflammatory Pain",
    date: "Feb 2026",
    tags: ["Betanin", "Pain", "miRNA"],
    image: "Betanin_proposed_analgesic_mechanism.png",
    download: "Betanin_proposed_analgesic_mechanism.png",
    description: "Proposed molecular mechanism illustrating how betanin may attenuate inflammatory pain through modulation of miR-107/GLT-1 and miR-145/Akt signaling, with downstream effects on glutamate accumulation, oxidative stress, and inflammatory cytokines."
  },
  {
    id: "fig-4",
    title: "SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases",
    date: "Aug 2025",
    tags: ["SLC7A11", "Ferroptosis", "Disulfidptosis"],
    image: "ferroptosis_disufidptosis.jpg",
    download: "ferroptosis_disufidptosis.jpg",
    description: "Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases."
  },
  {
    id: "fig-5",
    title: "SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases",
    date: "Aug 2025",
    tags: ["SLC7A11", "Ferroptosis", "Disulfidptosis"],
    image: "ferroptosis_disufidptosis.jpg",
    download: "ferroptosis_disufidptosis.jpg",
    description: "Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases."
  },
  {
    id: "fig-6",
    title: "SLC7A11 Redox Homeostasis, Ferroptosis, and Disulfidptosis in Neurodegenerative Diseases",
    date: "Aug 2025",
    tags: ["SLC7A11", "Ferroptosis", "Disulfidptosis"],
    image: "ferroptosis_disufidptosis.jpg",
    download: "ferroptosis_disufidptosis.jpg",
    description: "Schematic overview illustrating how SLC7A11 regulates redox homeostasis and neuronal survival, with its dysregulation driving ferroptosis or disulfidptosis in neurodegenerative diseases."
  }
];

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
</script>
