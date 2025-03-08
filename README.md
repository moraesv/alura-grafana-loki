# alura-grafana-loki

Este repositório contém o projeto desenvolvido durante o curso "Confiabilidade: centralizando logs com Grafana Loki" da Alura. O objetivo é demonstrar como centralizar e analisar logs de aplicações utilizando o Grafana Loki, aprimorando a observabilidade e a confiabilidade dos sistemas.

## Estrutura do Projeto

- **client/**: Simulador de chamadas para gerar logs na aplicação.
- **logs/**: Diretório destinado ao armazenamento dos logs gerados.
- **postgres/db/**: Configurações do banco de dados PostgreSQL utilizado pela aplicação.
- **prometheus/**: Configurações do servidor Prometheus para coleta de métricas.
- **template/**: Modelos e configurações adicionais para o projeto.
- **.gitignore**: Arquivo que especifica quais arquivos ou pastas devem ser ignorados pelo Git.
- **README.md**: Arquivo que contém as informações e instruções sobre o projeto.
- **api-cursos-dashboard-final.json**: Arquivo de configuração do dashboard final do Grafana.
- **docker-compose.yml**: Arquivo para orquestração dos serviços via Docker Compose.

## Tecnologias Utilizadas

- **Grafana**: Plataforma de visualização e análise de dados.
- **Loki**: Sistema de gerenciamento e consulta de logs escalável e altamente disponível.
- **Prometheus**: Sistema de monitoramento e alerta.
- **PostgreSQL**: Sistema de gerenciamento de banco de dados relacional.
- **Docker**: Plataforma para criação e gerenciamento de containers.

## Instruções para Execução

1. Certifique-se de ter o Docker e o Docker Compose instalados em sua máquina.
2. Clone este repositório:
   ```bash
   git clone https://github.com/moraesv/alura-grafana-loki.git
   ```
3. Navegue até o diretório do projeto:
   ```bash
   cd alura-grafana-loki
   ```
4. Inicie os serviços com o Docker Compose:
   ```bash
   docker-compose up -d
   ```
5. Acesse o Grafana através do navegador no endereço `http://localhost:3000` e faça login com as credenciais padrão (`admin`/`admin`).
6. Configure o Loki como fonte de dados no Grafana e importe o dashboard `api-cursos-dashboard-final.json` para visualizar os logs centralizados.

## Importância dos Logs para a Observabilidade

Logs são registros detalhados das operações e eventos que ocorrem em um sistema computacional. Eles desempenham um papel crucial na observabilidade, permitindo que desenvolvedores e operadores compreendam o comportamento interno das aplicações e identifiquem problemas de forma eficaz.

A centralização dos logs facilita a correlação de eventos, a detecção de anomalias e a realização de auditorias de segurança. Além disso, a análise de logs é fundamental para a identificação de falhas, monitoramento de desempenho e garantia de conformidade com políticas e regulamentações.

Ao utilizar ferramentas como o Grafana Loki, é possível coletar, armazenar e consultar logs de maneira escalável e eficiente, aprimorando a capacidade de resposta a incidentes e a manutenção proativa dos sistemas.

Para mais detalhes sobre o projeto e conceitos relacionados, consulte os materiais do curso "Confiabilidade: centralizando logs com Grafana Loki" da Alura.

