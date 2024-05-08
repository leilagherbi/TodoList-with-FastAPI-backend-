# TODO LIST WITH FASTAPI

A small code source developing a ToDo with FASTAPI.


## Prerequisites:  
FastAPI stands on the shoulders of giants:

- Python 3.6+ 
- FastAPI (pip install fastapi) (Optional) 
- A database library (e.g., SQLAlchemy) 
## Installation

Install my-project with npm

```bash
$ pip install fastapi
```
    
## Authors

- [@leilagherbi](https://github.com/leilagherbi)


## 🚀 About Me
I'm an Engineer at Administration and Network Security.
I have some knowledge on web development.


## Documentation

[Documentation](https://linktodocumentation)


## Example

```bash
from fastapi import FastAPI, Body

app = FastAPI()


class Task:
    title: str
    description: str = None
    completed: bool = False


async def get_db():
    # Database connection logic
    db = ...
    yield db

@app.post("/tasks")
async def create_task(task: Task = Body(...), 

db=Depends(get_db)):
    database connection
    saved_task = await save_task_to_db(task, db)
    return saved_task

@app.get("/tasks")
async def get_tasks(db=Depends(get_db)):
    # Retrieve tasks from database
    tasks = await get_tasks_from_db(db)
    return tasks


```
## License

This project is licensed under the terms of the MIT license.


## 🛠 Skills
- Python
- Web Development 
- Social Media Marketing 


## Appendix

- Tutorial: https://fastapi.tiangolo.com/tutorial/ (Get started with a hands-on guide)
- FastAPI Class: https://github.com/tiangolo/full-stack-fastapi-template (Explanation of the main application object)
- Body Parameters: https://fastapi.tiangolo.com/tutorial/body/ (Parsing request data)
- Path Parameters: https://fastapi.tiangolo.com/tutorial/query-params/ (Extracting data from the URL path)
- Query Parameters: https://fastapi.tiangolo.com/tutorial/query-params/ (Handling optional data in the URL)
- Dependency Injection: https://fastapi.tiangolo.com/tutorial/dependencies/ (Managing dependencies like database connections)
- Security: https://github.com/tiangolo/fastapi/discussions/4153 (Implementing authentication and authorization)
- ASGI: https://fastapi.tiangolo.com/tutorial/background-tasks/ (Working with asynchronous operations)
- Testing: https://fastapi.tiangolo.com/tutorial/testing/ (Writing unit and integration tests)
- Deployment: https://github.com/tiangolo/fastapi/discussions/7329 (Deploying your application to production)


