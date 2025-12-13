<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Mécanique Orbitale — Projet</title>

  <!-- KaTeX -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.11/dist/katex.min.css">
  <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.11/dist/katex.min.js"></script>
  <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.11/dist/contrib/auto-render.min.js"></script>

  <style>
    body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial;max-width:980px;margin:40px auto;padding:0 16px;line-height:1.5}
    h1,h2{line-height:1.15}
    .card{border:1px solid #e5e7eb;border-radius:14px;padding:18px;margin:14px 0}
    code{background:#f6f8fa;padding:2px 6px;border-radius:8px}
  </style>
</head>
<body>
  <h1>Projet — Introduction à la mécanique orbitale</h1>
  <p>
    Cette page rend les équations en <b>KaTeX</b> (compatible GitHub Pages).
  </p>

  <div class="card">
    <h2>Géométrie orbitale</h2>
    <p>
      Rayon orbital en fonction de l’anomalie vraie :
      $$ r(\nu)=\frac{a(1-e^2)}{1+e\cos\nu}. $$
    </p>
    <p>
      Estimation de l’excentricité à partir de deux mesures :
      $$ e=\frac{r_2-r_1}{r_1\cos\nu_1-r_2\cos\nu_2}. $$
    </p>
  </div>

  <div class="card">
    <h2>Vitesse & période</h2>
    <p>
      Vis-viva :
      $$ v=\sqrt{\mu\left(\frac{2}{r}-\frac{1}{a}\right)}. $$
    </p>
    <p>
      Période :
      $$ T=2\pi\sqrt{\frac{a^3}{\mu}}. $$
    </p>
  </div>

  <div class="card">
    <h2>Dérives séculaires J2</h2>
    <p>
      Avec \(p=a(1-e^2)\) et \(n=\sqrt{\mu/a^3}\) :
      $$ \dot{\Omega}=-\frac{3}{2}nJ_2\left(\frac{R_T}{p}\right)^2\cos i, $$
      $$ \dot{\omega}=\frac{3}{4}nJ_2\left(\frac{R_T}{p}\right)^2(4-5\sin^2 i). $$
    </p>
  </div>

  <div class="card">
    <h2>Manœuvres & ergols</h2>
    <p>
      Tsiolkovski :
      $$ \Delta V=I_{sp}g_0\ln\left(\frac{m_0}{m_f}\right). $$
    </p>
  </div>

  <script>
    document.addEventListener("DOMContentLoaded", function () {
      renderMathInElement(document.body, {
        delimiters: [
          {left: "$$", right: "$$", display: true},
          {left: "\\[", right: "\\]", display: true},
          {left: "$", right: "$", display: false},
          {left: "\\(", right: "\\)", display: false}
        ],
        throwOnError: false
      });
    });
  </script>
</body>
</html>

