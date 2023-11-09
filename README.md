# Arquitetura de Computadores - Ficha 1

## Informação do aluno

    Nome: André costa

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### P1. Identifica e descreve os principais componentes de um processador. Fornece uma breve explicação da função de cada componente

- Lista os componentes principais de um processador.
- Para cada componente, descreve o seu papel e função no processador.
- Considera componentes como unidade lógica aritmética (ALU), unidade de controlo (UC), registos internos, memória e interfaces de entrada/saída (I/O).

P1 - Resposta:

    Unidade de Controle-Responsável:    
    
    por controlar as operações de busca, decodificação e execução de instruções.
    Unidade Lógica e Aritmética (ULA): Executa operações lógicas e aritméticas, como adição, subtração e comparação.
    Registradores: Armazenam dados temporários e endereços de memória para operações rápidas. Incluem registradores de dados, endereços e registradores de controle.
    Cache: Memória de acesso rápido usada para armazenar dados frequentemente acessados, reduzindo o tempo de acesso à memória principal.
    Pipeline: Divide a execução de instruções em estágios, permitindo que várias instruções sejam processadas simultaneamente.
    Unidade de Ponto Flutuante (FPU): Executa operações que envolvem números de ponto flutuante, como multiplicação e divisão.
    Barramentos: Meios de comunicação que permitem a transferência de dados entre diferentes componentes, como barramento de dados, barramento de endereço e barramento de controle.
    Memória Cache: Armazena temporariamente dados frequentemente usados para aumentar a velocidade de acesso à memória principal.
    Memória de Acesso Aleatório (RAM): Armazena dados temporariamente para o processador acessar rapidamente.
    Memória de Somente Leitura (ROM): Contém instruções permanentes que não são modificadas durante a operação.


### P2. Compara as arquiteturas de Von Neumann e Harvard em termos de características e principais diferenças

- Lista as principais características da arquitetura Von Neumann.
- Lista as principais características da arquitetura de Harvard.
- Explica as principais diferenças entre as duas arquiteturas, particularmente na organização da memória, busca de instruções e separação de dados.
- Fornece exemplos de sistemas de computação que usam cada arquitetura.

P2 - Resposta:

                    Organização da Memória:
                        Von Neumann: Memória unificada para dados e instruções.
                    Harvard: Memórias separadas para dados e instruções.

        Busca de Instruções:
        Von Neumann: A CPU busca instruções e dados usando o mesmo barramento.
        Harvard: Instruções e dados são acessados por barramentos distintos, permitindo recuperação simultânea.
    
    Separação de Dados:
    Von Neumann: Instruções e dados compartilham a mesma memória.
    Harvard: Instruções e dados são armazenados em memórias diferentes.

### P3. Descreve o ciclo *fetch-decode-execute* num processador, detalhando cada etapa e explicando a sua importância na execução de programas de computador

- Fornece uma explicação detalhada da fase de busca de instrução, incluindo o que ela envolve e por que é importante na operação do processador.
- Explica a fase de descodificação e o seu papel na interpretação das instruções de execução.
- Descreve a fase de execução, destacando a execução propriamente dita das instruções e quaisquer interações com dados.
- Conclui explicando a ordem destas fases e como elas garantem a execução adequada dos programas de computador.
- Usa um diagrama para ilustrar o ciclo.

P3 - Resposta:

        Fase de Busca de Instrução:
    
    O que envolve: Nesta fase, a Unidade de Controle (UC) do processador busca a próxima instrução na memória principal.
    Importância: É crucial porque a instrução a ser executada deve ser carregada na CPU antes que qualquer ação possa ocorrer. Sem a busca adequada, a CPU não teria as instruções necessárias para realizar operações.
    Fase de Descodificação:
    
    O que envolve: Após a busca, a UC interpreta a instrução buscada. Ela identifica a operação a ser realizada e determina quais operandos são necessários.
    Importância: Essa fase é vital para a execução correta, pois define como a instrução deve ser interpretada e executada. Cada instrução tem um código de operação específico que a UC precisa entender para coordenar as ações da CPU.
    Fase de Execução:
    
    O que envolve: Com base na instrução e nos operandos identificados na fase de descodificação, a CPU executa a operação. Isso pode envolver cálculos aritméticos, transferência de dados, controle de fluxo, entre outros.
    Importância: É aqui que a ação real ocorre. A CPU manipula dados de acordo com a instrução, realiza cálculos ou transfere informações entre diferentes partes do sistema. A execução é fundamental para o funcionamento do programa.
    +--------------------------------------+
    |          FASE DE BUSCA               |
    |   Memória Principal                  |
    |   +-----------------------------+    |
    |   | Instrução Atual            |    |
    |   +-----------------------------+    |
    +--------------------------------------+
                       |
                       v
    +--------------------------------------+
    |      FASE DE DESCODIFICAÇÃO           |
    |   Unidade de Controle                |
    |   +-----------------------------+    |
    |   | Código de Operação         |    |
    |   +-----------------------------+    |
    +--------------------------------------+
                       |
                       v
    +--------------------------------------+
    |         FASE DE EXECUÇÃO             |
    |   Unidade de Execução               |
    |   +-----------------------------+    |
    |   | Execução da Instrução      |    |
    |   +-----------------------------+    |
    +--------------------------------------+







