# password-validator
validador de senhas


URL da documetação Swagger
http://localhost:8080/swagger-ui.html


Método GET /validate/{password}

exemplo: localhost:8080/validate/AbTp9!fok


Solução: 
	
	Implementação do Partnner Regexp para validação de senhas com spring boot java
	
	URL de referência: https://qastack.com.br/programming/3802192/regexp-java-for-password-validation
	
	Implementação de JUnit como teste unitário e documentação Swagger

Descrição
Considere uma senha sendo válida quando a mesma possuir as seguintes definições:

Nove ou mais caracteres
Ao menos 1 dígito
Ao menos 1 letra minúscula
Ao menos 1 letra maiúscula
Ao menos 1 caractere especial
Considere como especial os seguintes caracteres: !@#$%^&*()-+
Não possuir caracteres repetidos dentro do conjunto
Exemplo:

IsValid("") // false  
IsValid("aa") // false  
IsValid("ab") // false  
IsValid("AAAbbbCc") // false  
IsValid("AbTp9!foo") // false  
IsValid("AbTp9!foA") // false
IsValid("AbTp9 fok") // false
IsValid("AbTp9!fok") // true
Nota: Espaços em branco não devem ser considerados como caracteres válidos.

Problema
Construa uma aplicação que exponha uma api web que valide se uma senha é válida.

Input: Uma senha (string).
Output: Um boolean indicando se a senha é válida.

Embora nossas aplicações sejam escritas em Kotlin e C# (.net core), você não precisa escrever sua solução usando elas. Use a linguagem de programação que considera ter mais conhecimento.

Pontos que daremos maior atenção
Testes de unidade / integração
Abstração, acoplamento, extensibilidade e coesão
Design de API
Clean Code
SOLID
Documentação da solução no README
Pontos que não iremos avaliar
docker file
scripts ci/cd
coleções do postman ou ferramentas para execução
Sobre a documentação
Nesta etapa do processo seletivo queremos entender as decisões por trás do código, portanto é fundamental que o README tenha algumas informações referentes a sua solução.

Algumas dicas do que esperamos ver são:

Instruções básicas de como executar o projeto;
Detalhes sobre a sua solução, gostariamos de saber qual foi seu racional nas decisões;
Caso algo não esteja claro e você precisou assumir alguma premissa, quais foram e o que te motivou a tomar essas decisões.
Como esperamos receber sua solução
Esta etapa é eliminatória, e por isso esperamos que o código reflita essa importância.

Se tiver algum imprevisto, dúvida ou problema, por favor entre em contato com a gente, estamos aqui para ajudar.

Nos envie o link de um repo público com a sua solução.
