---
title: Vivien Yor • VSCI Laboratory
weight: 1
---

# Vivien Yor • VSCI Laboratory

Independent analysis of geopolitics, technology, and global processes.

---

## Core Operational Framework

The VSCI Laboratory operates as an open-science platform exploring the structural shifts of **Technological Westphalia** and the era of **Cybernetic Baroque**. 

Our quantitative analysis relies on the **VSCI Index (Vivien's Sovereignty & Connectivity Index)**, which measures real infrastructure and data sovereignty across operational tiers.

---

## Measurement Level (The Toolkit)

<div style="padding: 30px; background: var(--light); border: 1px solid var(--lightgray); border-radius: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.04); margin: 25px 0;">

<span style="font-family: monospace; font-size: 0.75rem; color: var(--secondary); text-transform: uppercase; letter-spacing: 2px; font-weight: bold; display: block; text-align: center; margin-bottom: 15px;">Vivien’s Sovereignty & Connectivity Index Matrix</span>

$$VSCI = w_1 \cdot S_{il} + w_2 \cdot S_{ft} + w_3 \cdot E_{ng} + w_4 \cdot D_{at}$$

<p style="text-align: center; font-size: 0.95rem; color: var(--darkgray); max-width: 600px; margin: 15px auto 25px auto; line-height: 1.5;">
  Measures actual technological autarky through calculated weight coefficients across four critical infrastructural layers.
</p>

<hr style="border: 0; border-top: 1px dashed var(--lightgray); margin: 20px 0;">

* **$S_{il}$ • Silicon Layer** — Hardware autarky, semiconductor manufacturing independence, and lithography capacity.
* **$S_{ft}$ • Software Stack** — Independent operating systems, core algorithmic workflows, and auditable processing code.
* **$E_{ng}$ • Energy Grid** — Power infrastructure resilience, computing center supply, and structural grid autonomy.
* **$D_{at}$ • Data Sovereignty** — Structured machine-readable datasets, local storage networks, and cryptographic validation.

</div>

---

## 📚 Foundation Research

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0; width: 100%;">

  <!-- Card 1: Atlas of Power -->
  <div style="padding: 24px; border: 1px solid var(--lightgray); border-radius: 8px; background: var(--light); box-shadow: 0 4px 12px rgba(0,0,0,0.05); display: flex; flex-direction: column; justify-content: space-between; position: relative;">
    <div>
      <span style="font-size: 0.75rem; text-transform: uppercase; color: var(--gray); font-family: monospace; letter-spacing: 1px;">Monograph • Volumes I–III</span>
      <h3 style="margin: 10px 0 12px 0; color: var(--secondary); font-size: 1.4rem;">Atlas of Power</h3>
      <p style="font-size: 0.9rem; line-height: 1.5; margin: 0; color: var(--dark); opacity: 0.85;">A fundamental scientific work laying the methodological foundations of Tech-Realism and the concept of New Westphalia in the 21st century.</p>
    </div>
    <div style="margin-top: 24px; padding: 10px; background: rgba(143, 159, 169, 0.08); border: 1px solid var(--lightgray); border-radius: 6px; font-family: monospace; font-size: 0.8rem; text-align: center; color: var(--secondary); font-weight: bold; letter-spacing: 0.5px;">
      DOI: 10.5281/zenodo.21533111
    </div>
  </div>

  <!-- Card 2: Cybernetic Baroque -->
  <div style="padding: 24px; border: 1px solid var(--lightgray); border-radius: 8px; background: var(--light); box-shadow: 0 4px 12px rgba(0,0,0,0.05); display: flex; flex-direction: column; justify-content: space-between; position: relative;">
    <div>
      <span style="font-size: 0.75rem; text-transform: uppercase; color: var(--gray); font-family: monospace; letter-spacing: 1px;">Monograph • Zenodo 2026</span>
      <h3 style="margin: 10px 0 12px 0; color: var(--secondary); font-size: 1.4rem;">Cybernetic Baroque</h3>
      <p style="font-size: 0.9rem; line-height: 1.5; margin: 0; color: var(--dark); opacity: 0.85;">An in-depth analysis of the structural transformation of global political economy, digital governance, and platform neo-absolutism.</p>
    </div>
    <div style="margin-top: 24px; padding: 10px; background: rgba(143, 159, 169, 0.08); border: 1px solid var(--lightgray); border-radius: 6px; font-family: monospace; font-size: 0.8rem; text-align: center; color: var(--secondary); font-weight: bold; letter-spacing: 0.5px;">
      DOI: 10.5281/zenodo.21669927
    </div>
  </div>

</div>

---

### Recent Analysis

<script>
  (function() {
    function cleanAndFlagVsciStream() {
      // 1. Мягко скрываем "Not Found", не удаляя узлы сетки
      document.querySelectorAll('*').forEach(function(el) {
        if (el.children.length === 0 && (el.textContent.trim() === "Not Found" || el.innerText === "Not Found")) {
          el.style.display = 'none';
        }
      });

      const flags = { 'ru': '🇷🇺', 'en': '🇬🇧', 'fr': '🇫🇷', 'es': '🇪🇸' };

      // 2. Безопасно обрабатываем элементы списков Quartz 5
      const items = document.querySelectorAll('.recent-notes li, [class*="recent-notes"] li, .explorer-item');
      items.forEach(function(item) {
        const link = item.querySelector('a');
        if (link) {
          const href = (link.getAttribute('href') || '').toLowerCase();
          const text = link.textContent.toLowerCase();
          
          // Мягкий фильтр мусора: скрываем, но не очищаем innerHTML
          if (href === '/' || href === './' || href.endsWith('index') || text.includes('vivien yor')) {
            item.style.style.display = 'none';
            return;
          }

          if (!item.dataset.vsciFlagged) {
            let flag = '';
            const fullText = item.textContent.toLowerCase();

            if (fullText.includes('lang-ru') || fullText.includes('language: ru') || href.includes('lang-ru') || text.includes('вестфалия') || text.includes('технореализм')) {
              flag = flags.ru;
            } else if (fullText.includes('lang-en') || fullText.includes('language: en') || href.includes('lang-en')) {
              flag = flags.en;
            } else if (fullText.includes('lang-fr') || fullText.includes('language: fr') || href.includes('lang-fr')) {
              flag = flags.fr;
            } else if (fullText.includes('lang-es') || fullText.includes('language: es') || href.includes('lang-es')) {
              flag = flags.es;
            }

            if (flag) {
              if (!link.textContent.startsWith(flag)) {
                link.textContent = flag + ' ' + link.textContent;
              }
            }
            item.dataset.vsciFlagged = 'true';
          }
        }
      });
    }

    // Привязка к SPA роутеру Quartz 5
    cleanAndFlagVsciStream();
    document.addEventListener("nav", cleanAndFlagVsciStream);
    
    // Страховочные задержки
    setTimeout(cleanAndFlagVsciStream, 100);
    setTimeout(cleanAndFlagVsciStream, 600);
  })();
</script>
