# meiyo\_styles

-----

Este é o **`meiyo_styles`**, um pacote de estilos SCSS desenvolvido para fornecer uma base consistente e um conjunto de componentes visuais reutilizáveis em meus projetos web. Inspirado no conceito de ter controle total sobre o design, este pacote evita frameworks CSS volumosos, focando na flexibilidade e na personalização completa através do poder do SCSS. 

## Recursos

  * **Modular e Organizado:** Estilos divididos em módulos lógicos (base, componentes, layout, mixins) para fácil navegação e manutenção.
  * **Reutilizável:** Basta instalar via NPM e importar em qualquer novo projeto.
  * **Compilável:** Inclui scripts para compilar seu SCSS para CSS.

## Instalação

Para incluir `meiyo_styles` em seu projeto, instale-o via npm:

```bash
npm install meiyo_styles
```

## Uso

Após a instalação, você pode importar os estilos diretamente no seu arquivo SCSS principal do seu projeto. O compilador Sass se encarregará de encontrar os arquivos dentro da pasta `node_modules`.

### Importando no seu SCSS

```scss
// Exemplo: seu-projeto/src/styles/main.scss

// Importa todos os estilos principais do pacote
@import 'meiyo_styles';

// Opcional: Você também pode importar arquivos específicos do pacote se precisar
// Por exemplo, para acessar apenas suas variáveis ou mixins
@import 'meiyo_styles/src/base/variables';
@import 'meiyo_styles/src/mixins/responsive';

/*
  Adicione seus estilos específicos do projeto aqui,
  ou sobrescreva estilos do 'meiyo_styles' se necessário.
*/
body {
  font-family: var(--font-primary, sans-serif);
  color: #333;
}
```

### Exemplo de Configuração de Compilação (com Sass)

O comando `npm install` já traz o CSS compilado e pronto para uso, mas caso queira compilar o SCSS do seu repositório por algum motivo, certifique-se de que seu projeto tem um script de compilação SCSS configurado, como este em seu `package.json` principal:

```json
// seu-projeto/package.json
{
  "name": "seu-projeto",
  // ...
  "scripts": {
    "sass:build": "sass src/styles/main.scss:public/css/styles.css",
    "sass:watch": "sass --watch src/styles/main.scss:public/css/styles.css"
  },
  "devDependencies": {
    "sass": "^1.x.x"
  }
}
```

## Estrutura do Pacote

A estrutura interna do `meiyo_styles` é organizada da seguinte forma:

```
meiyo_styles/
├── src/
│   ├── base/               # Estilos fundamentais (reset, tipografia, variáveis)
│   ├── components/         # Componentes de UI reutilizáveis (botões, cards, forms)
│   ├── layout/             # Estrutura e organização do layout (header, footer, grid)
│   ├── utilities/          # Mixins, variáveis e funções SCSS reutilizáveis e utilitárias
│   └── main.scss           # Ponto de entrada principal do pacote
├── package.json
└── README.md
```

## Desenvolvimento (Para Contribuidores)

Se você estiver desenvolvendo ou contribuindo para o `meiyo_styles` diretamente:

1.  Clone este repositório:
    ```bash
    git clone https://github.com/blink992/meiyo_styles.git
    cd meiyo_styles
    ```
2.  Instale as dependências de desenvolvimento:
    ```bash
    npm install
    ```

## Licença

Este projeto está licenciado sob a licença **MIT**. Veja o arquivo [LICENSE](./LICENSE.md) para mais detalhes.

-----

## Contato

Pedro Arthur Gregorio Abreu - [pedro.agb2004@gmail.com](mailto:pedro.agb2004@gmail.com)

Link do Projeto: [https://github.com/meiyo-aru/meiyo-styles](https://github.com/meiyo-aru/meiyo-styles)

-----

