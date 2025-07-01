name: Deploy sitio Nissan

on:
  push:
    branches:
      - main

permissions:
  contents: read
  pages: write
  id-token: write

concurrency:
  group: "pages"
  cancel-in-progress: false

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Clonar repositorio
        uses: actions/checkout@v3

      - name: Configurar GitHub Pages
        uses: actions/configure-pages@v4

      - name: Subir contenido
        uses: actions/upload-pages-artifact@v2
        with:
          path: .  # Aquí apunta a la raíz, donde está tu index.html

  deploy:
    needs: build
    runs-on: ubuntu-latest
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}

    steps:
      - name: Publicar en GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4
