# **Tutorial: Pensamento Algorítmico e Sistêmico em Programação**

## **1. Introdução ao Pensamento Computacional**

### **O que é Pensamento Algorítmico?**
É a capacidade de **decompor problemas** em etapas lógicas e ordenadas, como uma receita de bolo. 

**Analogia**:  
Pense em fazer um café:
1. Pegar xícara
2. Colher pó de café
3. Adicionar água quente
4. Mexer
5. Servir

Cada passo é essencial e na ordem correta. Se trocar a ordem (ex: servir antes de mexer), o resultado será diferente.

### **Exemplo Prático: Calcular Média**
**Problema**: Como calcular a média de 3 notas?

**Passo a passo algorítmico**:
1. Receber nota1
2. Receber nota2
3. Receber nota3
4. Somar as três notas
5. Dividir por 3
6. Exibir resultado

```python
# Implementação em Python
nota1 = float(input("Digite a primeira nota: "))
nota2 = float(input("Digite a segunda nota: "))
nota3 = float(input("Digite a terceira nota: "))
media = (nota1 + nota2 + nota3) / 3
print(f"A média é: {media:.2f}")
```

---

## **2. Abstração e Modelagem de Problemas**

### **Identificando Padrões**
**Exercício**: Como identificar se um número é par?

**Solução algorítmica**:
- Se o resto da divisão por 2 for 0 → Par
- Senão → Ímpar

```python
numero = int(input("Digite um número: "))
if numero % 2 == 0:
    print("Par")
else:
    print("Ímpar")
```

### **Analogia do Trânsito**
Pense em um semáforo como um sistema:
- **Entradas**: Cores (verde, amarelo, vermelho)
- **Processamento**: Tempo de cada cor
- **Saída**: Carros parando ou andando

---

## **3. Construindo Algoritmos**

### **Exemplo: Validar Login**
**Requisitos**:
1. Usuário deve ter pelo menos 5 caracteres
2. Senha deve ter 8+ caracteres e um número

**Algoritmo**:
```python
usuario = input("Crie um usuário: ")
senha = input("Crie uma senha: ")

if len(usuario) >= 5:
    if len(senha) >= 8 and any(c.isdigit() for c in senha):
        print("Cadastro válido!")
    else:
        print("Senha inválida!")
else:
    print("Usuário muito curto!")
```

**Fluxograma Mental**:
```
[Início] → [Digitar usuário] → [Tem 5+ letras?] → Não → [Erro]
                             → Sim → [Digitar senha] → [Tem 8+ chars e número?] → Não → [Erro]
                                                                                 → Sim → [Sucesso]
```

---

## **4. Pensamento Sistêmico**

### **Componentes Interconectados**
**Exemplo: Sistema de Biblioteca**
1. **Entrada**: Livro, usuário, data
2. **Processamento**: Registrar empréstimo
3. **Saída**: Comprovante
4. **Feedback**: Lembretes de devolução

**Implementação Simplificada**:
```python
livro = input("Título do livro: ")
usuario = input("Nome do usuário: ")
data = input("Data de empréstimo (dd/mm/aaaa): ")

print(f"""
COMPROVANTE:
Livro: {livro}
Usuário: {usuario}
Data: {data}
Devolução em 7 dias!
""")
```

---

## **5. Exercícios Práticos**

### **Desafio 1: Contador de Palavras**
Crie um programa que:
1. Receba uma frase
2. Conte quantas palavras existem
3. Ignore espaços extras

**Solução**:
```python
frase = input("Digite uma frase: ")
palavras = frase.split()
print(f"Total de palavras: {len(palavras)}")
```

### **Desafio 2: Calculadora de IMC**
Desenvolva uma calculadora que:
1. Pergunte peso e altura
2. Calcule IMC (peso / altura²)
3. Classifique:
   - Abaixo de 18.5: Magreza
   - 18.5–24.9: Normal
   - 25+: Sobrepeso

---

## **6. Analogias para Fixação**

1. **Algoritmo = Receita Culinária**  
   - Ingredientes → Variáveis  
   - Passos → Linhas de código  
   - Forno → Computador  

2. **Bug = Erro na Receita**  
   - Ex: Sal em vez de açúcar → Resultado inesperado  

3. **Depuração = Prova do Bolo**  
   - Testar cada parte antes de servir  

---

## **7. Material Complementar**

**Ferramentas Visuais**:
- [Flowgorithm](http://flowgorithm.org/) (para criar fluxogramas)
- [PythonTutor](https://pythontutor.com/) (visualização passo a passo)

**Próximos Passos**:
- Estruturas condicionais (if/else)
- Loops (for/while)
- Funções

Este tutorial aborda os fundamentos do pensamento algorítmico com exemplos práticos e analogias do cotidiano. Recomendo praticar com os exercícios e expandir gradualmente a complexidade dos problemas!
