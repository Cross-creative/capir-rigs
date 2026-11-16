# Animator Bench

[English](#english) | [Português](#português)

---

## English

> A catalog of rigs, resources, plugins/programs and videos for animators.

### About

Animator Bench is a static website (a single HTML file) that works as a catalog for animators. It is hosted on GitHub Pages and uses a JSON file in this repository (rigs.json) as its database, so no backend is needed. Source code: https://github.com/Cross-creative/capir-rigs

### Features

- Four sections: Rigs, Resources, Plugins/Programs and Videos.
- Search by name or description and filter by category.
- Creator area to add, edit, move and remove items, saving straight to the repository through the GitHub API.
- Smart buttons: file links show "Download", while pages such as the Roblox Marketplace show "View".
- Automatic file size and format detection for GitHub Releases links.
- Video previews for YouTube links and direct .mp4, .webm and .ogg files.
- Interactive stick figure in the header (drag it like jelly).
- Language switch (English / Portuguese) with automatic detection, and optional texts in both languages for every item.
- Responsive layout, keyboard focus styles and reduced-motion support.

### Files

- index.html: the whole site (HTML, CSS and JavaScript).
- icon.gif and icon.png: site icon (animated and static).
- favicon.png: browser tab icon.
- rigs.json: the catalog data, created automatically on the first save from the Creator area.
- LICENSE: GNU AGPL v3.
- README.md and README.txt: this file.

### Setup

1. Put the files in the root of the main branch of your repository.
2. At the top of the script in index.html, set GITHUB_OWNER, GITHUB_REPO, GITHUB_BRANCH and DATA_PATH.
3. Enable GitHub Pages: Settings > Pages > Deploy from a branch > main / (root).
4. Upload your files to a Release (Releases > Draft a new release) and use the asset download links.
5. Create a fine-grained personal access token limited to this repository, with the permission Contents: Read and write.
6. Open the site, click "Creator area", paste the token and start adding items.

The token is only kept in memory while the page is open. It is never stored or written to the code, and reloading the page signs you out.

### Data format

rigs.json holds two lists. The "section" field of an item can be rigs, resources or plugins. Items without it are treated as rigs. Texts can be written in both languages with namePt, descriptionPt and titlePt; the site shows the other language when one is empty.

```json
{
  "rigs": [
    {
      "id": "rig-1",
      "section": "rigs",
      "name": "BetterR6",
      "namePt": "BetterR6",
      "kind": "R6",
      "format": ".blend",
      "size": "1.87 MB",
      "description": "Short description.",
      "descriptionPt": "Descrição curta.",
      "url": "https://github.com/OWNER/REPO/releases/download/Rig/file.blend"
    }
  ],
  "videos": [
    {
      "id": "video-1",
      "title": "Rig setup walkthrough",
      "titlePt": "Tutorial de configuração do rig",
      "description": "Short description.",
      "descriptionPt": "Descrição curta.",
      "url": "https://www.youtube.com/watch?v=VIDEO_ID"
    }
  ]
}
```

### Content and credits

The license below covers the source code of the site only. Rigs, resources, plugins and videos listed in the catalog belong to their respective creators and may have their own licenses. Only publish files you have permission to share, and give credit to the authors. If you own something listed here and want it removed, please open an issue.

### License

Copyright (C) 2026 Cross Creative & Capis. This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License, version 3, as published by the Free Software Foundation. It is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the LICENSE file for the full text.

Because this is the AGPL, if you modify the site and host it for other people, you must offer your visitors the source code of your version. The icon in the header links to the repository set in GITHUB_OWNER and GITHUB_REPO, so point those to your own repository.

---

## Português

> Um catálogo de rigs, recursos, plugins/programas e vídeos para animadores.

### Sobre

O Animator Bench é um site estático (um único arquivo HTML) que funciona como catálogo para animadores. Ele fica hospedado no GitHub Pages e usa um arquivo JSON deste repositório (rigs.json) como banco de dados, então não precisa de servidor. Código-fonte: https://github.com/Cross-creative/capir-rigs

### Recursos

- Quatro seções: Rigs, Resources, Plugins/Programs e Videos.
- Busca por nome ou descrição e filtro por categoria.
- Área do criador para adicionar, editar, mover e remover itens, salvando direto no repositório pela API do GitHub.
- Botões inteligentes: links de arquivo mostram "Download", e páginas como o Roblox Marketplace mostram "View".
- Detecção automática de tamanho e formato para links do GitHub Releases.
- Prévia de vídeo para links do YouTube e arquivos .mp4, .webm e .ogg diretos.
- Boneco interativo no topo da página (arraste como se fosse gelatina).
- Seletor de idioma (inglês / português) com detecção automática e textos opcionais nos dois idiomas em cada item.
- Layout responsivo, foco visível no teclado e suporte a movimento reduzido.

### Arquivos

- index.html: o site inteiro (HTML, CSS e JavaScript).
- icon.gif e icon.png: ícone do site (animado e estático).
- favicon.png: ícone da aba do navegador.
- rigs.json: os dados do catálogo, criado automaticamente no primeiro salvamento pela área do criador.
- LICENSE: GNU AGPL v3.
- README.md e README.txt: este arquivo.

### Instalação

1. Coloque os arquivos na raiz da branch main do seu repositório.
2. No topo do script do index.html, defina GITHUB_OWNER, GITHUB_REPO, GITHUB_BRANCH e DATA_PATH.
3. Ative o GitHub Pages: Settings > Pages > Deploy from a branch > main / (root).
4. Envie seus arquivos para uma Release (Releases > Draft a new release) e use os links de download dos arquivos.
5. Crie um token de acesso pessoal fine-grained limitado a este repositório, com a permissão Contents: Read and write.
6. Abra o site, clique em "Creator area", cole o token e comece a adicionar itens.

O token fica só na memória enquanto a página está aberta. Ele nunca é guardado nem escrito no código, e recarregar a página encerra o acesso.

### Formato dos dados

O rigs.json tem duas listas. O campo "section" de um item pode ser rigs, resources ou plugins. Itens sem ele são tratados como rigs. Os textos podem ter versão em português com namePt, descriptionPt e titlePt; o site mostra o outro idioma quando um deles estiver vazio.

```json
{
  "rigs": [
    {
      "id": "rig-1",
      "section": "rigs",
      "name": "BetterR6",
      "namePt": "BetterR6",
      "kind": "R6",
      "format": ".blend",
      "size": "1.87 MB",
      "description": "Short description.",
      "descriptionPt": "Descrição curta.",
      "url": "https://github.com/OWNER/REPO/releases/download/Rig/file.blend"
    }
  ],
  "videos": [
    {
      "id": "video-1",
      "title": "Rig setup walkthrough",
      "titlePt": "Tutorial de configuração do rig",
      "description": "Short description.",
      "descriptionPt": "Descrição curta.",
      "url": "https://www.youtube.com/watch?v=VIDEO_ID"
    }
  ]
}
```

### Conteúdo e créditos

A licença abaixo cobre somente o código-fonte do site. Rigs, recursos, plugins e vídeos listados no catálogo pertencem aos seus respectivos criadores e podem ter licenças próprias. Publique apenas arquivos que você tem permissão para compartilhar e dê o crédito aos autores. Se algo listado aqui é seu e você quer a remoção, abra uma issue.

### Licença

Copyright (C) 2026 Cross Creative & Capis. Este programa é software livre: você pode redistribuí-lo e/ou modificá-lo sob os termos da GNU Affero General Public License, versão 3, publicada pela Free Software Foundation. Ele é distribuído na esperança de que seja útil, mas SEM NENHUMA GARANTIA; sem sequer a garantia implícita de COMERCIALIZAÇÃO ou ADEQUAÇÃO A UM PROPÓSITO ESPECÍFICO. Veja o arquivo LICENSE para o texto completo.

Como a licença é a AGPL, se você modificar o site e hospedá-lo para outras pessoas, precisa oferecer o código-fonte da sua versão aos visitantes. O ícone do topo leva ao repositório definido em GITHUB_OWNER e GITHUB_REPO, então aponte essas constantes para o seu próprio repositório.
