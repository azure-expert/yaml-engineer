## O que é YAML
- Uma linguage de serializacao, seu nopme e YAML ain't markup language (YAML nao e uma linguagem de marcacao)
- usada geralmente para arquivos de configuração, como  Docker, Kubernetes, Ansible
- é de facil leitura para as pessoas humanas, de fácil entendimento
- a extensão dos arquivos é `.yml` ou `.yaml`

## Algumas características
Além da sua familiaridade com `XML`, possui como principais características:

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

## Sintaxe do `JSON`:
A sintaxe do `JSON` seria mais dificil de interpretar se usarmos como o exemplos acima.

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

## `YAML` com Ansible
Abaixo um exemplo basico de uma estrutura de `YAML` com Ansible:

```yml
- name: Install a list of packages (suitable replacement for 2.11 loop deprecation warning)
  ansible.builtin.yum:
    name:
      - nginx
      - postgresql
      - postgresql-server
    state: present
```






Referências
[Treinaweb](https://www.treinaweb.com.br/blog/o-que-e-yaml) - O que é `YAML`
[Imasters](https://imasters.com.br/arquitetura-da-informacao/introducao-ao-yaml-1-2#:~:text=YAML%20%C3%A9%20uma%20linguagem%20usada,no%20GitHub%20Actions%20%5B3%5D%3B) - Introdução ao `YAML`


