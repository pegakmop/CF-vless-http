<div align="center">

# CF-Workers-VLESS

**[Русский](README.md)** | **[English](README_EN.md)**

Группа в Telegram для обсуждений и обратной связи: https://t.me/eooceu  

Высокопроизводительный VLESS-прокси-сервис на базе Cloudflare Workers  

</div>

---

## Русский

### Возможности
- 🚀 Высокая производительность на базе Cloudflare Workers  
- 🔐 Доступ к главной странице по паролю  
- 📱 Поддержка множества клиентов (v2rayN, Shadowrocket, Loon, Karing, Clash, Sing-box и др.)  
- 🌐 Автоматическое переключение при сбоях и балансировка нагрузки  
- 📊 Тестирование соединений и мониторинг статуса в реальном времени  
- 🎨 Современный адаптивный интерфейс  

### Переменные окружения

#### Обязательные
| Переменная | Описание | По умолчанию | Пример |
|------------|----------|--------------|--------|
| `PASSWORD` | Пароль для доступа к главной странице | `123456` | `your_web_password` |

#### Дополнительные
| Переменная | Описание | По умолчанию | Пример |
|------------|----------|--------------|--------|
| `UUID` / `AUTH` / `uuid` | UUID пользователя | `5dc15e15-f285-4a9d-959b-0e4fbdd77b63` | `your-uuid-here` |
| `PROXYIP` / `proxyip` / `proxyIP` | Список IP-адресов прокси | `13.230.34.30` | `ip1,ip2,ip3` |
| `SUB_PATH` / `subpath` | Путь для подписки | `link` | `sub` |

### Шаги по установке

#### Способ 1: через Cloudflare Dashboard
1. **Вход в Cloudflare Dashboard**  
   - Перейдите на [Cloudflare Dashboard](https://dash.cloudflare.com/)  
   - Войдите в свой аккаунт  

2. **Создание Worker**  
   - Нажмите «Workers & Pages»  
   - Нажмите «Create application»  
   - Выберите «Create Worker»  
   - Введите имя Worker (избегайте слов vless, proxy и т. п., рекомендуется оставить стандартное)  

3. **Загрузка кода**  
   - Скопируйте содержимое файла `_worker.js` в редактор  
   - Нажмите «Deploy» в правом верхнем углу  

4. **Настройка переменных окружения**  
   - В настройках Worker откройте «Settings» → «Variables»  
   - Добавьте необходимые переменные окружения и привяжите собственный домен  
   - Нажмите «Save»  

5. **Доступ по своему домену**  
   - Перейдите на привязанный домен  
   - Введите пароль для входа на главную страницу и получите ссылки для подписки  

---

## English

### Features
- 🚀 High-performance proxy based on Cloudflare Workers  
- 🔐 Password-protected homepage access  
- 📱 Support for multiple clients (v2rayN, Shadowrocket, Loon, Karing, Clash, Sing-box, etc.)  
- 🌐 Automatic failover and load balancing  
- 📊 Real-time connection testing and status monitoring  
- 🎨 Modern responsive interface  

### Environment Variables

#### Required
| Variable | Description | Default | Example |
|----------|-------------|---------|---------|
| `PASSWORD` | Homepage access password | `123456` | `your_web_password` |

#### Optional
| Variable | Description | Default | Example |
|----------|-------------|---------|---------|
| `UUID` / `AUTH` / `uuid` | User UUID | `5dc15e15-f285-4a9d-959b-0e4fbdd77b63` | `your-uuid-here` |
| `PROXYIP` / `proxyip` / `proxyIP` | Proxy server IP list | `13.230.34.30` | `ip1,ip2,ip3` |
| `SUB_PATH` / `subpath` | Subscription path | `link` | `sub` |

### Deployment Steps

#### Method 1: Via Cloudflare Dashboard
1. **Login to Cloudflare Dashboard**  
   - Visit [Cloudflare Dashboard](https://dash.cloudflare.com/)  
   - Login to your account  

2. **Create Worker**  
   - Click "Workers & Pages"  
   - Click "Create application"  
   - Select "Create Worker"  
   - Enter Worker name (avoid keywords like vless, proxy, etc., recommend using default)  

3. **Upload Code**  
   - Copy `_worker.js` file content to editor  
   - Click "Deploy" in the top right corner  

4. **Configure Environment Variables**  
   - Find "Settings" → "Variables" in Worker settings  
   - Add required environment variables and bind custom domain  
   - Click "Save"  

5. **Access Custom Domain**  
   - Enter login password to access homepage and view subscription links  

---

## Лицензия / License

GPL 2.0
