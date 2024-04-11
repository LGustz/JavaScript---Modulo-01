# JavaScript---Modulo-01
1. Variaveis:
    ### Variaveis são usadas para armazenar dados, tanto do usuário quanto do sistema, por exemplo:
    ```js
    // Tipos de variaveis

    // VAR -- Variavel global

    // Exemplo:
    var str = 'String' // Letra, palavras ou caracteres
    var int = 1 // Números inteiros
    var float = 3.14 // Números com vírgula
    var bool = true // or false

    //Chamando variveis
    console.log(str) // Output: 'String'
    console.log(int) // Output: 1
    console.log(float) // Output: 3.14
    console.log(bool) // Output: true or false

    // LET - Variavel de quarto

    // Exemplo:
    for(let i = 0; i <= 10; i++){
        console.log('Variavel do tipo let apenas será usada onde ela foi declarada!', i)
    }

    // CONST - Variavel sem alteração

    // Exemplo:
    const num = 43
    // const num = 7
    console.log('Variavel const = ', num)```
2. Condição:
    ### Os blocos de condições são usados para comparar dados para exibir um conteúdo ou não, por exemplo:
    ```js
    // Blocos de decisão (IF / ELSE / ELSEIF)

    // If - Se...

    // Exemplo:
    var num = 1
    // Se num for igual a 1, então printar "Num é igual a 1".
    if (num == 1) {
        console.log('Num é igual a 1')
    }

    // If Else - Se, se não...

    // Exemplo:
    var num = 2
    // Se num for diferente de 1, então printar "Num não é igual a 1".
    if (num != 1) {
        console.log('Num não é igual a 1')
    }
    // Se não, então printar "Num é igual a 1". 
    else {
        console.log('Num é igual a 1')
    }

    // Else IF - Se, então, se não...
    num = 10
    // Se num for igual a 10, então printar "Num é igual a 1".
    if (num == 10) {
        console.log('Num é igual a 10')
    }
    // Então se, printar "Num é igual a 9".
    else if (num == 9) {
        console.log('Num é igual a 9')
    }
    // Se não, então printar "Num não é igual a 10 nem a 9".
    else {
        console.log('Num não é igual a 10 nem a 9')
    }
    ```
3. Laços de repetição:
    ### Os laços de repetição são usados para formar loops para que um determinado comando se repita quantas vezes forem necessárias, por exemplo:
    ```js
    // Laços de repetição (FOR / WHILE / DO WHILE)

    // For - Para
    // Geralmente utilizado quando sabemos quantas vezes queremos repetir algum comando. 

    // Exemplo:
    // Para cada vez que I for menor/igual a 10 então printar "Isso está se repetindo pela ', i, 'º vez".
    for(let i = 0; i <= 10; i++){
        console.log('Isso está se repetindo pela ', i, 'º vez.')
    }

    console.log('-------------------------------------------')

    // Outro exemplo:
    // Usamos laços de reprtição para percorrer um arrey.
    var arr = ['João', 'Lucas', 'Felipe']
    for(let i = 0; i in arr; i++){
        console.log(arr[i])
    }

    console.log('-------------------------------------------')


    // While - Enquanto
    // Geralmente utilizado quando não sabemos quantas vezes queremos repetir algum comando, podendo gerar um loop infinito.

    var i = 0
    // Exmplo loop infinito:
    // Enquanto for verdade, repetir até não ser.
    while(true){
        console.log('Comando While repetindo pela ', i, 'º vez.')
        i++
    }

    // Exemplo loop até 10:
    // Enquanto i for menor/igual a 10, então repetir o comando até ser igual a 10.
    while(i <=10){
        console.log('Comando While repetindo pela ', i, 'º vez.')
        i++
    }
    ```
4. Funções:
   ### Funções servem para armazenar códigos que são reutilizados no código., por exemplo: 
   ```js
    // Funções 

    // Exemplo de função com parâmetros:
    // Declarando a função soma com os parâmetros 'num1' e 'num2'. 
    function soma(num1, num2) {
        console.log(num1 + num2)
    }
    // Chamando a função:
    // Mude os parâmetros para os números que deseja somar.
    soma(10, 2)

    // Exemplo de função sem parâmetro:
    function sub(){
        var num3 = 10
        var num4 = 5
        console.log(num3 - num4)
    }
    // Chamando a função:
    sub()

    // Exemplo de arrow function:
    // Aqui ao invés de declararmos uma função já fazemos ela direta na variavel 'arrow'.
    const arrow = () =>{
        var i = 1
        var u = 2
        console.log(u + i)
    }
    // Chamando a função:
    arrow()
   ```

5. Funções Nativas:
   ###  Funções nativas em JavaScript são comando pré definidos, e eles tem diversas funções como por exemplo, pegar a hora/dia/mês/ano atual, tempo de intervalo entre ações, operações matemáticas,  entre outros.
    ```js

    // Vamos começar com o Date(), pegaremos o dia, mês e ano atual.
    // Exemplo:
    var data = new Date();
    var dia = data.getDate()
    var mes = data.getMonth() + 1
    var ano = data.getFullYear()

    // console.log(`${dia} / ${mes} / ${ano}`)
    console.log('Dia | Mês | Ano \n',dia,'/',mes,'/',ano)


    // Agora veremos a função Math que serve para realizar calculos autometicamente, sem precisar da fórmula, por exemplo:
    var aoQuadrado = Math.pow(2, 2)
    console.log('O quadrado de 2 é igual a ', aoQuadrado)

    // Função para arredondar um número usamos o .ceil
    var round = Math.ceil(1.99)
    console.log('Se arredondarmos 1,99 teremos: ', round)

    // PI com Math()
    //                   Math.PI = 3.14...
    console.log('Pi = ', Math.PI)
    ```
6. Objetos em JavaScript:
    ### Objetos servem para transformar elementos reais em informações no código, como por exemplo:
    ```js
    // Criando um Objeto de uma pessoa
    let pessoa = {
        nome : 'Zé Ninguém',
        idade : 99,
        curso : 'DS'
    }
    // Objeto inteiro 
    console.log(pessoa)

    // Nome do obj pessoa
    console.log(pessoa.nome)

    // Idade do obj pessoa
    console.log(pessoa.idade)

    // Curso do obj pessoa
    console.log(pessoa.curso)

    let carro = {
        modelo : 'Fusca',
        placa : '1234567', 
    }
    console.log('Modelo: ', carro.modelo, '\nPlaca: ', carro.placa)
    ```
