<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Item Viewer</title>
  <style>
    body { font-family: sans-serif; padding: 20px; }
    input, button { margin: 5px 0; padding: 8px; width: 300px; }
    #carousel img { width: 150px; height: auto; cursor: pointer; }
    #carousel div { display: inline-block; margin: 10px; text-align: center; }
  </style>
</head>
<body>
  <h2>Item Viewer</h2>
  <input type="text" id="itemId" placeholder="Enter Item ID"><br>
  <input type="text" id="apiKey" placeholder="Enter API Key"><br>
  <button onclick="fetchItem()">Submit</button>

  <div id="result" style="margin-top: 20px;"></div>

  <script>
    async function fetchItem() {
      const itemId = document.getElementById('itemId').value;
      const apiKey = document.getElementById('apiKey').value;
      const resultDiv = document.getElementById('result');
      resultDiv.innerHTML = "Loading...";

      try {
        const res = await fetch(`https://new.selectika-new-infrastructure.selectika.com/ask/${itemId}/sbi`, {
          headers: { 'Authorization': `Bearer ${apiKey}` }
        });

        if (!res.ok) throw new Error("Request failed");
        const data = await res.json();

        const ref = data.referenceItem;
        const items = data.items.slice(0, 5);

        let html = `
          <h3>Reference Item</h3>
          <a href="${ref.page_url}" target="_blank">
            <img src="${ref.images[0].url}" width="200"><br>${ref.item_id}
          </a>
          <h3>Recommended Items</h3>
          <div id="carousel">
        `;

        for (const item of items) {
          html += `
            <div>
              <a href="${item.page_url}" target="_blank">
                <img src="${item.images[0].url}">
              </a>
              <div>${item.item_id}</div>
            </div>
          `;
        }

        html += "</div>";
        resultDiv.innerHTML = html;

      } catch (err) {
        resultDiv.innerHTML = "Error: " + err.message;
      }
    }
  </script>
</body>
</html>
