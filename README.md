# Projeto Go com Arquitetura Hexagonal do cusrso Full Cycle 2.0

## Ferramentas e comandos uteis no desenvolvimento
**Mockgen**
- Usado para gerar os mocks de teste de unidade
```bash
mockgen -destination=application/mocks/application.go -source=application/product.go application
```
**Cobra**
- Aplicação que facilita o uso de CLI
- Configuração
```bash
#Init - Only first time (Run to create cmd folder and root.go file inside cmd)
cobra init
#Resolve possible modules problem
go mod tidy
#Run to test
go run main.go
```
- Adicionando modulos de comandos
```bash
#Create file inside cmd folder (cobra add [file-name])
cobra add cli
```
- Roando Command Line Interface 
```bash
#Create product in the database
go run main.go cli -a=create -n="Product from CLI" -p=25.0
```