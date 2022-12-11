# Projeto de Automação Industrial
## _Estação de Classificação (Sorting Station)_


>  Hugo Gabriel de Melo Santos <br/>
>  Larissa Duarte Santana

<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1G1dyyB2jy8fpW_XQ-wZS6W3tS32QUEOw" />
</p>

### Descrição do Projeto
A simulação consiste em duas esteiras, que fazem a separação de peças a partir de suas cores, variando entre azul, verde ou cinza. Essas peças são divididas para três saídas distintas, sendo assim, as peças azuis, verde e cinzas vão para as saídas 1, 2 e 3, respectivamente. Próximo às extremidades entre as duas esteiras existe um sensor que consegue retornar um valor numérico que identifica cada objeto em relação às suas características físicas. De acordo com o que é computado pelo sensor é possível acionar atuadores que definem o caminho dos objetos em uma das 3 rampas presentes após o sensor.

Então, após definida a rampa correta, um dos atuadores de 3 presentes (um para cada rampa) empurra a peça para a direção correta e nesse momento a peça causa um interrompimento em um segundo sensor que serve para fazer com que os atuadores possam ter o retorno de que o objeto já foi encaminhado para o caminho correto e voltem para o seu estado inicial.

### Ferramentas

Esse projeto foi desenvolvido em simulação virtual a partir da utilização das seguintes ferramentas:
- [TIA Portal V15.1](https://support.industry.siemens.com/cs/document/109761045/simatic-step-7-and-wincc-v15-1-trial-download?dti=0&pnid=14666&lc=en-WW);
- [STEP 7 PLCSIM](https://support.industry.siemens.com/cs/document/109761045/simatic-step-7-and-wincc-v15-1-trial-download?dti=0&pnid=14666&lc=en-WW);
- [Factory IO](https://factoryio.com);
- Linguagem de Programação LADDER.

### Endereços lógicos de entrada
| Name | Tipo de Dado | Endereço Lógico
| ------ | ------ | -------- |
| Botão Liga | Bool | %I0.1 |
| Botão Desliga | Bool | %I0.3 |
| Reset | Bool | %I0.2 |
| Sensor | Bool | %ID30 |
| Sensor de Saída | Bool | %I0.0 |





