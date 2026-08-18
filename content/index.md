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
## Foundation Research

The mathematical and conceptual models used in this laboratory serve as a direct analytical extension of the fundamental author's monographs:
* **[[атлас_власти|Vivien Yor. Atlas of Power. Volumes I–III (Zenodo, 2026)]]**
* **[[кибербарокко|Vivien Yor. Cybernetic Baroque: Platform Neo-Absolutism and the Geopolitics of Sovereign Code (Zenodo, 2026)]]**
---


### Recent Analysis

<script>
  (function() {
    function killNotFound() {
      const elements = document.querySelectorAll('*');
      elements.forEach(el => {
        if (el.textContent.trim() === "Not Found" || el.innerText === "Not Found") {
          el.style.display = 'none';
          el.style.opacity = '0';
          el.style.visibility = 'hidden';
          el.innerHTML = '';
        }
      });
    }
    killNotFound();
    setTimeout(killNotFound, 500);
    setTimeout(killNotFound, 1500);
  })();
</script>
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
