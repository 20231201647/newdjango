# Django 项目

这是一个使用 Django 4.2 创建的 Web 项目。

## 项目结构

```
myproject/
├── __init__.py
├── settings.py      # 项目设置
├── urls.py         # URL 路由配置
├── wsgi.py         # WSGI 配置
└── asgi.py         # ASGI 配置
manage.py           # Django 管理脚本
requirements.txt    # 项目依赖
README.md          # 项目说明
```

## 快速开始

### 1. 安装依赖

```bash
pip install -r requirements.txt
```

### 2. 运行数据库迁移

```bash
python manage.py migrate
```

### 3. 创建超级用户（可选）

```bash
python manage.py createsuperuser
```

### 4. 启动开发服务器

```bash
python manage.py runserver
```

服务器将在 http://127.0.0.1:8000 启动。

## 功能特性

- Django 4.2 框架
- SQLite 数据库（默认）
- 中文语言设置
- 亚洲/上海时区
- 开发模式（DEBUG=True）

## 下一步

1. 创建应用：`python manage.py startapp myapp`
2. 在 `settings.py` 的 `INSTALLED_APPS` 中添加新应用
3. 配置应用的路由和视图
4. 运行 `python manage.py makemigrations` 和 `python manage.py migrate` 来创建数据库表

## 注意事项

- 在生产环境中请修改 `SECRET_KEY`
- 设置 `DEBUG = False`
- 配置合适的 `ALLOWED_HOSTS`