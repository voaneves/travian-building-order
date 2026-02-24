<a name="readme-top"></a>
<div align="center">
  
  [![Contributors][contributors-shield]][contributors-url]
  [![Forks][forks-shield]][forks-url]
  [![Stargazers][stars-shield]][stars-url]
  [![Issues][issues-shield]][issues-url]
  [![MIT License][license-shield]][license-url]
  [![LinkedIn][linkedin-shield]][linkedin-url]

</div>
<br />
<div align="center">
  <a href="https://github.com/voaneves/travian-building-order">
    <img src="https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/svg/1f33e.svg" alt="Travian Crop Logo" width="120" height="120">
  </a>
  <h3 align="center">travian-building-order</h3>
  <p align="center">
    Otimizador de Crop e Infraestrutura para máxima eficiência.
    <br />
    <a href="https://github.com/voaneves/travian-building-order"><strong>Explore a documentação »</strong></a>
    <br />
    <br />
    <a href="https://github.com/voaneves/travian-building-order/issues">Reportar um Bug</a>
    ·
    <a href="https://github.com/voaneves/travian-building-order/issues">Solicitar uma Melhoria</a>
  </p>
</div>

<details>
  <summary>Tabela de Conteúdos</summary>
  <ol>
    <li>
      <a href="#sobre-o-projeto">Sobre o Projeto</a>
      <ul>
        <li><a href="#tecnologias-utilizadas">Tecnologias Utilizadas</a></li>
      </ul>
    </li>
    <li><a href="#estrutura-do-projeto">Estrutura do Projeto</a></li>
    <li><a href="#metodologia">Metodologia</a></li>
    <li><a href="#desafios-e-soluções">Desafios e Soluções</a></li>
    <li><a href="#resultados">Resultados</a></li>
    <li><a href="#como-começar">Como Começar</a></li>
    <li><a href="#a-fazer">A Fazer (To Do)</a></li>
    <li><a href="#reportando-bugs">Reportando Bugs</a></li>
    <li><a href="#licença">Licença</a></li>
  </ol>
</details>

## Sobre o projeto

Você já parou para pensar em quanto tempo e recursos desperdiça tentando adivinhar a ordem ideal das construções na sua aldeia? 

Este projeto nasceu para resolver exatamente essa dor de cabeça. O **Travian Building Order** é um otimizador de capital focado em calcular a fila de construção perfeita para maximizar sua produção de cereal. Ele tira o "achismo" do seu jogo e coloca a lógica matemática para trabalhar a seu favor. 🚀

Pontos-chave para prestar atenção:
- **Interface Intuitiva:** Design escaneável com Glassmorphism e Tailwind, focando no que importa.
- **Configuração Personalizada:** Suporta oásis, bônus premium e até o Aqueduto dos Egípcios.
- **Retorno sobre Investimento (ROI):** O algoritmo foca em entregar o menor tempo de retorno para cada ação.
- **Ação Direta:** Fornece não apenas os níveis, mas a exigência mínima de Celeiro para a próxima obra.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

### Tecnologias Utilizadas

Para garantir fluidez sem burocracias, utilizamos tecnologias diretas e executáveis no lado do cliente:

- **HTML5 & Vanilla JavaScript:** Lógica de cálculo robusta sem necessidade de frameworks pesados.
- **Tailwind CSS (via CDN):** Para uma estilização rápida, moderna e responsiva.
- **Inter Font:** Tipografia focada em legibilidade e clareza dos dados.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

## Estrutura do Projeto

- `index.html` (Aplicação completa com UI e lógica de negócio)
- `README.md` (Documentação)
- `LICENSE` (Termos de uso)

## Metodologia

💡 Como transformamos a complexidade do jogo em um plano de ação simples?

### Análise de Cenário (AS IS)

Inicialmente, o jogador precisaria abrir planilhas complexas ou calcular na ponta do lápis se vale mais a pena evoluir um campo de cereal ou subir o nível do Moinho, considerando custos crescentes e bônus multiplicativos. 

### Otimização e Execução (TO BE)

