# 📚 Pesquisa: Framework Laravel

## 0) O que é um Framework?
Um **framework** é um conjunto de ferramentas, bibliotecas e estruturas pré-definidas que ajudam no desenvolvimento de software, padronizando e acelerando o processo.

---

## 1) O que é API?
**API** (Application Programming Interface) é um conjunto de definições e protocolos que permite a comunicação entre diferentes sistemas ou aplicações.

---

## 2) O que é Framework Laravel?
O **Laravel** é um framework PHP de código aberto, focado em tornar o desenvolvimento web mais simples e elegante, utilizando a arquitetura **MVC**.

---

## 3) Por que utilizar o Laravel?
- Estrutura organizada (MVC)
- Ferramentas integradas para autenticação, rotas, banco de dados
- Comunidade ativa e ampla documentação
- Segurança robusta
- Suporte a **Blade templates** e **Eloquent ORM**

---

## 4) Como é a estrutura do CSS no Laravel?
O Laravel não define uma estrutura de CSS própria, mas geralmente o CSS é organizado em:
- `/public/css` para arquivos compilados
- `/resources/css` ou `/resources/sass` para código-fonte de estilos
- Uso do **Vite** ou **Laravel Mix** para compilar

---

## 5) Como o Laravel funciona?
O Laravel segue o padrão **MVC**:
- **Model**: Gerencia os dados e lógica de negócio
- **View**: Interface que o usuário vê
- **Controller**: Controla a lógica entre Model e View

---

## 6) Como o Laravel é estruturado?
Principais pastas:
- `app/` → Lógica da aplicação
- `routes/` → Arquivos de rotas
- `resources/views` → Arquivos Blade (HTML)
- `database/migrations` → Scripts de banco de dados
- `public/` → Arquivos acessíveis publicamente

---

## 7) O que é composer para o PHP junto ao Laravel?
O **Composer** é um gerenciador de dependências para PHP, usado para instalar e atualizar bibliotecas necessárias para o Laravel.

---

## 8) O que é o Node?
O **Node.js** é um ambiente de execução JavaScript fora do navegador. No Laravel, é usado junto com o **npm** para gerenciar pacotes front-end e compilar assets.

---

## 9) Como funciona o MVC no Laravel?
- **Model** → Representa e gerencia os dados (Eloquent ORM)
- **View** → Renderiza a interface (Blade templates)
- **Controller** → Recebe requisições, processa dados e envia para a View

---

## 10) O que é Blade no Laravel?
O **Blade** é o motor de templates do Laravel. Permite criar layouts dinâmicos e reutilizar trechos de código HTML com sintaxe simplificada.

---

## 11) O que é JSON e exemplo para Laravel?
**JSON** (JavaScript Object Notation) é um formato leve de troca de dados.

Exemplo:
```json
{
  "name": "Eric",
  "email": "eric@example.com"
}
```
---

## 12) O que é um terminal e por que devemos utilizar?
O **terminal** é uma interface de linha de comando que permite interagir com o sistema operacional através de textos e comandos, sem usar interface gráfica.

No Laravel, o terminal é usado para:
- Executar comandos do **Artisan** (CLI do Laravel)
- Instalar pacotes com **Composer** ou **npm**
- Controlar versões com **Git**
- Iniciar o servidor local com `php artisan serve`

---

## 13) Principais comandos do GIT
- `git init` → Inicializa um novo repositório
- `git clone <url>` → Clona um repositório existente
- `git status` → Mostra o status dos arquivos
- `git add .` → Adiciona alterações para commit
- `git commit -m "mensagem"` → Salva as alterações
- `git push` → Envia alterações para o repositório remoto
- `git pull` → Baixa alterações do repositório remoto

---

## 14) Estrutura do banco de dados no Laravel
O Laravel utiliza **Migrations** para criar e alterar tabelas de forma controlada.
Ele também conta com o **Eloquent ORM**, que permite trabalhar com tabelas como se fossem objetos PHP.

Exemplo de model:
```php
class User extends Model
{
    protected $fillable = ['name', 'email', 'password'];
}
```
---

## 14) Como é a estrutura do banco de dados no Laravel?
O Laravel utiliza o **Eloquent ORM** para manipular o banco de dados de forma orientada a objetos.  
A estrutura básica é composta por:
- **Models** → Representam tabelas
- **Migrations** → Criam/alteram tabelas com versionamento
- **Seeders** → Inserem dados iniciais
- **Factories** → Geram dados fictícios para testes

---

## 15) Como é feito o versionamento no banco de dados no Laravel?
O versionamento é feito através de **Migrations**.  
Cada alteração no banco (criação, modificação ou exclusão de tabelas/colunas) é registrada em um arquivo.  
Para aplicar as alterações:
```bash
php artisan migrate

```
---

## 16) Principais comandos para criação no Laravel
a) Criar um projeto Laravel
composer create-project laravel/laravel nome-do-projeto

b) Criar um Controller
php artisan make:controller NomeController

c) Criar uma View
As views ficam em resources/views/ e usam o Blade.
Exemplo: <!-- resources/views/home.blade.php -->
<h1>Bem-vindo ao Laravel!</h1>

d) Criar um Model
php artisan make:model NomeModel


---

## 17) O que é Migration no Laravel?
Migration é um sistema de controle de versão para o banco de dados.
Ele permite criar, alterar e excluir tabelas usando código PHP.

Exemplo:

public function up()
{
    Schema::create('produtos', function (Blueprint $table) {
        $table->id();
        $table->string('nome');
        $table->decimal('preco', 8, 2);
        $table->timestamps();
    });
}

---

18) Softwares necessários para Laravel
PHP (>= 8.0)

Composer → Gerenciador de pacotes do PHP

Node.js e npm → Para gerenciar dependências do frontend

Servidor local (XAMPP, Laragon, Laravel Sail ou Valet)

Banco de dados (MySQL, PostgreSQL, SQLite)

Git → Controle de versão

VS Code ou outro editor de código

perl
Copiar
Editar

Se quiser, eu já posso **juntar tudo do 0 ao 18 em um único `.md` pronto** para você colar no GitHub.  
Quer que eu faça o arquivo completo?
