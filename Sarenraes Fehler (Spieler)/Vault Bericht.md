```dataviewjs
// Chart.js einbinden
if (!window.Chart) {
    const script = document.createElement('script');
    script.src = "https://cdn.jsdelivr.net/npm/chart.js";
    script.type = "text/javascript";
    script.async = true;
    script.onload = () => renderChart(); // Chart.js laden und danach rendern
    document.head.appendChild(script);
} else {
    renderChart(); // Falls Chart.js schon geladen ist
}

// Funktion zur Erstellung des Charts
function renderChart() {
    const pages = dv.pages()  // Option: Narrow down to a subset of pages if needed
        .groupBy(p => p.NoteIcon)
        .filter(p => !!p.key);  // Filter out groups without a NoteIcon property

    // Labels
    const noteTypes = pages.map(p => p.key);
    // Data
    const noteTypesCount = pages.map(p => p.rows.length);

    const chartData = {
        type: 'bar',
        data: {
            labels: noteTypes,
            datasets: [{
                label: 'Count',
                data: noteTypesCount,
                backgroundColor: Array(noteTypes.length).fill('gold'), // Farbe für jedes Element
            }]
        }
    };

    // HTML-Container für das Chart erstellen
    const canvas = this.container.createEl("canvas"); // Neues Canvas-Element
    new Chart(canvas, chartData); // Chart in Canvas rendern
}

```


```dataviewjs
const pages = dv.pages()  // maybe narrow down to a subset of pages
  .groupBy(p => p.NoteIcon)
  .filter(p => !!p.key);  // filter out pages without noteType property

// Labels
const noteTypes = pages.map(p => p.key).values;
// Data
const noteTypesCount = pages.map(p => p.rows.length).values;

const chartData = {
    type: 'bar',
    data: {
        labels: noteTypes,
        datasets: [{
            label: 'Count',
            data: noteTypesCount,
            backgroundColor: [
                'gold'
            ],
        }]
    }
}

window.renderChart(chartData, this.container)
```

