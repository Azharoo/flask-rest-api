Python REST API in FLASK
==================================================
REQUIREMENTS: pip install Flask, flask-httpauth


Use CURL to test this:

GET all tasks:

curl -u warren:python -i http://127.0.0.1:5000/todo/api/v1.0/tasks

GET task by id:

curl -u warren:python -i http://127.0.0.1:5000/todo/api/v1.0/tasks/1

curl -u warren:python -i http://127.0.0.1:5000/todo/api/v1.0/tasks/2

POST a new task:

curl -u warren:python -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks

UPDATE a task:

curl -u warren:python -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2

DELETE a task:

curl -u warren:python -i -H "Content-Type: application/json" -X DELETE http://localhost:5000/todo/api/v1.0/tasks/2
