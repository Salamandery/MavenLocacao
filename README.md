# 🎬 Sistema de Locação de Filmes

<p align="center">
  <img src="https://img.shields.io/badge/Java-8%2B-blue?style=for-the-badge&logo=java"/>
  <img src="https://img.shields.io/badge/Maven-Build-red?style=for-the-badge&logo=apache-maven"/>
</p>

<div align="center">
  <b>🇧🇷 Português | <a href="#english-version">🇺🇸 English below</a></b>
</div>

---

## 📑 Sumário | Table of Contents
- [Sobre o Projeto | About](#sobre-o-projeto--about)
- [Tecnologias | Technologies](#tecnologias--technologies)
- [Estrutura | Structure](#estrutura--structure)
- [Como Executar | How to Run](#como-executar--how-to-run)
- [Entidades | Entities](#entidades--entities)
- [Exemplo de Uso | Usage Example](#exemplo-de-uso--usage-example)
- [Autor | Author](#autor--author)

---

## Sobre o Projeto | About

**PT-BR:**
> Projeto simples em Java para simular um sistema de locação de filmes. Permite cadastrar usuários, filmes e realizar locações, controlando datas e valores. O código é didático, focado em lógica de negócio e boas práticas de programação orientada a objetos.

**EN:**
> Simple Java project to simulate a movie rental system. Allows registering users, movies, and performing rentals, controlling dates and values. The code is educational, focused on business logic and object-oriented programming best practices.

---

## 🚀 Tecnologias | Technologies
- Java 8+
- Maven

---

## 🗂️ Estrutura | Structure
```
MavenLocacao/
├── pom.xml
├── README.md
└── src/
    └── main/
        └── java/
            └── br/
                └── ce/
                    └── wcaquino/
                        ├── entidades/
                        │   ├── Filme.java
                        │   ├── Locacao.java
                        │   └── Usuario.java
                        ├── servicos/
                        │   └── LocacaoService.java
                        └── utils/
                            └── DataUtils.java
```

---

## ⚙️ Como Executar | How to Run

**PT-BR:**
1. **Pré-requisitos:** Java 8+ e Maven instalados.
2. **Compilar o projeto:**
   ```bash
   mvn clean compile
   ```
3. **Executar exemplo:**
   Rode o método `main` da classe `LocacaoService` para ver um fluxo de locação de filme:
   - No terminal:
     ```bash
     mvn exec:java -Dexec.mainClass="br.ce.wcaquino.servicos.LocacaoService"
     ```
   - Ou execute pelo seu IDE preferido.

**EN:**
1. **Prerequisites:** Java 8+ and Maven installed.
2. **Compile the project:**
   ```bash
   mvn clean compile
   ```
3. **Run example:**
   Run the `main` method in `LocacaoService` to see a movie rental flow:
   - In terminal:
     ```bash
     mvn exec:java -Dexec.mainClass="br.ce.wcaquino.servicos.LocacaoService"
     ```
   - Or run it from your favorite IDE.

---

## 🎭 Entidades | Entities

- **Filme / Movie:** Nome, estoque disponível, preço de locação.
- **Usuario / User:** Nome do usuário.
- **Locacao / Rental:** Usuário, filme, data de locação, data de retorno, valor da locação.

---

## 💡 Exemplo de Uso | Usage Example

O método `main` em `LocacaoService` demonstra:
- Criação de usuário e filme
- Realização de uma locação
- Impressão dos resultados no console

**PT-BR:**
```java
LocacaoService service = new LocacaoService();
Usuario usuario = new Usuario("Joao");
Filme filme = new Filme("FILME", 1, 5.0);
Locacao locacao = service.alugarFilme(usuario, filme);
System.out.println(locacao.getValor() == 5.0);
```

**EN:**
```java
LocacaoService service = new LocacaoService();
Usuario usuario = new Usuario("Joao");
Filme filme = new Filme("FILME", 1, 5.0);
Locacao locacao = service.rentMovie(usuario, filme);
System.out.println(locacao.getValor() == 5.0);
```

---

## 👨‍💻 Autor

<div align="center">

**Rodolfo M. F. Abreu**  
Desenvolvedor de software apaixonado por tecnologia, aprendizado contínuo e boas práticas de programação. Sempre em busca de novos desafios e oportunidades para colaborar em projetos inovadores.

[![GitHub](https://img.shields.io/badge/GitHub-rodolfomfabreu-black?style=for-the-badge&logo=github)](https://github.com/salamandery)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rodolfo%20Abreu-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/rodolfo-marques-ferreira-de-abreu/)

Sinta-se à vontade para entrar em contato para dúvidas, sugestões ou colaborações!

</div>

---

<div align="center" id="english-version">
  <b>🇺🇸 English version above | <a href="#top">🇧🇷 Versão em português acima</a></b>
</div>