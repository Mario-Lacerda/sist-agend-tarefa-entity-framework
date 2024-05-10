#  **Desafio Dio - Sistema de Agendamento de Tarefas**
O objetivo do Sistema de Agendamento de Tarefas é ajudar as organizações a gerenciar seus projetos e recursos de forma mais eficiente. O sistema permite que os usuários criem e gerenciem tarefas, atribuam tarefas a recursos e rastreiem o progresso das tarefas. Ao fornecer uma visão centralizada de todos os projetos e recursos, o sistema pode ajudar as organizações a melhorar a comunicação, a colaboração e a tomada de decisão.



## **Benefícios:**

- **Melhoria da comunicação e colaboração:** O sistema fornece uma plataforma centralizada para que as equipes colaborem em projetos e tarefas.

- **Tomada de decisão aprimorada:** O sistema fornece às organizações uma visão em tempo real do progresso do projeto e da utilização de recursos, o que permite uma tomada de decisão mais informada.

- **Maior eficiência:** O sistema automatiza muitas tarefas de gerenciamento de projetos, liberando tempo para que as equipes se concentrem em tarefas mais estratégicas.

- **Redução de custos:** Ao melhorar a eficiência e a tomada de decisão, o sistema pode ajudar as organizações a reduzir custos.

  

## **Descrição:**

O Sistema de Agendamento de Tarefas é um aplicativo que permite às organizações gerenciar seus projetos e recursos de forma mais eficiente. O sistema permite que os usuários criem e gerenciem tarefas, atribuam tarefas a recursos e rastreiem o progresso das tarefas. O sistema também pode ser integrado com outros sistemas, como um sistema de gerenciamento de projetos ou um sistema de gerenciamento de recursos humanos.

## **Requisitos:**

- O sistema deve permitir que os usuários criem e gerenciem tarefas.
- O sistema deve permitir que os usuários atribuam tarefas a recursos.
- O sistema deve rastrear o progresso das tarefas.
- O sistema deve ser integrável com outros sistemas.



## Contexto



Você precisa construir um sistema gerenciador de tarefas, onde você poderá cadastrar uma lista de tarefas que permitirá organizar melhor a sua rotina.

Essa lista de tarefas precisa ter um CRUD, ou seja, deverá permitir a você obter os registros, criar, salvar e deletar esses registros.

A sua aplicação deverá ser do tipo Web API ou MVC, fique a vontade para implementar a solução que achar mais adequado.

A sua classe principal, a classe de tarefa, deve ser a seguinte:

![Diagrama da classe Tarefa](diagrama.png)

Não se esqueça de gerar a sua migration para atualização no banco de dados.



## Métodos esperados

É esperado que você crie o seus métodos conforme a seguir:


**Swagger**


![Métodos Swagger](swagger.png)

### **Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |

Esse é o schema (model) de Tarefa, utilizado para passar para os métodos que exigirem

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```



## Solução

O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima.



## **Regras de negócio**

- Uma tarefa só pode ser agendada se houver um recurso disponível para executá-la.

- Uma tarefa só pode ser concluída se todas as suas dependências tiverem sido concluídas.

- Um recurso só pode ser atribuído a uma tarefa por vez.

  

  ## Integração

  

  O Sistema de Agendamento de Tarefas pode ser integrado com outros sistemas, como um sistema de gerenciamento de projetos ou um sistema de gerenciamento de recursos humanos.

  

##   *Testes*

O Sistema de Agendamento de Tarefas deve ser testado para garantir que atenda aos requisitos e funcione conforme o esperado.



##  Conclusão**

O Sistema de Agendamento de Tarefas é uma ferramenta valiosa para organizações que buscam gerenciar seus projetos e recursos de forma mais eficiente. O sistema pode ajudar as organizações a melhorar a comunicação, a colaboração, a tomada de decisão e a eficiência, resultando em menores custos e maior sucesso do projeto.
