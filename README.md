**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I - 2019/2020*

# Ficha de Exercícios - 8: estruturas

Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:

- O código apresentado deve ser bem indentado. 
- O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
- `gcc -Wall -Wextra -Wpedantic -ansi -g exercicio1.c -o exercicio1`
- Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
- Evite o uso de constantes mágicas. 
- Evite duplicação de código. 
- Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.

1.	Defina os seguintes tipos, declarando as variáveis que achar necessárias:

	a) Uma estrutura que guarde o nome de um mês, a abreviatura de 3 letras do mês, o número de dias do mês e o número do mês.
		
	b)	Uma estrutura que guarde o nome do automóvel, o número de cavalos, a cilindrada, o seu ano e a sua cor
	
	c)	Um vetor de estruturas que guarde para os 12 meses as estruturas definidas em a). Inicialize devidamente o 2º mês.
	
	d)	Um vetor de estruturas que guarde para 10 automóveis as estruturas definidas em b). Inicialize devidamente o 6º automóvel.
	
	e)	Um ponteiro para a estrutura definida em a). Aponte-o para o 2ºmês e escreva na consola o seu nome através do ponteiro.
	
	f)	Um ponteiro para a estrutura definida em b). Aponte-o para o 6º automóvel e leia o seu ano.
	
	g)	Um enumerado que tenha como opções: nao, sim, talvez com os valores 0, 1 e 2.
	
	h)	Um enumerado que tenha como opções os meses do ano, tendo como valores os números dos meses respetivos

2.	Desenvolva um programa que permita guardar os seguintes dados referentes a um Equipamento: 
- Número de Equipamento: deve ser gerado automaticamente pelo sistema somando 1 ao número atribuído anteriormente.  
- Designação: string com um máximo de 255 caracteres.
- Data de Aquisição: dia, mês e ano.  
- Condição (enumerado): Normal, Abatido, Avariado.  
- Nº de Série: string com um máximo de 50 caracteres.
- Observações: string com um máximo de 255 caracteres.

	*Nota:* deve ser criada uma estrutura (struct) que suporte as informações acima mencionadas.

3.	Altere o programa anterior para permitir as seguintes funcionalidades, sob a forma de menu:
- Criar Equipamento:  Pede e valida os dados do utilizador e preenche o equipamento. 
- Mostrar o Equipamento: Mostra os dados do Equipamento.

4.	 Altere o programa anterior tendo em conta as notas que se seguem:  
- Não são permitidas quaisquer variáveis globais;  
- Todos os tipos devem ser definidos usando typedef
- Todos os tipos repetidos devem implicar a definição de tipos de dados específicos.   
	- Por exemplo: deve ser definido um tipo para os nomes e outro para as datas.  
- O tipo das datas, deve ser definido como estrutura própria.  
- Os valores enumerados, nomeadamente a “Condição”, implica a definição do respetivo tipo enumerado, que deve obedecer ao seguinte:   
	- Começar no número 1
	- Quando se mostrar o equipamento deve ser escrito em formato de texto 
- É preciso validar todos os dados.
- Sempre que o utilizador inserir um dado inválido deve ser­-lhe repetida a sua solicitação.
	- Exemplo:  
		```bash
		> Data de Aquisição: aa/12/1111
		Erro: data inválida. Tente novamente.  
		> Data de Aquisição: 
		```
5.	 Altere o programa anterior para permitir que o programa guarde até 10 equipamentos. As notas adicionais mantêm-se para esta alínea.
- Criar Equipamento - Deve adicionar um novo equipamento ao sistema. Se não for possível, por exemplo porque não há mais espaço disponível, deve apresentar uma mensagem de erro indicativa. 
- Mostrar Equipamento - Deve pedir ao utilizador o número do Equipamento, procurá-lo, e, se existir, mostrar os seus dados.
- Listar Equipamentos - Deve listar todos os equipamentos existentes (podem não existir ainda os 10).
