# AppAula01 - Spring Boot (Back-End)

Projeto introdutório de **Desenvolvimento Web Back-End** com **Java + Spring Boot**, criado para demonstrar uma API REST simples no VS Code.

---

## 📌 Sobre o projeto

Este projeto expõe um endpoint HTTP GET:

- `GET /olaMundo`

Resposta esperada:

`Bem-vindo à disciplina de Desenvolvimento Web Back-End 🚀`

---

## 🧰 Tecnologias utilizadas

- **Java 17**
- **Spring Boot 3.5.11**
- **Maven (Wrapper: `mvnw`/`mvnw.cmd`)**
- **Spring Web**
- **Spring Boot Actuator**

---

## ✅ Pré-requisitos

Antes de começar, instale:

1. **VS Code**
2. **JDK 17** (Java 17)
3. Extensões do VS Code:
   - **Extension Pack for Java**
   - **Spring Boot Extension Pack** (opcional, mas recomendado)
4. **Git** (opcional, para versionamento)

> Dica: para confirmar a instalação do Java, abra o terminal e verifique se a versão é 17.

---

## 🚀 Como criar este projeto no VS Code (passo a passo)

### 1) Criar o projeto Spring Boot

1. Abra o VS Code.
2. Pressione `Ctrl + Shift + P` para abrir a paleta de comandos.
3. Execute: **Spring Initializr: Create a Maven Project**.
4. Escolha as opções:
   - **Language**: Java
   - **Spring Boot**: `3.5.11` (ou a mais próxima disponível)
   - **Group Id**: `com.facens`
   - **Artifact Id**: `appaula01`
   - **Packaging**: Jar
   - **Java**: `17`
5. Em dependências, selecione:
   - **Spring Web**
   - **Spring Boot Actuator**
6. Escolha a pasta de destino e aguarde a geração.
7. Abra o projeto no VS Code.

---

### 2) Estrutura esperada

Após criar, a estrutura principal ficará semelhante a:

- `pom.xml`
- `src/main/java/com/facens/appaula01/Appaula01Application.java`
- `src/main/resources/application.properties`
- `src/test/java/com/facens/appaula01/Appaula01ApplicationTests.java`

---

### 3) Criar o Controller

Crie o arquivo:

`src/main/java/com/facens/appaula01/OlaMundoController.java`

Com este conteúdo:

```java
package com.facens.appaula01;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class OlaMundoController {

    @GetMapping("/olaMundo")
    public String ola() {
        return "Bem-vindo à disciplina de Desenvolvimento Web Back-End 🚀";
    }
}
```

---

### 4) Executar o projeto

No terminal do VS Code, na raiz do projeto:

#### Windows

```bash
.\mvnw.cmd spring-boot:run
```

#### Linux/macOS

```bash
./mvnw spring-boot:run
```

A aplicação deve subir em:

- `http://localhost:8080`

---

### 5) Testar o endpoint

Abra no navegador:

- `http://localhost:8080/olaMundo`

Você deve ver:

`Bem-vindo à disciplina de Desenvolvimento Web Back-End 🚀`

---

## 🧪 Executar testes

Para rodar os testes automatizados:

#### Windows

```bash
.\mvnw.cmd test
```

#### Linux/macOS

```bash
./mvnw test
```

---

## 🔍 Endpoints úteis

Além do endpoint principal, como o Actuator está habilitado, você pode consultar:

- `GET /actuator/health`

Exemplo:

- `http://localhost:8080/actuator/health`

---

## 📚 Observações

- O projeto usa o **Maven Wrapper**, então não é obrigatório ter Maven instalado globalmente.
- Se a porta `8080` estiver ocupada, altere em `src/main/resources/application.properties`:

```properties
server.port=8081
```

---

## 👨‍🏫 Contexto acadêmico

Projeto base para a disciplina de **Desenvolvimento Web Back-End**.

Se quiser, você pode evoluir este projeto com:

- novos endpoints (`POST`, `PUT`, `DELETE`)
- integração com banco de dados
- validações com Bean Validation
- arquitetura em camadas (Controller, Service, Repository)

---

## 📄 Licença

Uso educacional.