1. **Coleta de Parâmetros:** O usuário define o cenário base (tipo de aldeia, capital, oásis).
2. **Cálculo de Eficiência:** O script varre todas as possibilidades imediatas (Moinho, Padaria, Mansão, Aqueduto e Campos).
3. **Tomada de Decisão:** O algoritmo seleciona a ação que oferece o menor custo por ponto de produção gerado.
4. **Ciclo Contínuo (PDCA do Travian):** O processo é repetido até que todos os campos atinjam o nível máximo ou a condição de parada da aldeia.

## Desafios e Soluções

### Desafio 1: Complexidade Matemática dos Bônus

- **Problema:** Bônus de Oásis, Premium (Ouro) e Edifícios (Moinho/Padaria) interagem de forma multiplicativa, tornando o cálculo de ROI dinâmico.
- **Solução:** Estruturamos os custos e os valores de produção em matrizes fixas no JavaScript e criamos funções independentes (`totalprodn`) para simular o cenário exato antes de tomar a decisão de "comprar" o nível.

### Desafio 2: Experiência do Usuário (UX)

- **Problema:** Exibir uma tabela com 20 ou 30 passos de construção pode ser visualmente exaustivo e confuso.
- **Solução:** Aplicamos cores estratégicas aos ícones e destaques visuais nas ações (ex: verde para campos, azul para Moinho). Usamos a "Escaneabilidade" inegociável para o jogador ler, aplicar e voltar para o jogo rapidamente.

## Resultados

1. **Decisão Baseada em Dados:** O script revela exatamente quando o custo-benefício de uma Mansão do Herói para anexar um Oásis supera a evolução de um campo de cereal nível 10+.
2. **Planejamento Logístico:** A coluna de "Celeiro Mínimo" entrega a informação tática exata para evitar que o jogador trave a fila por falta de capacidade de armazenamento.

Afinal, a verdadeira eficiência está em utilizar a automação a nosso favor. Delegar os cálculos exaustivos para a máquina significa mais tempo livre, menos estresse diário e, principalmente, energia de sobra para focar na estratégia e no bem-estar pessoal fora do jogo. 🚀

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

## Como começar

1. Clone este repositório para sua máquina:

   ```bash
   git clone [https://github.com/voaneves/travian-building-order.git](https://github.com/voaneves/travian-building-order.git)
   ```

2. Dê um clique duplo no arquivo `index.html` para abri-lo no seu navegador favorito.

3. Configure os parâmetros da sua aldeia no painel superior.

4. Clique no botão **Gerar Fila Perfeita** e siga a tabela de construção!

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

## A Fazer

- [ ] Incluir suporte a heróis com bônus de produção de recursos.
- [ ] Adicionar funcionalidade de exportação da tabela gerada para CSV ou PDF.
- [ ] Implementar modo escuro (Dark Mode) para jogatinas noturnas.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

## Reportando bugs

Encontrou algum problema nos cálculos ou na interface? Siga o passo a passo:

1. Verifique se o bug já foi relatado na nossa aba de "Issues" no GitHub.

2. Se não encontrar um relato existente, clique em "New Issue" para abrir um novo chamado.

3. Forneça um título claro, descrevendo também os passos necessários para reproduzir o erro (ex: informando os níveis de Oásis que você selecionou).

4. Se possível, inclua capturas de tela do seu painel.

5. Clique em "Submit Issue". 

Agradecemos o seu feedback! Se quiser contribuir diretamente no código, abra um Pull Request. Toda ajuda é bem-vinda para deixarmos esse projeto cada vez melhor.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

## Licença

Este projeto é licenciado sob a [MIT License](/LICENSE).

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/voaneves/travian-building-order.svg?style=for-the-badge
[contributors-url]: https://github.com/voaneves/travian-building-order/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/voaneves/travian-building-order.svg?style=for-the-badge
[forks-url]: https://github.com/voaneves/travian-building-order/network/members
[stars-shield]: https://img.shields.io/github/stars/voaneves/travian-building-order.svg?style=for-the-badge
[stars-url]: https://github.com/voaneves/travian-building-order/stargazers
[issues-shield]: https://img.shields.io/github/issues/voaneves/travian-building-order.svg?style=for-the-badge
[issues-url]: https://github.com/voaneves/travian-building-order/issues
[license-shield]: https://img.shields.io/github/license/voaneves/travian-building-order.svg?style=for-the-badge
[license-url]: https://github.com/voaneves/travian-building-order/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/voaneves
