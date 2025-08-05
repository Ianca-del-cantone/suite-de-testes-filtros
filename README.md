# 🧾 Suíte de Testes - Filtro "Todos (All)"

Este repositório faz parte do meu aprendizado em QA, onde documento a criação de suítes de teste usando critérios de aceite escritos em Gherkin. O objetivo aqui é desenvolver uma visão crítica para validar funcionalidades com clareza e organização, preparando um material que facilite análise e automação.

O foco é aprimorar a escrita técnica, simular cenários reais de teste e mostrar a importância de uma suíte de testes bem construída para garantir qualidade.


 **Site utilizado nos testes:** [TodoMVC - React](https://todomvc.com/examples/react/dist/) 
 

<details>
  <summary><strong>📋 Clique aqui para ver a suíte de testes do filtro "All"</strong></summary>

<br>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Cenário</th>
      <th>Caso de Teste (Gherkin)</th>
      <th>Prioridade</th>
      <th>Severidade</th>
      <th>Resultado Esperado</th>
      <th>Resultado Obtido</th>
      <th>Defeitos</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CT01</td>
      <td>Exibir todos os itens com o filtro "All"</td>
      <td>Dado que possuo itens concluídos e itens a fazer<br>Quando clico no filtro "All"<br>Então os itens a fazer devem aparecer sem marcação e os itens concluídos devem aparecer em cinza claro, riscados e com o check marcado à esquerda</td>
      <td>Alta</td>
      <td>Alta</td>
      <td>Então os itens a fazer devem aparecer sem marcação e os itens concluídos devem aparecer em cinza claro, riscados e com o check marcado à esquerda.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT02</td>
      <td>Itens não concluídos aparecem sem marcação</td>
      <td>Dado que possuo uma lista com itens, incluindo alguns não concluídos<br>Quando clico no filtro "All"<br>Então os itens não concluídos devem estar sem marcação</td>
      <td>Média</td>
      <td>Média</td>
      <td>Então os itens não concluídos devem estar sem marcação.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT03</td>
      <td>Visualizar itens após marcar como concluído</td>
      <td>Dado que possuo uma lista com itens pendentes<br>E marco alguns itens como concluídos<br>Quando clico no filtro "All"<br>Então todos os itens, pendentes e concluídos, devem ser exibidos corretamente, com os concluídos riscados e marcados</td>
      <td>Alta</td>
      <td>Alta</td>
      <td>Então todos os itens, pendentes e concluídos, devem ser exibidos corretamente, com os concluídos riscados e marcados.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT04</td>
      <td>Visualizar todos os itens após limpar itens concluídos</td>
      <td>Dado que possuo itens concluídos e pendentes<br>E já limpei os itens concluídos<br>Quando clico no filtro "All"<br>Então apenas os itens pendentes devem ser exibidos na lista</td>
      <td>Média</td>
      <td>Média</td>
      <td>Então apenas os itens pendentes devem ser exibidos na lista.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT05</td>
      <td>Manter filtro "All" ativo após adicionar novo item</td>
      <td>Dado que o filtro "All" está selecionado<br>Quando adiciono um novo item à lista<br>Então o novo item deve ser exibido junto com os demais itens, independente do seu status</td>
      <td>Baixa</td>
      <td>Baixa</td>
      <td>Então o novo item deve ser exibido junto com os demais itens, independente do seu status.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT06</td>
      <td>Exibir contador correto no filtro "All"</td>
      <td>Dado que possuo itens pendentes e concluídos<br>Quando seleciono o filtro "All"<br>Então o contador deve mostrar a quantidade correta de itens pendentes restantes</td>
      <td>Média</td>
      <td>Média</td>
      <td>Então o contador deve mostrar a quantidade correta de itens pendentes restantes.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT07</td>
      <td>Alterar status de item no filtro "All"</td>
      <td>Dado que o filtro "All" está ativo<br>E possuo itens pendentes na lista<br>Quando marco um item como concluído<br>Então o item deve mudar de estado para concluído, riscado e com check marcado e a lista deve continuar exibindo todos os itens</td>
      <td>Alta</td>
      <td>Alta</td>
      <td>Então o item deve mudar de estado para concluído, riscado e com check marcado e a lista deve continuar exibindo todos os itens.</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
  </tbody>
</table>

</details>

## 🧪 O que é uma Suíte de Testes?

Uma suíte de testes reúne casos que validam o comportamento esperado de uma funcionalidade ou fluxo, assegurando que a aplicação funcione conforme o planejado e que possíveis falhas sejam detectadas rapidamente.

 Ter uma suíte bem documentada é essencial para:
- Cobrir os principais cenários e variações
- Facilitar a execução manual e futura automação
- Ajudar na rastreabilidade dos testes
- Manter consistência na validação de funcionalidades
- Apoiar entregas com mais confiança


## ✍️ Linguagem Gherkin
A linguagem Gherkin é usada para escrever casos de teste de forma simples e legível, mesmo por pessoas não técnicas.
Ela segue o formato:

```
Cenário: [descrição do cenário]  
Dado que [estado inicial]  
Quando [ação realizada]  
Então [resultado esperado]  
```

Esse formato facilita a comunicação entre desenvolvedores, QAs e stakeholders, pois descreve o comportamento do sistema pela ótica do usuário.

---

## 🧩 Funcionalidade

Filtro "Todos (All)" na lista de tarefas do TodoMVC, que deve mostrar todos os itens da lista com suas características visuais e manter o contador correto.

---

## 📝 User Story  
Eu, como usuária da aplicação  
Gostaria de visualizar todos os itens da minha lista, sejam pendentes ou concluídos  
Porque assim acompanho minhas tarefas de forma completa e organizada  

---

## 📌 Regras de Negócio

- **RN1**: O filtro "All" apresenta todos os itens da lista
- **RN2**: Itens concluídos aparecem com texto riscado, cinza claro e checkbox marcado
- **RN3**: Itens pendentes aparecem sem marcação
- **RN4**: O contador reflete corretamente a quantidade de itens pendentes

---

## ✅ Critérios de Aceite (Gherkin)  

**Cenário:** Visualizar todos os itens com o filtro "All"<br>  
**Dado que** existem itens pendentes e concluídos na lista<br>  
**Quando** seleciono o filtro "All"<br>  
**Então** todos os itens devem aparecer conforme seu status  


---

## 🧠 Diferença entre Prioridade e Severidade

| Conceito       | O que significa                                                        | Quem define          |
| -------------- | ---------------------------------------------------------------------- | -------------------- |
| **Prioridade** | Define o quão rápido o teste deve ser executado ou o defeito resolvido | Time de produto / QA |
| **Severidade** | Mede o impacto técnico do problema no sistema                          | Time de QA           |

---

## 📝 Sobre os Casos de Teste  
Todos os testes foram escritos com foco em:

- Cobrir os comportamentos principais do filtro
- Trabalhar com critérios claros e mensuráveis  
- Organizar os testes com colunas como Prioridade, Severidade, Status, etc.

---

## 🎯 Objetivo do Projeto  
Praticar a criação de suítes de testes a partir de critérios bem definidos.

- Validar o comportamento do filtro "Todos (All)" na exibição dos itens
- Reforçar o uso de Gherkin como ponte entre negócio e testes  
- Desenvolver habilidades práticas essenciais para a atuação em QA

---

## 📌 Observação
Este projeto não contém código-fonte, pois o foco está na documentação de testes e raciocínio analítico em QA.
É um exercício essencial para fortalecer a base teórica e desenvolver uma visão crítica sobre o que deve ser testado em uma aplicação.

















