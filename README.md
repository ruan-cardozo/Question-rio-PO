# Question-rio-PO

1-O que é programação orientada a objetos?
R: Programação orientada a objetos é um paradigma de programação que permite a criação de objetos que possuem propriedades e métodos específicos, visando uma maior organização e reutilização de código.

2-Quais são os pilares da programação orientada a objetos?
R:Os quatro pilares da programação orientada a objetos são: encapsulamento, abstração, herança e polimorfismo.

3-O que é uma classe em Java?
R:Em Java, uma classe é um modelo ou plano para a criação de objetos. Ela define as propriedades e comportamentos que os objetos dessa classe terão.

4-Como criar um objeto a partir de uma classe em Java?
R:Para criar um objeto a partir de uma classe em Java, é preciso usar a palavra-chave "new" seguida do nome da classe e dos parênteses.

5-O que faz a palavra new no Java?
R:Em Java, a palavra-chave "new" é usada para criar uma instância de um objeto a partir de uma classe. Ela aloca memória para o objeto e chama o construtor da classe para inicializar suas variáveis.

6-Quais as semelhanças entre Java e C?
R:Algumas semelhanças entre Java e C são: 
*Sintaxe similar,
*Utilização de chaves para delimitar blocos de código,
*Ambos são compilados em bytecode (Java) ou código de máquina (C),
*Possuem suporte para operações aritméticas e lógicas,
*Permitem a definição de funções ou métodos para modularização do código.

7-Quais as diferenças entre Java e C?
R:Algumas diferenças entre Java e C são:
*Java é uma linguagem de programação orientada a objetos, enquanto C é uma linguagem de programação procedural
*Java é uma linguagem interpretada e compilada, enquanto C é uma linguagem apenas compilada
*Java possui um gerenciamento automático de memória, enquanto C exige que o programador gerencie manualmente a alocação e desalocação de memória
*Java é multiplataforma, enquanto C é mais limitado a sistemas operacionais específicos
*Java possui recursos avançados de segurança, como a execução em sandbox e verificação de tipos em tempo de compilação.

8-O que é a classe InputReader e qual é a sua função no programa?
R:A classe InputReader é uma classe personalizada usada para ler entradas do usuário a partir do console em um programa Java. Sua função é encapsular a lógica de leitura de entrada e fornecer uma interface fácil de usar para o programador. Ela é frequentemente usada em conjunto com a classe BufferedReader para fornecer uma entrada de dados mais eficiente.

9-Qual é a finalidade do método readDouble na classe InputReader?
R:O método readDouble na classe InputReader é usado para ler um valor de ponto flutuante (double) da entrada do usuário a partir do console em um programa Java. Ele é utilizado quando se espera que o usuário digite um número decimal como entrada e retorna esse valor como um tipo de dado double.

10-O que é a interface PaymentType e como ela é utilizada no programa?
R:A interface PaymentType é uma interface personalizada usada no programa para definir os tipos de pagamento disponíveis. Ela é implementada por cada uma das classes de pagamento, como a classe CashPayment e CreditCardPayment, e define os métodos que essas classes devem implementar para calcular e exibir informações de pagamento. A interface PaymentType é utilizada para fornecer um meio de abstração para o processamento de pagamentos, permitindo que diferentes tipos de pagamento sejam adicionados ao programa sem a necessidade de alterações significativas no código existente.

11-Como a classe PaymentTypeSelector é responsável por selecionar o tipo de pagamento a ser utilizado?
R: A classe PaymentTypeSelector é responsável por selecionar o tipo de pagamento a ser utilizado ao exibir um menu de opções de pagamento para o usuário e, em seguida, receber e processar a entrada do usuário para selecionar a opção de pagamento apropriada. Ela utiliza um objeto da classe InputReader para ler a entrada do usuário a partir do console e, em seguida, cria uma instância da classe de pagamento apropriada com base na opção selecionada. A classe PaymentTypeSelector é usada para fornecer um meio de interação entre o usuário e o sistema de pagamento, permitindo que o usuário selecione o tipo de pagamento desejado a partir de uma lista de opções disponíveis.

12-Qual é a relação entre a classe PaymentTypeSelector e as classes PixPayment, CreditPayment e BoletoPayment?
R:A classe PaymentTypeSelector é responsável por selecionar o tipo de pagamento a ser utilizado, e com base nessa escolha, ela cria uma instância da classe de pagamento apropriada, que pode ser PixPayment, CreditPayment ou BoletoPayment. Essas três classes são subclasses da classe Payment, que é a classe base para todas as formas de pagamento. A classe PaymentTypeSelector usa o polimorfismo para interagir com essas classes de forma uniforme, permitindo que ela selecione o tipo de pagamento com base em uma única interface (a interface PaymentType) e use métodos comuns para interagir com todas as formas de pagamento. Essa estrutura de classes permite que o sistema de pagamento seja facilmente estendido para adicionar novos tipos de pagamento no futuro, sem afetar o código existente.

13-O que é polimorfismo e como ele é utilizado no programa?
R:Polimorfismo é a capacidade de objetos de diferentes classes responderem a um mesmo método de forma diferente. No programa, o polimorfismo é utilizado quando as classes PixPayment, CreditPayment e BoletoPayment implementam a interface PaymentType e, assim, podem ser referenciadas pela classe PaymentTypeSelector por meio de uma referência polimórfica.

