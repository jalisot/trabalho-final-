# trabalho-final-
the boys
# Sistema de Gerenciamento de Heróis, Crimes, Missões e Simulador de Batalhas

## Descrição Geral

Este sistema foi desenvolvido para gerenciar heróis, seus atributos, crimes cometidos, missões realizadas e simular batalhas entre eles. O código está organizado para ser modular e fácil de entender, com operações CRUD (Criar, Ler, Atualizar e Deletar) disponíveis para heróis, crimes e missões. Além disso, inclui um simulador de batalhas que considera fatores como força, popularidade e aleatoriedade para determinar o vencedor.

## Funcionalidades Principais

1. **Banco de Dados de Heróis**:

   - Gerenciamento de heróis com atributos como nome, idade, características físicas, poderes, força, popularidade, status e histórico de batalhas.
   - Adição, modificação, visualização e remoção de heróis.
   - Atualização automática do status com base na popularidade e número de derrotas.

2. **Banco de Dados de Crimes**:

   - Registro de crimes associados a heróis, incluindo descrição, data, severidade e ocultação de crimes antigos.
   - Impacto direto na popularidade dos heróis baseado na severidade dos crimes.

3. **Banco de Dados de Missões**:

   - Gerenciamento de missões, com atributos como nome, dificuldade, heróis envolvidos, resultado e recompensas.
   - Ajuste de força e popularidade dos heróis com base no resultado das missões.

4. **Simulador de Batalhas**:

   - Simulação de batalhas entre dois heróis, levando em consideração força, popularidade e fatores aleatórios.
   - Relatório detalhado da batalha, incluindo vencedor, impacto na força e popularidade e desempenho dos heróis.

## Estrutura do Código

- **HeroDatabase**: Classe principal que gerencia heróis, crimes e missões.
  - Métodos para adicionar, modificar, listar e remover dados.
  - Simulação de batalhas e cálculo de resultados.
- **Criação de Exemplos**: Heróis como *Homelander*, *Starlight*, *The Deep*, *A-Train* e *Queen Maeve* estão pré-configurados para demonstrar as funcionalidades.

## Como Executar o Sistema

### Pré-requisitos

- Python 3.x instalado no sistema.

### Passos para Execução

1. Faça o download ou copie o código para um arquivo `heroes_management.py`.
2. Abra um terminal ou prompt de comando e navegue até o diretório onde o arquivo está salvo.
3. Execute o programa com o comando:
   ```bash
   python heroes_management.py
   ```

### Exemplos de Uso

#### Adicionar um novo herói

No código:

```python
heroes_db.add_hero(
    name="Black Noir",
    age=32,
    sex="Male",
    physical_features="Masked, silent",
    powers=["Stealth", "Combat skills"],
    strength=90,
    popularity=75,
    status="Ativo",
    wins=20,
    losses=2
)
```

#### Simular uma batalha

No código:

```python
heroes_db.simulate_battle("Homelander", "Queen Maeve")
```

Resultado esperado:

- Relatório detalhado exibindo o desempenho de ambos os heróis.
- Atualização no histórico de vitórias e derrotas, assim como na popularidade.

#### Consultar heróis

No código:

```python
print(heroes_db.list_heroes())
```

## Comentários Adicionais

- O código é extensível e pode ser adaptado para incluir novos tipos de atributos ou funcionalidades.
- Toda modificação em heróis, crimes ou missões reflete diretamente nos atributos relacionados, mantendo a consistência dos dados.




