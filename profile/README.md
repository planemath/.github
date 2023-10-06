#  Planemath

## Project rules

 - Criação de Branches
	 - Todas as branches devem ser identificadas seguindo o seguinte padrão: `0000-NNNN-Type `
	 - `0000`: Número da Issue
	 - `NNNN`: Nome da Branch 
	 - `Type`: Tipo
	
 - Pull Requests
	- Os Pull Request's também devem ser identificados porém com o padrão: `0000-Description `
	- `0000`:Número da Issue
	- `Description`: Descrição
 - Commits 
 	- Para features: "feat: ...."
	- Para bugs: "bugfix: ..."
	- Para Prova de Conceito: "poc: ..."
  	  


# Gerenciamento de Projeto 

	Pontuações de task, horas por sprint

## Horas

|Membro| Quarta-Feira | Quinta-Feira | Sexta-feira | Segunda-Feira | Terça-Feira |
|--|--------------|--------------|-------------|---------------|-------------|
|Diogo| 2 | 3 | 1 | 8 | 8 |


## Pontuação de task


## Work Flow


```mermaid
graph LR

R{Repasse} -->   D[Desenvolvimento]--> V((Validação))
```
```mermaid
graph LR



A[Peguei a Task] --> B{Repasse da Task}
B --> C[Criar roteiro de testes / Testes automatizados ] 
C --> D[Desenvolvimento da task] 
E --> D
C --> E{Validação do roteiro de testes}
D --> F[Desenvolvimento de testes unitários seguindo o roteiro]
F --> G((Checklist de engenharia ))
F --> H((Checklist Funcional))
H --> I
G --> I[Criar Pull Request]
I --> J[Code Review]
J ==> K[Merge]

```