14-Qual é a finalidade do método getName na interface PaymentType e nas classes que a implementam?
R:O método getName na interface PaymentType e nas classes que a implementam tem a finalidade de retornar uma String com o nome do tipo de pagamento correspondente, que é utilizado posteriormente na impressão do recibo de pagamento.

15-O que é a classe Scanner e como ela é utilizada no programa?
R:A classe Scanner é uma classe em Java que permite a leitura de dados a partir da entrada padrão do sistema (normalmente o teclado). No programa em questão, ela é utilizada para ler a entrada do usuário referente às informações do pagamento, como o valor e o tipo de pagamento selecionado.

16-O que é uma exceção e como ela é tratada no método selectPaymentType da classe PaymentTypeSelector?
R:Uma exceção é um evento que ocorre durante a execução de um programa que interrompe o fluxo normal de execução. No método selectPaymentType da classe PaymentTypeSelector, uma exceção é lançada caso o tipo de pagamento escolhido pelo usuário não seja válido. Essa exceção é tratada por meio de um bloco try-catch, que exibe uma mensagem de erro para o usuário e solicita que ele escolha novamente um tipo de pagamento válido.

17-Como seria possível adicionar um novo tipo de pagamento ao programa?
R:Para adicionar um novo tipo de pagamento ao programa, seria necessário criar uma nova classe que implementasse a interface PaymentType e adicioná-la à lista de opções de pagamento na classe PaymentTypeSelector. Em seguida, seria necessário implementar a lógica específica para o novo tipo de pagamento na classe correspondente.

18-Qual é a importância de utilizar interfaces no desenvolvimento de sistemas orientados a objetos?
R:A utilização de interfaces no desenvolvimento de sistemas orientados a objetos permite a separação clara das responsabilidades de cada classe e ajuda a manter o baixo acoplamento e a alta coesão do código. Além disso, as interfaces permitem que diferentes classes possam implementar comportamentos similares, o que aumenta a flexibilidade do sistema e facilita sua expansão e manutenção.

19-Qual é a diferença entre uma classe abstrata e uma interface?
R:Uma classe abstrata pode conter métodos concretos (implementados) e campos, enquanto uma interface só pode ter métodos abstratos (sem implementação) e constantes. Além disso, uma classe pode estender apenas uma classe abstrata, mas pode implementar várias interfaces.

20-O que é encapsulamento e como ele é aplicado no programa?
R:Encapsulamento é o conceito de esconder a complexidade interna de um objeto, permitindo que o acesso a ele seja feito somente por meio de métodos públicos. No programa, o encapsulamento é aplicado por meio do uso de modificadores de acesso, como private e public, que controlam a visibilidade dos atributos e métodos das classes. Por exemplo, na classe Payment, os atributos são definidos como private e os métodos get e set são usados para acessá-los e modificá-los de forma controlada.

21-Como seria possível melhorar a legibilidade do programa?
R:Algumas sugestões para melhorar a legibilidade do programa seriam:
*Utilizar nomes mais descritivos para as variáveis e métodos;
*Dividir o código em métodos menores, com responsabilidades mais específicas;
*Adicionar comentários explicativos quando necessário;
*Utilizar indentação e espaços em branco para tornar o código mais organizado;
*Utilizar padrões de nomenclatura de classes, variáveis e métodos consistentes ao longo do código.

22-Qual é a finalidade da classe Main no programa?
R:A classe Main é responsável por iniciar a execução do programa Java. É nela que se encontra o método main, que é o ponto de entrada da aplicação.

23-O que é um construtor padrão e quando ele é utilizado?
R:Um construtor padrão é um construtor que não recebe nenhum parâmetro e é criado automaticamente pelo compilador caso nenhum outro construtor seja definido na classe. Ele é utilizado quando um objeto da classe é criado sem a necessidade de passar parâmetros para a inicialização dos seus atributos.

24-Como é possível proteger o programa contra erros de entrada do usuário?
R:Uma maneira de proteger o programa contra erros de entrada do usuário é utilizar a classe Scanner em conjunto com estruturas de controle de fluxo, como if e try-catch, para validar a entrada do usuário e tratar possíveis exceções. Além disso, é importante fornecer mensagens claras de erro ao usuário para que ele saiba como corrigir a entrada incorreta.

25-Qual é a importância de utilizar nomes descritivos para as classes, métodos e variáveis?
R:Utilizar nomes descritivos ajuda a tornar o código mais legível e compreensível, facilitando a manutenção e a colaboração em equipe. Além disso, nomes bem escolhidos tornam o código mais fácil de ser documentado e de ser entendido por desenvolvedores que não estiveram envolvidos diretamente no desenvolvimento do software.

26-O que é herança e como ela pode ser aplicada no programa?
R:Herança é um conceito da programação orientada a objetos em que uma classe pode herdar atributos e métodos de outra classe. No programa, poderia ser utilizada para criar uma classe genérica de pagamento que incluísse atributos e métodos comuns a todas as formas de pagamento, e então as classes específicas de cada forma de pagamento poderiam herdar dessa classe genérica.

27-Como é possível utilizar a sobrecarga de métodos no programa?
R:A sobrecarga de métodos permite que vários métodos com o mesmo nome, mas diferentes parâmetros, sejam definidos em uma classe. No programa, a sobrecarga de métodos pode ser utilizada para criar vários construtores com diferentes parâmetros, por exemplo.
