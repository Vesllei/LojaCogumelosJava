# Loja de Cogumelos em Java


1. **CRUD's (Cadastro, Alteração, Deleção e Listagem):**
   - Para cada entidade do sistema, crie métodos específicos para realizar as operações CRUD.
   - Para o cadastro, implemente um método que receba os dados necessários como parâmetros e crie um novo objeto da entidade correspondente.
   - Para a alteração, crie um método que receba o ID do objeto a ser alterado e os novos dados, e atualize o objeto existente com as informações fornecidas.
   - Para a deleção, implemente um método que receba o ID do objeto a ser excluído e remova-o da lista de objetos ou marque-o como inativo, dependendo dos requisitos.
   - Para a listagem, crie um método que retorne uma lista com todos os objetos da entidade ou implemente métodos de busca que retornem apenas os objetos que correspondam a determinados critérios.

2. **Relação entre CRUD's:**
   - Identifique as associações entre as entidades do seu sistema e defina como essas associações serão representadas no código.
   - Por exemplo, se um Pedido possui uma lista de Produtos, crie um atributo na classe Pedido do tipo List<Produto> para armazenar os produtos associados a esse pedido.
   - Utilize chaves estrangeiras ou referências entre as entidades para estabelecer as relações no banco de dados ou na memória.

3. **Super Classe:**
   - Crie uma classe abstrata que contenha os atributos e métodos comuns a todas as entidades do sistema.
   - Esses atributos podem incluir informações como ID, nome, descrição, data de criação, etc.
   - Implemente métodos getter e setter para acessar e modificar esses atributos.

4. **Classe Abstrata:**
   - Identifique os comportamentos comuns entre diferentes tipos de objetos e crie uma classe abstrata para representá-los.
   - Por exemplo, se todos os produtos têm um método para calcular o preço, coloque esse método na classe abstrata Produto e torne-o abstrato para que as subclasses o implementem de acordo com suas especificações.

5. **Polimorfismo de Sobrescrita:**
   - Na classe abstrata ou superclasse, defina métodos que serão comuns a todas as subclasses.
   - Nas subclasses, sobrescreva esses métodos conforme necessário para ajustá-los às particularidades de cada tipo de objeto.

6. **Polimorfismo de Sobrecarga:**
   - Implemente métodos com o mesmo nome, mas com assinaturas diferentes, para lidar com diferentes tipos de entrada ou comportamentos.
   - Por exemplo, você pode ter métodos sobrecarregados para adicionar produtos ao carrinho, aceitando diferentes tipos de parâmetros, como um único produto ou uma lista de produtos.

7. **Interface:**
   - Identifique comportamentos comuns que podem ser compartilhados por diferentes classes e defina uma interface que as represente.
   - Por exemplo, você pode ter uma interface `Vendavel` que define métodos como `calcularPreco()` e `getNome()` que todas as classes de produto devem implementar.

8. **Encapsulamento:**
   - Defina os atributos das suas classes como privados para proteger o acesso direto a eles.
   - Forneça métodos getter e setter públicos para permitir o acesso controlado aos atributos.

9. **MVC (Model, View e Controller):**
   - Divida seu código em três camadas: Model, View e Controller.
   - Model: Contém a lógica de negócio e as classes de entidades.
   - View: Responsável pela interface com o usuário, como telas e formulários.
   - Controller: Coordena as interações entre a View e o Model, recebendo as entradas do usuário, chamando os métodos apropriados no Model e atualizando a View conforme necessário.

10. **Utilizar estruturas de laço e controle:**
    - Use estruturas de laço (for, foreach, while ou do while) para percorrer listas de itens ou realizar iterações repetidas.
    - Use estruturas de controle (if, else if, else ou switch) para tomar decisões com base em condições específicas.

11. **Log:**
    - Implemente uma classe de log que seja responsável por registrar informações relevantes do sistema.
    - Utilize a classe `FileWriter` para escrever as informações em um arquivo de texto específico.

12. **Serialização:**
    - Implemente métodos de serialização e desserialização nas classes que precisam ser salvas e recuperadas.
    - Utilize as classes `ObjectOutputStream` e `ObjectInputStream` para salvar e carregar objetos em arquivos.
