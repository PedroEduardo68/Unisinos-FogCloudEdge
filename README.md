# ?? FogCloudEdge

<p align="center">

![GitHub last commit](https://img.shields.io/github/last-commit/PedroEduardo68/Unisinos-FogCloudEdge?style=for-the-badge)
![GitHub repo size](https://img.shields.io/github/repo-size/PedroEduardo68/Unisinos-FogCloudEdge?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/PedroEduardo68/Unisinos-FogCloudEdge?style=for-the-badge)
![GitHub top language](https://img.shields.io/github/languages/top/PedroEduardo68/Unisinos-FogCloudEdge?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)

</p>

---

## ? Sobre o Projeto

Este projeto foi desenvolvido como parte das atividades da **Universidade do Vale do Rio dos Sinos (UNISINOS)**, com o objetivo de implementar uma arquitetura baseada em **Cloud Computing**, **Fog Computing** e **Edge Computing**.

A proposta demonstra como os dados podem ser processados em diferentes camadas da infraestrutura, reduzindo latência, melhorando desempenho e distribuindo a carga computacional.



---

# ? Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| Docker | Containers |
| MQTT | Comunicação IoT |
| PostgresqL | Banco de Dados |
| Linux | Ambiente de execução |
| Git | Versionamento |
| GitHub | Hospedagem |

---


---

# ? Fluxo de Funcionamento

```mermaid
sequenceDiagram

participant Edge
participant Fog
participant Cloud
participant Database

Edge->>Fog: Envia dados
Fog->>Fog: Processamento Local
Fog->>Cloud: Dados filtrados
Cloud->>Database: Armazenamento
Database-->>Cloud: Resultado
Cloud-->>Fog: Resposta
Fog-->>Edge: Resultado
```

---


# ? Execução


Utilizando Docker

```bash
docker compose up
```

---



<p align="center">

Desenvolvido com Pedro Camera  na UNISINOS

</p>
