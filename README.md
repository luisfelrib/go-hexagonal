# Projeto Go com Arquitetura Hexagonal

## Ferramentas e comandos uteis no desenvolvimento
**Mockgen**
- Usado para gerar os mocks de teste de unidade
```bash
mockgen -destination=application/mocks/application.go -source=application/product.go application
```
**SQLite**
- Banco de dados SQL implementado direto em cima de um arquivo
```bash
#Create database file
touch db.sqlite
#Open database with SQLite3
sqlite3 db.sqlite
#Create table using SQLite3 terminal
create table products(id string, name string, price float, status string);
```
- Adicionando modulos de comandos
```bash
#Create file inside cmd folder (cobra add [file-name])
cobra add cli
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
