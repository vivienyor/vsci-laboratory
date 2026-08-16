---
title: Vivien Yor • VSCI Laboratory
weight: 1
---

# Vivien Yor • VSCI Laboratory

Independent analysis of geopolitics, technology, and global processes

### Recent Analysis

<script>
  (function() {
    function killNotFound() {
      // Находим вообще все элементы на странице
      const elements = document.querySelectorAll('*');
      elements.forEach(el => {
        // Если внутри элемента написано "Not Found" — полностью стираем его
        if (el.textContent.trim() === "Not Found" || el.innerText === "Not Found") {
          el.style.display = 'none';
          el.style.opacity = '0';
          el.style.visibility = 'hidden';
          el.innerHTML = '';
        }
      });
    }
    // Запускаем проверку сразу и повторно через секунду для надежности
    killNotFound();
    setTimeout(killNotFound, 500);
    setTimeout(killNotFound, 1500);
  })();
</script>
<script>
  (function() {
    function cleanVsciStream() {
      // 1. Стираем текстовые упоминания Not Found
      const allElements = document.querySelectorAll('*');
      allElements.forEach(function(el) {
        if (el.textContent.trim() === "Not Found" || el.innerText === "Not Found") {
          el.style.display = 'none';
          el.innerHTML = '';
        }
      });

      // 2. Вырезаем дубликаты главной страницы из списка автоматических новостей
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
