# 💰 MoneyMap ASP.NET Expense Tracker  
**MoneyMap** — це вебдодаток для обліку витрат, розроблений за допомогою **ASP.NET Core MVC**. Додаток дозволяє користувачам реєструватися, додавати витрати, переглядати статистику та керувати фінансами у зручному інтерфейсі.  
## 🔧 Технології  
- ASP.NET Core MVC
- Entity Framework Core  
- PostgreSQL 
- Identity (система автентифікації/авторизації)  
- Bootstrap, CSS  
- Azure Web App (деплой)  
## 📁 Структура проєкту  
```
MoneyMapASP.Net/
└── Expense Tracker/            # Основний ASP.NET Core MVC проєкт
    ├── Controllers/            # Контролери
    ├── Models/                 # Моделі домену
    ├── Views/                  # Представлення (UI)
    ├── wwwroot/                # Статичні файли
    ├── Data/                   # Контекст бази даних
    └── Program.cs              # Точка входу
```  
## ⚙️ Як запустити  
### 1. Клонувати репозиторій  
```bash
git clone https://github.com/dolceyu/MoneyMapASP.Net.git
cd MoneyMapASP.Net/Expense\ Tracker
```  
### 2. Встановити залежності  
```bash
dotnet restore
```  
### 3. Налаштувати базу даних  
```bash
dotnet ef database update
```  
> ⚠️ У файлі `appsettings.json` змінити рядок підключення до БД за потреби.  
### 4. Запуск  
```bash
dotnet run
```  
## ✨ Основний функціонал  
- Реєстрація та вхід користувача  
- Додавання та редагування витрат  
- Категорії витрат  
- Графіки / статистика   
- Можливість розширення (адмінпанель, аналітика, інтеграції)  

