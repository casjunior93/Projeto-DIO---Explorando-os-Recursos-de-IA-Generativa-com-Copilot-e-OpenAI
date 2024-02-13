# Explorando os Recursos de IA Generativa com Copilot e OpenAI

Neste projeto, não pude utilizar o serviço de OpenAi, devido a limitação de uso. No entando, resolvi demostrar alguns usos relativos a atividades que faço regularmene utilizando o Copiloto da Microsoft ou o ChatGpt.

Na minha opinião, a parte mais interessante de se usar o Copiloto da Microsoft é que são apresentadas fontes após a resposta que podem ajudar a revisar e a saber mais sobre o assunto da pesquisa.

## 1 - Ajuda na criação de código

Regularmente, utilizo IA generativa para me auxiliar a pensar na lógica e implementação de uma funcionalidade. No exemplo abaixo, o Copiloto me ajuda com a criação de uma função que faz o corte de uma string e salva cada peça em um dicionário, com as chaves relativas às posições de corte.

Prompt:

_Crie uma função em Python que receba uma string do seguinte padrão: ck*12345678_89. A função deve cortar a string usando como corte o caractere '*' e armazenar os valores em um dicionário com chaves 'type', 'user_code' e 'digits', respectivamente a posição dos valores cortados._

Resultado:

```python
def parse_string(input_string):
    parts = input_string.split('_')

    if len(parts) != 3:
        return None

    result = {
        'type': parts[0],
        'user_code': parts[1],
        'digits': parts[2]
    }

    return result

input_string = "ck_12345678_89"
parsed_data = parse_string(input_string)

if parsed_data:
    print("Dados extraídos:")
    print(f"Tipo: {parsed_data['type']}")
    print(f"Código do usuário: {parsed_data['user_code']}")
    print(f"Dígitos: {parsed_data['digits']}")
else:
    print("A string não está no formato correto.")

```

## 2 - Criar uma agenda de estudos

Prompt:

_Crie um guia de estudos de 7 dias para aprender sobre probabilidade básica._

Resultado:

Claro! Vamos criar um guia de estudos de **7 dias** para aprender sobre **probabilidade básica**. Aqui está uma sugestão de como você pode estruturar seu estudo:

## Guia de Estudos de 7 Dias: Probabilidade Básica

### Dia 1: Introdução à Probabilidade

1. **Conceitos Fundamentais**:
   - Entenda o que é probabilidade e como ela se relaciona com eventos aleatórios.
   - Explore os termos-chave: experimento aleatório, espaço amostral, ponto amostral e evento.
2. **Cálculo de Probabilidades**:
   - Aprenda a calcular probabilidades usando porcentagens e frações.
   - Pratique com exemplos simples.

### Dia 2: Espaço Amostral e Eventos

1. **Espaço Amostral**:
   - Estude diferentes tipos de espaços amostrais.
   - Identifique os possíveis resultados de um experimento.
2. **Eventos**:
   - Compreenda o conceito de eventos como subconjuntos do espaço amostral.
   - Explore eventos mutuamente exclusivos e eventos independentes.

### Dia 3: Probabilidade de Eventos Simples

1. **Probabilidade de Eventos Únicos**:
   - Calcule a probabilidade de eventos simples.
   - Resolva problemas envolvendo lançamento de dados, moedas e cartas.

### Dia 4: Probabilidade Condicional

1. **Probabilidade Condicional**:
   - Saiba como calcular a probabilidade de um evento ocorrer dado que outro evento já aconteceu.
   - Examine exemplos de probabilidade condicional.

### Dia 5: Distribuição de Frequência e Estatística Descritiva

1. **Estatística Descritiva**:
   - Explore a coleta e organização de dados.
   - Aprenda a calcular média, mediana e moda.
2. **Distribuição de Frequência**:
   - Construa tabelas de frequência para dados discretos.
   - Analise histogramas.

### Dia 6: Estatística Inferencial

1. **Inferência Estatística**:
   - Entenda como fazer inferências sobre uma população com base em uma amostra.
   - Introdução à média amostral e desvio padrão.

### Dia 7: Revisão e Prática

1. **Revisão Geral**:
   - Recapitule os conceitos aprendidos durante a semana.
   - Resolva exercícios de revisão.
2. **Simulado**:
   - Faça um simulado com questões de probabilidade.
   - Avalie seu conhecimento.

Lembre-se de praticar diariamente, resolver problemas e consultar materiais adicionais para aprofundar seu entendimento. Boa sorte nos seus estudos! 📚🔢🍀

¹: [Probabilidade e Estatística: aplicação, fórmulas e mais!](https://www.pravaler.com.br/blog/dicas-de-estudo/probabilidade-e-estatistica-guia-completo/)
²: [Atividades de matemática - Math Center](https://math-center.org/pt-BR/resources/7th/probability/)

Origem: conversa com o Bing, 12/02/2024
(1) Probabilidade e Estatística: aplicação, fórmulas e mais!. https://www.pravaler.com.br/blog/dicas-de-estudo/probabilidade-e-estatistica-guia-completo/.
(2) Probabilidade Sétimo Ano | Atividades de matemática - Math Center. https://bing.com/search?q=guia+de+estudos+de+7+dias+para+aprender+sobre+probabilidade+b%c3%a1sica.
(3) Probabilidade Sétimo Ano | Atividades de matemática - Math Center. https://math-center.org/pt-BR/resources/7th/probability/.
(4) Uma sequência didática para o ensino de probabilidade Marcel Brito .... https://educapes.capes.gov.br/bitstream/capes/569772/1/PRO_Marcel%20Brito%20Soares.pdf.
(5) Quais são as chances? Veja o que é probabilidade e como calcular. https://dicas.vestibulares.com.br/probabilidade/.
