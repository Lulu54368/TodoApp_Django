# TodoApp
## How to begin
### Install and launch virtual environment
```
pipenv install django
pipenv shell
```
### Start app
```
python manage.py startapp todo
```
### Test
```
python manage.py runserver
```
### Edit setting.py
add 'todo' in installed_apps

## During development
### migrate
After modifying models.py, you need migrate
```
python manage.py migrate
```

### Interacting with sqlite
```
python manage.py shell
```
- all objects
  ```
  TodoItem.objects.all()
  ```
  
- add objects
  ```
  a = TodoItem(content = "a")
  a.save()
  ```
- query
  ```
  TodoItem.objects.get(id = 1)
  ```
