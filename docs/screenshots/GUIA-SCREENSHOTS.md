# Mini-guia de screenshots (padrão do projeto)

Este guia padroniza as imagens usadas no `README.md` para manter um visual limpo e profissional.

## 1) Nomes de arquivo (obrigatório)

Use exatamente estes nomes:

- `01-estrutura-projeto.png`
- `02-app-rodando.png`
- `03-endpoint-olaMundo.png`

## 2) Conteúdo de cada imagem

### `01-estrutura-projeto.png`
- VS Code aberto
- Explorer visível com a estrutura do projeto
- Arquivo `README.md` ou `OlaMundoController.java` aberto

### `02-app-rodando.png`
- Terminal do VS Code mostrando a aplicação em execução
- Evidência de startup do Spring Boot (porta `8080`)

### `03-endpoint-olaMundo.png`
- Navegador exibindo `http://localhost:8080/olaMundo`
- Resposta: `Bem-vindo à disciplina de Desenvolvimento Web Back-End 🚀`

## 3) Padrão visual recomendado

- **Formato:** PNG
- **Resolução sugerida:** 1366x768 (ou 1920x1080)
- **Tema do VS Code:** manter o mesmo em todas as capturas
- **Zoom de interface:** 100% (evitar texto muito pequeno)
- **Corte:** remover áreas irrelevantes (desktop, apps pessoais)

## 4) Boas práticas

- Evite informações pessoais (email, nome de usuário, notificações)
- Feche abas/desordem visual antes de capturar
- Mantenha boa nitidez (sem blur)
- Não misture formatos (`.png` com `.jpg`) para essas 3 imagens

## 5) Checklist rápido antes do commit

- [ ] Os 3 arquivos estão em `docs/screenshots/`
- [ ] Os nomes batem com o padrão
- [ ] O conteúdo corresponde ao que o `README.md` descreve
- [ ] As imagens estão legíveis e sem dados sensíveis
