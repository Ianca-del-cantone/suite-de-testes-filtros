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
