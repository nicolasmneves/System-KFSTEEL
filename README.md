# System KFSTEEL — Expedição de Silos

Sistema desktop feito para a **KFSTEEL** controlar a expedição de silos: login de usuários, cadastro de projetos e itens de pedido.

## Funcionalidades

- Tela de login
- Cadastro de projetos
- Itens de pedido ligados a cada projeto
- Banco **SQLite** local, criado automaticamente na primeira execução (tabelas `usuarios`, `projetos` e `itens_pedido`)

## Tecnologias

Java · JavaFX 21 · SQLite (sqlite-jdbc) · Maven

## Como rodar

```
./mvnw clean javafx:run
```

No Windows, use `mvnw.cmd clean javafx:run`. Também dá para abrir no IntelliJ e rodar `Launcher`.

## Estrutura

```
src/main/java/kfsteel/expedicao/
├── MainApp.java / Launcher.java     início da aplicação
├── Database.java                    conexão e criação das tabelas SQLite
├── LoginController.java
├── MainController.java
├── CadastroController.java
├── ProjetosController.java
├── Projeto.java / ItemPedido.java   modelos
└── Ui.java
src/main/resources/                  telas FXML, CSS e logo
```
