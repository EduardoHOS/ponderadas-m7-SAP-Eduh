🌟 **Querido Afonso**, espero que você esteja maravilhosamente bem neste dia incrível que escolheu para revisar minha ponderada! Conforme recomendado na **Adalove**, segue a entrega das **Regras de Negócio** e o **DMN**. Beijos de luz e muita energia positiva! 💫✨

---

### 📋 **Regras de Negócio**

| **Identificador** | **Nome**                                          | **Descrição**                                                                                                                                                          | **Módulo**           | **Data de Criação** | **Ator**                       | **Data da Última Alteração** | **Autor** | **Versão** | **Dependências**   |
|-------------------|---------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|---------------------|---------------------------------|--------------------------------|------------|------------|--------------------|
| **VE001**         | Critério de Aceitação de Venda                    | Para que uma venda seja aceita, é necessário que o retorno financeiro mínimo seja de 75% sobre o valor do investimento. Isso significa que a margem de lucro esperada deve ser de pelo menos 75% do valor da venda. | Vendas               | 2024-08-21          | Gerente de Vendas              | 2024-08-21                    | Eduardo    | 1.0        | VE002, VE004        |
| **VE002**         | Critério de Módulos Mínimos Business One          | Toda venda do SAP Business One deve incluir, no mínimo, a implementação de cinco módulos para garantir que as necessidades operacionais essenciais do cliente sejam atendidas. | Vendas               | 2024-08-21          | Gerente de Vendas              | 2024-08-21                    | Eduardo    | 1.0        | VE001              |
| **VE003**         | Critério de Módulos Máximos na Patente Inteli/G2  | Caso a venda do SAP Business One inclua mais de sete módulos, deve-se adicionar um sprint adicional ao planejamento do projeto para garantir que a implementação seja concluída com a qualidade e os ajustes necessários. | Vendas               | 2024-08-21          | SAP Business One               | 2024-08-21                    | Eduardo    | 1.0        | VE002              |
| **VE004**         | Critério de Pedido ao Fornecedor                  | Define os critérios para a geração automática de pedidos ao fornecedor no SAP Business One, especificamente para licenças de software. A regra exige a aprovação da venda e a verificação da disponibilidade de estoque. Uma vez atendidos, o sistema envia automaticamente o pedido ao fornecedor. | Vendas - Estoque     | 2024-08-21          | SAP Business One - Gerente de Estoque | 2024-08-21              | Eduardo    | 1.0        | VE001              |
| **VE005**         | Critério de Retorno                               | Como condições para devolução de produtos ou serviços no SAP Business One, os produtos podem ser retornados em até 30 dias da compra. Retornos aprovados geram automaticamente uma nota de crédito, ajustando o faturamento e o estoque. Produtos devolvidos que não estão aptos para revenda são classificados como obsoletos ou para descarte. | Vendas - Estoque     | 2024-08-21          | Estoque                        | 2024-08-21                    | Eduardo    | 1.0        | VE001, VE002       |

---

### 🛠 **Parte do DMN**

🔗 **Link para o modelo DMN**: [Clique aqui para visualizar](https://modeler.camunda.io/share/6e082ba9-1760-497b-9026-a020f31c35e3)

<iframe src="https://modeler.camunda.io/embed/6e082ba9-1760-497b-9026-a020f31c35e3" width="700" height="500" style="border:1px solid #ccc" allowfullscreen></iframe>
