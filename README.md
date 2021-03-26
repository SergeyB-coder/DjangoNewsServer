# DjangoNewsServer

env\Scripts\activate
python manage.py migrate
python manage.py createsuperuser

# input Username, email, Password

python manage.py runserver

# commandline

pip install httpie

http POST http://127.0.0.1:8000/auth/ username="Username" password="Password"

#result

{
    "token": "fe07a15334f305bc11f34802d2ad3e543e524fbd"
}

# commandline

http  http://127.0.0.1:8000/news/ "Authorization: Token fe07a15334f305bc11f34802d2ad3e543e524fbd"

#result

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
    Hello!

        <h3>Шоу правителей</h3>

        <h3>Победа демократии</h3>

</body>
</html>