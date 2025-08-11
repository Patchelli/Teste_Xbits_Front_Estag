🔁 Instruções de fork e entrega
Faça um fork deste repositório.

Crie um branch a partir da main:

bash
Copiar
Editar
git checkout -b feat/{seu-usuario}/rick-and-morty
Implemente os requisitos (cards, filtros e paginação).

Commits pequenos seguindo Conventional Commits (ex.: feat: cria grid de cards).

Atualize o README do seu projeto com:

Como rodar localmente

Decisões tomadas

O que ficou pendente

Abra um Pull Request para a main do seu fork com:

Descrição do que foi feito

Checklist (filtros e paginação ok; estados de loading/erro/vazio)

Compartilhe o link do PR para avaliação.

Desafio React (Estagiário) — Rick and Morty
Crie uma pequena aplicação React que consome a Rick and Morty API e exibe cards de personagens com paginação e filtros simples.

API: https://rickandmortyapi.com/documentation

Endpoint principal: GET https://rickandmortyapi.com/api/character

🎯 Objetivo
Exibir uma lista de personagens em cards (imagem + informações básicas).

Permitir paginação.

Permitir filtrar por nome (texto) e status (Alive/Dead/Unknown).

🧩 Requisitos (mínimos)
UI
Grid de cards com:

Imagem

Nome

Status (Alive/Dead/Unknown)

Espécie (Species)

Topo com filtros:

Busca por nome (name)

Status (status: alive, dead, unknown)

Paginação:

Botões Anterior / Próximo (ou numeração simples)

Estados visuais:

Carregando (ex.: “Carregando...”)

Erro (ex.: “Ocorreu um erro. Tente novamente.”)

Vazio (ex.: “Nenhum resultado encontrado.”)

Funcional
Consumir GET /api/character com os parâmetros:

page (ex.: ?page=2)

name (ex.: ?name=rick)

status (ex.: ?status=alive)

Ao alterar filtros, reiniciar para a página 1.

Manter filtros aplicados ao trocar de página.

🔎 Exemplos de chamadas
http
Copiar
Editar
GET https://rickandmortyapi.com/api/character?page=1
GET https://rickandmortyapi.com/api/character?name=rick&status=alive&page=2
🛠 Sugestões técnicas (simples)
Stack: React (Vite ou Create React App)

Fetch: fetch nativo ou axios

Estado: useState / useEffect (Redux não é necessário)

Estilo: CSS / Tailwind / Styled Components (livre)

Roteamento: não é necessário

✅ Critérios de avaliação
Corretude funcional: lista, filtros e paginação funcionando

Qualidade do código: organização, nomes claros, componentes simples

UX básica: estados de carregamento/erro/vazio e feedback visual

Atenção à API: uso correto de query params e paginação via info.prev / info.next

Commits: pequenos e descritivos

🎁 Bônus (opcional)
Filtro por gênero (gender) e/ou espécie (species)

Ordenação (ex.: por nome)

Modal de detalhes ao clicar no card (GET /api/character/{id})

Paginação pelo teclado (← →) ou infinite scroll

Testes (React Testing Library) para um componente

