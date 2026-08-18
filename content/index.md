---
title: Vivien Yor • VSCI Laboratory
weight: 1
---

# Vivien Yor • VSCI Laboratory

Independent analysis of geopolitics, technology, and global processes.

---

## Core Operational Framework

The VSCI Laboratory operates as an open-science platform exploring the structural shifts of **Technological Westphalia** and the era of **Cybernetic Baroque**. 

Our quantitative analysis relies on the **VSCI Index (Vivien Yor Sovereignty & Connectivity Index)**, which measures real infrastructure and data sovereignty across three operational tiers. 

For instance, the mathematical matrix for **Border Perimeter Security ($VSCI_{border}$)** is formally defined as:

$$VSCI_{border} = w_1 \cdot M_{supply} + w_2 \cdot M_{digital} + w_3 \cdot M_{logistics}$$

Where a calculated index score above the threshold of **0.75** shifts a national perimeter into the *Vulnerable Sovereign* status.

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
    <div style="margin-top: 20px; font-weight: bold;">
      [[books/атлас_власти|Open Monograph →]]
    </div>
  </div>

  <!-- Card 2: Cybernetic Baroque -->
  <div style="padding: 24px; border: 1px solid var(--lightgray); border-radius: 8px; background: var(--light); box-shadow: 0 4px 12px rgba(0,0,0,0.05); display: flex; flex-direction: column; justify-content: space-between; position: relative;">
    <div>
      <span style="font-size: 0.75rem; text-transform: uppercase; color: var(--gray); font-family: monospace; letter-spacing: 1px;">Monograph • Zenodo 2026</span>
      <h3 style="margin: 10px 0 12px 0; color: var(--secondary); font-size: 1.4rem;">Cybernetic Baroque</h3>
      <p style="font-size: 0.9rem; line-height: 1.5; margin: 0; color: var(--dark); opacity: 0.85;">An in-depth analysis of the structural transformation of global political economy, digital governance, and platform neo-absolutism.</p>
    </div>
    <div style="margin-top: 20px; font-weight: bold;">
      [[books/кибербарокко|Open Monograph →]]
    </div>
  </div>

</div>

---

### Recent Analysis

<script>
  (function() {
    function cleanVsciStream() {
      const allElements = document.querySelectorAll('*');
      allElements.forEach(function(el) {
        if (el.textContent.trim() === "Not Found" || el.innerText === "Not Found") {
          el.style.display = 'none';
          el.innerHTML = '';
        }
      });

      const listItems = document.querySelectorAll('.recent-notes li, [class*="recent-notes"] li');
      listItems.forEach(function(item) {
        const link = item.querySelector('a');
        if (link) {
          const href = link.getAttribute('href') || '';
          const text = link.textContent || '';
          
          if (
            href === '/' || 
            href === './' || 
            href.endsWith('index') || 
            text.includes('Vivien Yor')
          ) {
            item.style.display = 'none';
            item.innerHTML = ''; 
          }
        }
      });
    }

    cleanVsciStream();
    setTimeout(cleanVsciStream, 300);
    setTimeout(cleanVsciStream, 800);
    setTimeout(cleanVsciStream, 1500);
  })();
</script>
