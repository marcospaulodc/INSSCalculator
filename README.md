# INSSCalculator
Calculates the INSS rate according to the fixed annual table
Uma empresa precisa calcular o desconto do INSS sobre o salário dos seus empregados. 
O desconto do INSS segue uma tabela anual que contém alíquotas para determinadas faixas de salários. O valor do desconto é igual à porcentagem da alíquota sobre o salário. Entretanto, quando o empregado tiver um salário superior ao limite máximo da tabela, o desconto é um valor pré-estabelecido, chamado de teto.
Abaixo segue as tabelas de 2011 e 2012: 
2011
Salário-de-contribuição (R$)	Alíquota para fins de recolhimento 
ao INSS (%)
até R$ 1.106,90	8,00
de R$  1.106,91 a R$ 1.844,83	9,00
de R$ 1.844,84 até R$ 3.689,66	11,00
Teto	405,86


2012
Salário-de-contribuição (R$)	Alíquota para fins de recolhimento 
ao INSS (%)
até R$ 1000,00	7,00
de R$  1.000,01 a R$ 1.500,00	8,00
de R$ 1.500,01 até R$ 3.000,00	9,00
de R$ 3.000,01 até R$ 4.000,00	11,00
Teto	500,00


Para melhor entendimento, vejamos dois exemplos se o ano for 2011:
1.	Se o salário de João for R$ 1.000,00, o desconto do INSS será R$ 1.000,00 multiplicado por 8%, resultando em R$ 80,00.
2.	Se o salário de Maria for R$ 4.000,00, o desconto do INSS será o Teto R$ 405,86.
Anexado está uma solução no Visual Studio 2017. Nela, você deve criar uma classe que implemente a interface definida no projeto INSS chamada ICalculadorInss que possui um método decimal CalcularDesconto(DateTime data, decimal salario).
IMPORTANTE: 
•	Não precisa se limitar a uma classe, crie quantas classes julgar necessário, desde que exista uma que implemente a interface definida
•	A implementação do método Calcular não deve conter vários if-else’s encadeados nem switch.
•	Implemente o método Calcular de tal forma, que se uma nova tabela de outro ano for adicionada, nenhuma linha de código do método Calcular deve ser alterada.
•	A classe que implementa a interface ICaluladorInss não deve possuir nenhum outro método ou propriedade public; único método público deve ser o método da interface.
•	A única responsabilidade da classe que implementa a interface deve ser de calcular o desconto.
•	A implementação deve contemplar os conceitos de Orientação à Objetos.
