# Evo AI Application Stacks

Este repositório contém arquivos de configuração Docker Compose para implantação da aplicação Evo AI.

## Arquivos

- `evo_ai_backend.yml`: Configuração para o backend da aplicação Evo AI
- `evo_ai_frontend.yml`: Configuração para o frontend da aplicação Evo AI

## Como usar

1. Certifique-se de ter o Docker e o Docker Compose instalados
2. Clone este repositório
3. Execute o comando abaixo para criar a rede Docker necessária:
   ```
   docker network create app_network
   ```
4. Inicie o backend:
   ```
   docker-compose -f evo_ai_backend.yml up -d
   ```
5. Inicie o frontend:
   ```
   docker-compose -f evo_ai_frontend.yml up -d
   ```

## Notas

- O backend estará disponível na porta 8000
- O frontend estará disponível na porta 3000
- Certifique-se de ajustar os IPs e senhas conforme necessário antes de executar
