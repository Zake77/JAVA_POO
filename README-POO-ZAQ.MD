## 🔖 Sobre


## 💻 Conteúdo programático

ORIENTAÇÃO A OBJETO

 ~ ABSTRAÇÃO
 Expor métodos que queremos que outra classe acesse e obrigar que a classe siga aqueles comportamentos especificos, ocultar o que não precisa ser exposto e criar comportamento padrão para que todas que usem as classes, tenham esse determinado comportamento 

 ~ Criando via interface. Como um molde, um esuqeleto.
Implementando, terá que utilizar os métodos obrigada/contrato. 
@Override subscreve (personaliza)o comportamento da interface(conta)método
_____________________________________________________
Estanciar o objeto é chama-lo na classe princial(main).
Atributos são caracteristicas e métodos são funções/comportamentos.
_____________________________________________________
~ Encapsulamento 
Private só na classe ou com getter/set
Public todas as classes que quiserem
Protected dentro do pacote.

Getter and Setter
- Get para pegar/acessar um valor
- Set para setar/modificar
______________________________________________________
~ Herança
Subclasse, herda métodos, atributos e comportamentos da classe principal/vulgo superclasse ou classe principal.
Parecido com Interface. Sendo interface sendo mais usado. + Clean. Situações que Subclsse são mais utilizado, pois na herança vc pode implementar o metodo e na interface vc nao pode implementar.

Herdando fazendo extends após o nome da classe. Herdando atributos, sendo obrigado a implementa-los, gerando um construtor com retorno super se referindo os atributos da classe principal.

Chamando o método em outra classe: 
@Override
public void(){          //autocomplete
    super.codar();
}
______________________________________________________
~ Construtores
São as caracteristicas para o objeto, pegando os atributos e transformando em um construtor.

public PessoaDesenvolvedora(String nome, String stack, Double salario);
______________________________________________________
 - Método void não tem retorno mas pode imprimir.
 ____________________________________________________


- Implements é só para interface, implementa os comportamentos do contrato
- extends só para herança, herdando, extendendo o comportamento de outra classe.
_____________________________________________________
~ Polimorfirsmo varias formas.

//polimorfismo -> mesma parte do programa de várias formas diferentes para necessidades diferentes
- Sobrecarga  variações do mesmo método com a lista de argumentos e retornos diferentes,
- Sobrecarga é o mesmo nome tipo de retorno e assinatura diferente, com sobrecarga personalizamos o tipo de retorno e também a assinatura(parametros)só que temos que usar o mesmo nome
- VANTAGEN reutilizar códgo

- Subescrita através da palavra extends
 como um botão que liga e desliga.
 Conseguimos ter a implementação diferente porém com  mesmo nome e tipo de retorno.
 - VANTAGEN NÃO ter duplicação de código
 ____________________________________________________

 ~ Ferramentas
 - GitHub
 Ao pressionar a tecla . do teclado dentro do repositorio, abre-se o projeto no Vs.coode
 ____________________________________________________

 ## Como rodar o projeto

 - instalar o maven dentro da pasta do POM.XLM através do terminal.

1 - Configure o java 19 no GitPod
2 - cd/ pasta.api
3 - sdk install java 19.0.2-open

4 - Rode o comando mvn clean e mvn install

5 - Rode o comando mvn spring-boot:run
________________________________________________

~ Repository
É uma classe que usamos a ferramenta JPA, para fazer as query tudo para gente e nAo precisar escrever.
Criaremos a interface que dentro dela terá o contrato do repository (extends JpaRepository)<Curso, Long>

Classes
- Classe @Service de serviço tem regras de negócio, classe modelo e data gerallmente é a tabela.
- Classe repository/repositorio, é a classe que tem a interface entre o banco e a tabela
- Rest controller vai ter os end-points da aplicação.

