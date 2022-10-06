## O que é YAML
- Uma linguagem de serializacao, seu nopme e YAML ain't markup language (YAML nao e uma linguagem de marcacao)
- usada geralmente para arquivos de configuração, como  Docker, Kubernetes, Ansible
- é de facil leitura para as pessoas humanas, de fácil entendimento
- a extensão dos arquivos é `.yml` ou `.yaml`

## Algumas características
Além da sua familiaridade com `XM`L, possui como principais características:

- Utilizam um conjunto de caracteres unicode (UTF-8 ou UTF-16);
- Possui propósito centrado em dados no lugar de documentos marcados;
- Case sensitive;
- Pode ser utilizada por diversas linguagens;
- É mais legível que o XML e JSON;
- Possui excelente documentação, entre outros.

## Sintaxe do `YAML`
A sintaxe do YAML é extremamente simples e legível, como podemos verificar abaixo:

```yml
funcionario:
 nome: João
 idade: 30
 sexo: Masculino
 profissao: Programador
   dependente:
     nome: Maria
     sexo: Feminino
```

como seria esse mesmo exemplo em `JSON`:

```json
{
"funcionario": { 
	"nome": "João", 
	"idade": 30,
	"sexo": "Masculino",
	"profissao":  "Programador",
		"dependente": {
			"nome": "Maria", 
			"sexo": "Feminino"
		} 
	} 
}
```

