**Resumo da Função de Calculadora de Partidas Ranqueadas**

Esta função, chamada `calcularNivel`, recebe como parâmetros a quantidade de vitórias (`vitorias`) e derrotas (`derrotas`) de um jogador em partidas ranqueadas. Em seguida, ela realiza o seguinte processo:

1. Calcula o saldo de vitórias, subtraindo o número de derrotas do número de vitórias: `saldoVitorias = vitorias - derrotas`.

2. Determina o nível do jogador com base no saldo de vitórias, seguindo as seguintes regras:
   - Se o jogador tiver menos de 10 vitórias, é classificado como "Ferro".
   - Se o jogador tiver entre 11 e 20 vitórias, é classificado como "Bronze".
   - Se o jogador tiver entre 21 e 50 vitórias, é classificado como "Prata".
   - Se o jogador tiver entre 51 e 80 vitórias, é classificado como "Ouro".
   - Se o jogador tiver entre 81 e 90 vitórias, é classificado como "Diamante".
   - Se o jogador tiver entre 91 e 100 vitórias, é classificado como "Lendário".
   - Se o jogador tiver 101 ou mais vitórias, é classificado como "Imortal".

3. A função retorna uma mensagem formatada que inclui o saldo de vitórias e o nível do jogador no seguinte formato:
   `"O Herói tem saldo de {saldoVitorias} e está no nível de {nivel}"`.

Esta função é útil para calcular e exibir o nível de um jogador com base em suas vitórias e derrotas em partidas ranqueadas de um jogo, fornecendo uma mensagem descritiva do nível alcançado.

**Exemplo de Uso:**

```javascript
const vitorias = 70; // Substitua com a quantidade de vitórias desejada
const derrotas = 30; // Substitua com a quantidade de derrotas desejada

const resultado = calcularNivel(vitorias, derrotas);
console.log(resultado); // Exibe o resultado no console
```

O exemplo acima calcula o nível de um jogador com 70 vitórias e 30 derrotas e exibe a mensagem de resultado no console. Substitua os valores de `vitorias` e `derrotas` de acordo com os dados do jogador.