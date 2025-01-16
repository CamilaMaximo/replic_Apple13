
## Resumo do Código para Troca de Imagem de Produto

1. **Referências de Elementos do DOM**:
   - Identifica os botões dentro da lista (`#image-picker li`) e a imagem do produto (`#product-image`) para manipulação.

2. **Adiciona Event Listeners**:
   - Cada botão recebe um evento de clique para reagir à interação do usuário.

3. **Funções e Comportamentos**:
   - **Remoção de Seleção Anterior**:
     - Ao clicar em um botão, remove a classe `selected` de todos os botões para garantir que apenas o botão ativo seja destacado.
   - **Adição de Seleção Atual**:
     - Adiciona a classe `selected` ao botão clicado para indicar visualmente que ele está ativo.

4. **Alteração da Imagem do Produto**:
   - Obtém o `id` do botão clicado e altera o atributo `src` da imagem do produto para exibir a imagem correspondente (`img/iphone_<id>.jpg`).
   - **Efeito de Transição**:
     - Adiciona temporariamente a classe `changing` à imagem para criar um efeito de transição suave ao trocar a imagem.
     - Remove a classe `changing` após 200ms para concluir a animação.

5. **Exemplo de Uso**:
   - Usuário clica em um botão de cor ou estilo.
   - O botão clicado é destacado, a imagem correspondente ao botão é carregada, e uma transição suave ocorre.

6. **Benefícios da Implementação**:
   - Interface interativa e responsiva para troca de imagens com base na escolha do usuário.
   - Reutilização eficiente de classes e eventos para manter o código limpo e escalável.

