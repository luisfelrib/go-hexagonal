# Projeto Go com Arquitetura Hexagonal do cusrso Full Cycle 2.0

## Ferramentas e comandos uteis no desenvolvimento
**Mockgen**
- Usado para gerar os mocks de teste de unidade
```bash
mockgen -destination=application/mocks/application.go -source=application/product.go application
```