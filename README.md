# lnpg-cap8-selecao
Discente: Léo Bernardo da Silva Santos
Atividade prática do Capítulo 8, Estruturas de Seleção.
/respostas/
LLM usado: Grok.
q1_loops.md
# JAVA
public class exercicio1 {
    public static void main(String[] args) {
        int j = 0;
        int i = 0;
        int k;

        k = (j + 13) / 27;

        while (k <= 10) {
            k = k + 1;
            i = 3 * k - 1;
        }

        // out:
        System.out.println("Valor final de k: " + k);
        System.out.println("Valor final de i: " + i);
    }
}

# PYTHON
j = 5  
k = (j + 13) // 27

i = 0
while k <= 10:
    k += 1
    i = 3 * k - 1

print(f"k = {k}")
print(f"i = {i}")

# HASKELL
module Main where

loop :: Int -> Int
loop k
    | k > 10    = k
    | otherwise = loop (k + 1)

main :: IO ()
main = do
    let j    = 5          -- valor de exemplo
        k0   = (j + 13) `div` 27
        kFinal = loop k0
        i    = 3 * kFinal - 1

    putStrLn $ "k = " ++ show kFinal
    putStrLn $ "i = " ++ show i

# SWIFT
import Foundation

func main() {
    let j: Int = 5  // valor de exemplo
    var k: Int = (j + 13) / 27
    var i: Int = 0

    while k <= 10 {
        k += 1
        i = 3 * k - 1
    }

    print("k = \(k)")
    print("i = \(i)")
}

main()

Análise: 
Python: Quantidade de Linhas: 8, muito compacto; Legibilidade: Extremamente claro, qualquer pessoa que sabe programar o mínimo entende bem rápido. Sintaxe limpa, sem ruído. Concisão: Ganha de todos. É o rei da concisão sem sacrificar clareza na maioria dos casos.
Swift: Quantidade de Linhas: 12, limpo e organizado; Legibilidade: Muito legível também. Parece Python mas com tipos,   as variáveis são bem naturais. Concisão:
Haskell: Quantidade de Linhas: 13, Legibilidade: Muito elegante se você entende recursão, mas para um iniciante ou programador comum, parece grego. Concisão:
Java: Quantidade de Linhas: 18, o que contem mais palavras. Legibilidade: Funciona, mas tem muito arrodeio (classe pública, public static void main, etc). O código de verdade fica perdido no meio. Concisão:

q2_selecao.md
# C
#include <stdio.h>

int main() {
    int k = 4; // valor de exemplo
    int j = 0;

    switch (k) {
        case 1:
        case 2:
            j = 2 * k - 1;
            break;
        case 3:
        case 5:
            j = 3 * k + 1;
            break;
        case 4:
            j = 4 * k - 1;
            break;
        case 6:
        case 7:
        case 8:
            j = k - 2;
            break;
        default:
            j = 0; // nenhuma condição satisfeita
            break;
    }

    printf("k = %d\n", k);
    printf("j = %d\n", j);

    return 0;
}

# RUBY
def main
  k = 4  # valor de exemplo
  j = 0

  j = case k
    when 1, 2       then 2 * k - 1
    when 3, 5       then 3 * k + 1
    when 4          then 4 * k - 1
    when 6, 7, 8    then k - 2
    else 0
  end

  puts "k = #{k}"
  puts "j = #{j}"
end

main

# ERLANG
-module(selecao).
-export([main/0]).

calcular_j(K) when K =:= 1; K =:= 2 -> 2 * K - 1;
calcular_j(K) when K =:= 3; K =:= 5 -> 3 * K + 1;
calcular_j(K) when K =:= 4           -> 4 * K - 1;
calcular_j(K) when K =:= 6; K =:= 7; K =:= 8 -> K - 2;
calcular_j(_)                         -> 0.

main() ->
    K = 4,  % valor de exemplo
    J = calcular_j(K),
    io:format("k = ~w~n", [K]),
    io:format("j = ~w~n", [J]).

