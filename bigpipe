<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BigPipe Example</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f4f4;
      margin: 0;
      padding: 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .pagelet {
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      margin: 20px;
      padding: 20px;
      color: #333;
      background-color: #fff;
      width: 300px;
      text-align: center;
    }

    .pagelet1 { background-color: #3498db; color: #fff; }
    .pagelet2 { background-color: #e74c3c; color: #fff; }
    .pagelet3 { background-color: #2ecc71; color: #fff; }
  </style>
</head>
<body>
  <div id="pagelet-container"></div>

  <script>
    function simulateServerDelay() {
      return new Promise(resolve => setTimeout(resolve, 2000));
    }

    function renderPagelet(id, content, className) {
      const container = document.getElementById('pagelet-container');
      const pagelet = document.createElement('div');
     ` pagelet.className = pagelet ${className};`
      pagelet.id = id;
      pagelet.innerHTML = content;
      container.appendChild(pagelet);
    }

    async function loadPage() {
      await simulateServerDelay();
      renderPagelet('pagelet1', '<h2>Pagelet 1</h2><p>This is the content of pagelet 1.</p>', 'pagelet1');
      await simulateServerDelay();
      renderPagelet('pagelet2', '<h2>Pagelet 2</h2><p>This is the content of pagelet 2.</p>', 'pagelet2');
      await simulateServerDelay();
      renderPagelet('pagelet3', '<h2>Pagelet 3</h2><p>This is the content of pagelet 3.</p>', 'pagelet3');
    }

    window.onload = loadPage;
  </script>
</body>
</html>
