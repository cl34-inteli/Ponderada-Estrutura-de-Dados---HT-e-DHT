# Casos de Teste

&ensp; Casos de teste são importantes para garantir a qualidade e a confiabilidade de um código. Eles ajudam a identificar erros, validar se o software atende aos requisitos especificados e garantir que alterações no código não causem bugs. Além disso, facilitam a manutenção, aumentam a segurança do desenvolvimento e reduzem custos ao detectar falhas no processo antecipadamente.

## Caso de Teste 1: Inserção de Alunos
**Pré-condição**: Nenhum aluno foi inserido.

**Etapas do Teste**:
- Executar a função ``inserirAlunos`` com a lista de alunos fornecida no código.

- Verificar se os alunos foram inseridos nos nós corretos com base em seus RAs.

**Pós-condição**: Os alunos estão armazenados nos nós corretos da DHT, e a função ``imprimirEstadoNos`` exibe os dados corretamente.

## Caso de Teste 2: Busca de Aluno Existente
**Pré-condição**: Os alunos já foram inseridos.

**Etapas do Teste**:

- Executar a função ``buscarAluno`` com um RA existente.

- Verificar se o aluno é encontrado e se as informações exibidas estão corretas.

**Pós-condição**: O aluno é encontrado, e o nome e o nó onde ele está armazenado são exibidos corretamente.

## Caso de Teste 3: Busca de Aluno Inexistente
**Pré-condição**: Os alunos já foram inseridos na _hash table_.

**Etapas do Teste**:

- Executar a função ``buscarAluno`` com um RA que não existe.

- Verificar se a mensagem "Aluno não encontrado!" é exibida.

**Pós-condição**: A função indica corretamente que o aluno não foi encontrado.

## Caso de Teste 4: Remoção de Aluno Existente

**Pré-condição**: Os alunos já foram inseridos.

**Etapas do Teste**:

- Executar a função ``removerAluno`` com um RA existente.

- Verificar se o aluno é removido corretamente.

- Executar a função ``buscarAluno`` com o mesmo RA para confirmar que o aluno não está mais na _hash table_.

**Pós-condição**: O aluno é removido e a busca por esse RA retorna "Aluno não encontrado!".

## Caso de Teste 5: Verificação do Estado dos Nós
**Pré-condição:** Os alunos já foram inseridos na _hash table_.

**Etapas do Teste**:

- Executar a função ``imprimirEstadoNos`` para exibir o estado de todos os nós.

- Verificar se as informações exibidas correspondem aos alunos inseridos e aos nós corretos.

**Pós-condição**: A função exibe corretamente o estado de todos os nós, incluindo os alunos armazenados.