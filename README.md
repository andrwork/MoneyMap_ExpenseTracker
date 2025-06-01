# 💰 MoneyMap ASP.NET Expense Tracker  
**MoneyMap** — це вебдодаток для обліку витрат, розроблений за допомогою **ASP.NET Core MVC**. Додаток дозволяє користувачам реєструватися, додавати витрати, переглядати статистику та керувати фінансами у зручному інтерфейсі.  
## 🔧 Технології  
- ASP.NET Core MVC (.NET 8)  
- Entity Framework Core  
- SQL Server / SQLite (можна змінити на PostgreSQL)  
- Identity (система автентифікації/авторизації)  
- Bootstrap, CSS  
- Azure Web App (деплой)  
## 📁 Структура проєкту  
```
MoneyMapASP.Net/
└── Expense Tracker/             # Основний ASP.NET Core MVC проєкт
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
### 5. Вхід в систему  
- Адміністратор: (можна додати вручну через Seed або вручну в базу)  
- Звичайні користувачі можуть зареєструватися через `/Account/Register`  
## 📦 Деплой на Azure  
Проєкт може бути задеплоєний на Azure App Service за допомогою Azure CLI:  
```bash
az webapp deploy --resource-group <ResourceGroup> --name <WebAppName> --src-path <шлях_до_zip>
```  
## ✨ Основний функціонал  
- Реєстрація та вхід користувача  
- Додавання та редагування витрат  
- Категорії витрат  
- Графіки / статистика  
- Зміна пароля  
- Можливість розширення (адмінпанель, аналітика, інтеграції)  
## 📌 План розвитку  
- [ ] Перехід на PostgreSQL  
- [ ] Інтеграція з платіжними системами  
- [ ] Адаптивний дизайн  
- [ ] CI/CD з GitHub Actions  
## 📄 Ліцензія  
Проєкт розповсюджується під MIT License.  
З любов’ю 💙 від [@dolceyu](https://github.com/dolceyu)
