## 📚 Catalog Microservice

O microsserviço de **Catalog** é responsável por centralizar e disponibilizar informações sobre os produtos e serviços oferecidos pela empresa.  
Ele garante que os dados de itens estejam sempre atualizados e acessíveis para outros módulos, como **Sales** e **Inventory**, permitindo consistência nas operações de venda e gestão de estoque.  

### Principais responsabilidades:
- Manter o cadastro de produtos e serviços (nome, descrição, preço, categoria, estoque disponível).
- Disponibilizar informações para consulta e integração com pedidos de venda.
- Permitir atualização e exclusão de itens vinculados a pedidos.
- Garantir rastreabilidade das alterações feitas em itens de catálogo.

---

## 🔹 Endpoints relacionados a itens de pedido

- **POST /sales/orders/{id}/items** → Adicionar um item ao pedido de venda, vinculando produto, quantidade e preço unitário.  
- **PUT /sales/orders/{id}/items/{itemId}** → Atualizar informações de um item já existente em um pedido (ex.: quantidade, desconto, preço).  
- **DELETE /sales/orders/{id}/items/{itemId}** → Remover um item específico de um pedido de venda.  
