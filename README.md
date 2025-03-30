# 🎓 Portafolio Grupo 1 - Construcción de Software

Bienvenidos al portafolio del **Grupo 1** de la Universidad Continental. Aquí encontrarán los portafolios individuales de cada integrante.

---

## 🚀 Integrantes del Grupo 1

🔹 **Alex Álvarez Solis**  
📌 [Ver portafolio](https://alexdev8386.github.io/Alvarezdev.github.io/)  

---

## 🔎 Buscar en los Portafolios  

Escribe una palabra clave (como **C#**, **Python**, **Java**) en la barra de búsqueda para encontrar coincidencias en los portafolios de los integrantes.

<input type="text" id="searchInput" placeholder="Buscar por tecnología..." onkeyup="searchPortfolio()">

<div id="searchResults"></div>

---

## 📌 Producto Académico N-01  
🔹 Este portafolio forma parte del trabajo académico de **Construcción de Software** en la **Universidad Continental**.

---

## 📷 Galería  

<img src="https://via.placeholder.com/300x200?text=Grupo+1" alt="Grupo 1">
<img src="https://via.placeholder.com/300x200?text=Proyecto+01" alt="Proyecto 01">

---

## 📜 Créditos  
Grupo 1 - Construcción de Software, Universidad Continental.  
Desarrollado con [GitHub Pages](https://pages.github.com/) y Markdown.

---

## 📜 Código de Búsqueda (JavaScript)
Este código agrega funcionalidad a la barra de búsqueda:

```html
<script>
const portfolios = [
  { name: "Alex Álvarez Solis", url: "https://alvarezdev.github.io", tech: ["C#", "Python"] }
];

function searchPortfolio() {
    let input = document.getElementById('searchInput').value.toLowerCase();
    let resultsDiv = document.getElementById('searchResults');
    resultsDiv.innerHTML = '';

    portfolios.forEach(portfolio => {
        if (portfolio.tech.some(tech => tech.toLowerCase().includes(input))) {
            resultsDiv.innerHTML += `<p><a href="${portfolio.url}" target="_blank">${portfolio.name}</a></p>`;
        }
    });

    if (resultsDiv.innerHTML === '') {
        resultsDiv.innerHTML = '<p>No se encontraron resultados</p>';
    }
}
</script>
