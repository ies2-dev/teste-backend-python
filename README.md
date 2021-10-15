# IES2 - Inovação e Tecnologia
Este é um teste de **Desenvolvedor Python** como pré-entrevista para a candidatura à posição de Desenvolvedor Python  Por gentileza, para executar este teste, faça um *[fork][fork_from_github]* deste repositório em sua conta. caso você não tenha uma conta do GitHub, você pode fazer uma clicando neste [link][create_account].

## Desafios

  1. Prover uma API Restful em `Django` para um cliente enviar dados à um servidor.
  2. Esta API deve possuir seu próprio `README.md`.
  3. os endpoints devem ser documentados com [Api Blueprint][apiblueprint]
  5. A Api deve aceitar os formatos de entrada de dados via JSON, e o retorno poder ser tanto em JSON quanto em XML
  6. Deve haver um tratamento de datas para que as mesmas possam ser armazenadas de forma consistente à um banco  de dados (qualquer um à sua escolha)
  7. A api prover uma forma consistente de o cliente poder fazer uma alteração no modo em que a data é retornada para ele, como por exemplo: o cliente poder escolher se ele vai receber o dado de retorno das datas em `ISO Date`ou `timestamp`.

### Requisitos

#### 1. URLs

  * endpoint que irá receber os dados => POST -- `/data`
  * endpoint que irá retornar todos os dados => GET -- `/data`
  * endpoint que irá retornar os dados de um usuário => GET -- `/data/<id>`
  
#### 2. Request data format
 
```json
{
	"name" : "John Doe",
	"skills": [
		"Django",
		"Python",
		"Flask",
		"Celery",
		"DevOps",
		"MongoDB",
		"PyTest",
		"Clean Code"
	],
	"birthdate": "26/11/1993"
}
```

#### 3. Um dos formatos de retorno possíveis deve ser :
 
```json
[
    {
	    "id": 1,
		"name" : "Jane Doe",
		"skills": [
			"Django","Flask", "Celery"
		],
		"birthdate": 1993-11-26T19:00:00+00:00
	}
]
```

## Recomendações

Aqui estão algumas instruções que podem lhe auxiliar na hora de tomar suas decisões na hora de desenvolver.

### Tecnologias  para este desafio


* [Django](https://www.djangoproject.com/) - Framework à ser utilizado
* [Django REST framework](http://www.django-rest-framework.org/) - biblioteca de abstração Restful

* [PyTest](https://docs.pytest.org/en/latest/) - Ferramentas de testes do Python


### O que será observado

* Tomadas de decisões ao longo do desenvolvimento
* Modo como será utilizado o git
* O domínio sobre a linguagem ao resolver problemas de formas simples e elegantes utilizando as ferramentas disponíveis
* Capacidade de abstração
* Organização
* Conhecimentos sobre Django
* PEP-8
* Teste unitários
* Clean Code
* DevOps

## Autor

* **Bovenzo**  - [GitHub](https://github.com/alissonbovenzo)

[fork_from_github]:https://github.com/ies2-dev/teste-backend-python/fork
[create_account]:https://github.com/join
[apiblueprint]:https://apiblueprint.org/