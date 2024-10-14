# Projeto: Controle de Válvulas e Bombas

## Descrição
Este projeto é uma aplicação simples em C# que interage com o usuário para verificar o estado de três boias (A, B e C) e determinar as ações necessárias para o controle de válvulas e bombas de água.

## Tecnologias Utilizadas
- **Linguagem**: C#
- **Ambiente de Desenvolvimento**: .NET SDK
- **Editor**: Visual Studio ou Visual Studio Code

## Funcionalidades
- Pergunta ao usuário se as boias A, B e C estão cheias.
- Determina as ações a serem tomadas com base nas respostas:
  - Ligar válvula da COPASA.
  - Ligar a bomba.
  - Chamar um técnico se houver inconsistências.

## Estrutura do Código
O código consiste em três partes principais:
1. **Leitura de Entrada**: Coleta as respostas do usuário.
2. **Lógica de Controle**: Avalia as respostas e decide qual mensagem deve ser exibida.
3. **Saída de Resultados**: Imprime a ação a ser realizada com base nas condições.

### Exemplo de Código
```csharp
Console.WriteLine("A boia A está cheia? (sim/não)");
string resposta1 = Console.ReadLine().ToLower();

// Repetir para boias B e C...

if (resposta1 == "não" && resposta2 == "não" && resposta3 == "não")
{
    Console.WriteLine("Ligar válvula da COPASA!");
}
// Condições adicionais...