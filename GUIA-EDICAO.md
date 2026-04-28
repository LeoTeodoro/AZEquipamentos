# Guia de Edição - Site AZ Equipamentos de Pesca

Este guia explica como substituir os marcadores (placeholders) no código `index.html` para preencher o site com o conteúdo e as imagens reais da AZ Equipamentos de Pesca.

Para editar o site, abra o arquivo `index.html` em qualquer editor de código ou texto (como VS Code, Notepad++ ou Sublime Text). Pressione `Ctrl + F` (ou `Cmd + F` no Mac) para buscar os nomes dos placeholders.

## 1. Identidade e Imagens Globais
- `[LOGO_AZ]` -> Substitua pelo caminho da imagem do logotipo. Ex: `assets/img/logo-az.png`
- `[FOTO_HERO_PRINCIPAL]` -> Imagem gigante do topo. **Atenção:** Na seção `<style>`, busque por `url('...[FOTO_HERO_PRINCIPAL]...')` e substitua a URL inteira pelo caminho da sua imagem real.
- `[FOTO_VARA_LATERAL]` -> Imagem na seção "Um novo conceito...". Ex: `assets/img/vara-detalhe.jpg`
- `[FOTO_CTA_FINAL]` -> Imagem de fundo do bloco vermelho no final. Substitua na área de `<style>` assim como a imagem Hero.

## 2. Seção de Modelos (Repita para MODELO_1, MODELO_2, MODELO_3)
- `[FOTO_MODELO_X]` -> Caminho da foto de demonstração do modelo
- `[NOME_MODELO_X]` -> Ex: *Smart-flex 1.8m*
- `[DESCRICAO_MODELO_X]` -> Breve descrição. Ex: *Ideal para pescaria leve em rios e pesqueiros.*
- `[COMPRIMENTO_X]` -> Ex: *1.80 metros*
- `[PESO_X]` -> Ex: *150g*
- `[RESISTENCIA_X]` -> Ex: *10-20 lbs*
- `[MATERIAL_X]` -> Ex: *Carbono Tubular*
- `[LINK_ML_MODELO_X]` -> O link exato do seu anúncio no Mercado Livre para aquele modelo específico.

## 3. Galeria de Fotos
- `[FOTO_GALERIA_X]` -> Caminho da foto em resolução normal (aparece no site)
- `[FOTO_GALERIA_X_FULL]` -> Caminho da foto em ALTA resolução (abre ao clicar)
- **Como adicionar mais:** Copie o bloco inteiro que começa com `<a href="..." data-fancybox="gallery" ...>` e cole logo abaixo dele.

## 4. Seção de Vídeos
- `[YOUTUBE_ID_VIDEO_X]` -> Copie apenas o ID do vídeo do YouTube. 
  - Exemplo: Se o link for `https://www.youtube.com/watch?v=dQw4w9WgXcQ`, o ID é **`dQw4w9WgXcQ`**.
- **Como adicionar mais:** Duplique o bloco `<div class="video-card">...</div>`.

## 5. Prova Social e Contadores Numéricos
**Importante:** Para a animação do contador funcionar perfeitamente, insira APENAS números nos `data-target`.
- `[NUMERO_PESCADORES]` -> Ex: `5000`
- `[ANOS_DESENVOLVIMENTO]` -> Ex: `3`
- `[TAMANHOS_DISPONIVEIS]` -> Ex: `3`

**Depoimentos:**
- `[FOTO_DEPOIMENTO_X]` -> Foto do rosto do cliente. Ex: `assets/img/cliente1.jpg`
- `[NOME_PESCADOR_X]` -> Ex: *João da Silva*
- `[TEXTO_DEPOIMENTO_X]` -> Ex: *A melhor vara que já usei na minha vida!*
- `[CIDADE_X]` -> Ex: *Belo Horizonte - MG*

## 6. Footer (Rodapé)
- `[LINK_INSTAGRAM]` -> Ex: `https://instagram.com/azpesca`
- `[LINK_YOUTUBE]` -> Ex: `https://youtube.com/@azpesca`
- `[LINK_WHATSAPP]` -> Ex: `https://wa.me/5531999999999`