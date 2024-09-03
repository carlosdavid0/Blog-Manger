# Downloads & Animes

Este projeto é um blog de animes e downloads, desenvolvido com o propósito de oferecer uma interface amigável e interativa para fãs de animes. O blog é responsivo e inclui um carrossel de imagens, postagens recentes e navegação por tópicos populares.

## Estrutura de Pastas

A estrutura do projeto é organizada da seguinte forma:

```
├── assets
│   ├── novidades-1.svg
│   ├── novidades-2.svg
│   ├── novidades-3.svg
│   ├── slide1.svg
│   ├── slide2.svg
│   └── slide3.svg
├── blog.css
├── blog.rtl.css
├── estrutura_pasta.txt
├── global.css
├── index.html
└── scripts
    └── bootstrap.bundle.min.js
```

### Descrição dos Arquivos e Pastas

- **assets**: Contém imagens SVG usadas no carrossel e nas seções de novidades do blog.
- **blog.css**: Folha de estilos específica para a estrutura e layout do blog.
- **blog.rtl.css**: Versão do CSS do blog para suporte a idiomas da direita para a esquerda.
- **global.css**: Folha de estilos global aplicada a todo o site.
- **index.html**: Página principal do blog que contém a estrutura HTML do site.
- **scripts/bootstrap.bundle.min.js**: Script JS do Bootstrap que inclui funcionalidades como o carrossel.

## Configuração e Inicialização do Projeto

### Requisitos

- Navegador Web moderno (Google Chrome, Firefox, Safari)
- Conexão com a internet para carregamento de dependências via CDN

### Instruções para Inicialização

1. **Clonar o Repositório**:

   Para começar, você precisa clonar o repositório do projeto para sua máquina local:

   ```bash
   git clone https://github.com/carlosdavid0/Blog-Manger.git
   cd Blog-Manger
   ```

2. **Abrir o Projeto**:

   Após clonar o repositório, abra o arquivo `index.html` em seu navegador preferido.

3. **Customização**:

   - **CSS**: Para customizar o layout ou temas, edite os arquivos `global.css` e `blog.css`.
   - **HTML**: Para alterar o conteúdo, como os títulos das postagens ou as imagens do carrossel, edite o arquivo `index.html`.
   - **Imagens**: Substitua as imagens na pasta `assets` para atualizar o carrossel ou os cartões de novidades.

## Funcionalidades Principais

### Carrossel de Imagens

O carrossel de imagens na seção principal do blog é configurado no seguinte trecho do código HTML:

```html
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators">
    <li
      data-target="#carouselExampleIndicators"
      data-slide-to="0"
      class="active"
    ></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img
        class="d-block img-fluid"
        src="assets/slide1.svg"
        alt="First slide"
      />
      <div class="carousel-caption d-none d-md-block">
        <h4>Death Note | Nova temporada</h4>
        <h5>50° temporada disponível</h5>
      </div>
    </div>
    <!-- Outros itens do carrossel -->
  </div>
</div>
```

### Postagens Recentes

As postagens são exibidas em cartões com imagens e descrições breves:

```html
<div class="col-md-4 col-sm-12">
  <div class="card mb-2">
    <img
      class="card-img-top"
      src="assets/novidades-1.svg"
      alt="Card image cap"
    />
    <div class="card-body">
      <h4 class="card-title">Blue Dragon</h4>
      <p class="card-text">Quando o vilarejo de Shu é atacado...</p>
      <a class="btn btn-primary text-light">Button</a>
    </div>
  </div>
</div>
```

### Navegação

O menu de navegação principal é configurado no cabeçalho e permite a navegação entre diferentes seções do blog.

## Regras de Negócio

1. **Conteúdo Atualizado**: A página inicial deve sempre exibir as últimas postagens e atualizações de animes.
2. **Resolução de Imagens**: Todas as imagens devem ser otimizadas para carregamento rápido, especialmente em conexões lentas.
3. **Responsividade**: O blog deve ser completamente responsivo, garantindo uma experiência consistente em dispositivos móveis e desktops.
4. **Suporte a RTL**: O blog possui suporte a idiomas que utilizam escrita da direita para a esquerda, usando o arquivo `blog.rtl.css`.

## Contribuição

1. **Fork e Clone**: Faça um fork do projeto e clone-o para seu ambiente local.
2. **Criação de Branch**: Crie uma branch para suas alterações.
3. **Pull Request**: Submeta um pull request com uma descrição detalhada das mudanças.

```bash
git checkout -b minha-feature
# Faça suas alterações
git commit -m "Descrição das mudanças"
git push origin minha-feature
```

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

**Desenvolvido por [Carlos David](https://github.com/carlosdavid0)**
