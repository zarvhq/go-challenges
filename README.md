# 🧠 Desafio Técnico: Distância de Manhattan em Go

## Objetivo

Você deve implementar uma função em Go que calcula a distância entre dois pontos marcados com `1` em uma matriz bidimensional. Este exercício tem como objetivo avaliar sua capacidade de trabalhar com arrays, lógica e manipulação de estruturas em Go.

---

## ✏️ Descrição do Desafio

A matriz de entrada é composta apenas por `0`s e dois `1`s.  
Sua missão é localizar as duas posições marcadas com `1` e retornar a distância de Manhattan entre elas.

> A distância de Manhattan entre dois pontos `(x1, y1)` e `(x2, y2)` é dada por:
>
> ```
> |x1 - x2| + |y1 - y2|
> ```

Você deve implementar a seguinte função:

```go
func manhattanDistance(matrix [][]int) int
```

---

## 📥 Exemplo de Entrada

```go
matrix := [][]int{
    {0, 0, 0, 0},
    {0, 1, 0, 0},
    {0, 0, 0, 1},
    {0, 0, 0, 0},
}
```

### ✅ Saída Esperada

```
3
```

> Os pontos estão nas posições (1,1) e (2,3).  
> |1 - 2| + |1 - 3| = 1 + 2 = 3

---

## ✅ Requisitos

- A matriz sempre terá **exatamente dois elementos com valor `1`**.
- Os demais elementos serão `0`.
- A matriz terá no máximo **100 linhas por 100 colunas**.
- A função deve retornar um valor inteiro representando a distância.

---

## 🚀 Instruções

1. Crie um repositório privado no github.
2. Implemente sua solução em um pacote `manhattan` e utilize o pacote dentro do arquivo principal `main.go`.
3. Documente seu projeto com instruções para rodar.

---

## ✅ Pontos avaliados

- Histórico de versionamento
- Estrutura do pacotes
- Cobertura de testes

---

## 🧪 Teste Inicial

Você pode usar o seguinte código para testar rapidamente sua função:

```go
// endereço do seu pacote
import "manhattan"

func main() {
    matrix := [][]int{
        {0, 0, 0, 0},
        {0, 1, 0, 0},
        {0, 0, 0, 1},
        {0, 0, 0, 0},
    }

    result := manhattan.Distance(matrix)
    fmt.Println(result) // Esperado: 3
}
```

---

## 🧠 Dica

Você só precisa percorrer a matriz uma vez para encontrar as posições dos dois `1`s.  
Depois, é só aplicar a fórmula da distância de Manhattan.

---

Boa sorte, e divirta-se com o desafio! 🚀
