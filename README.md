
# Notes App Back End

This project is the creation of a back end system for managing records such as creating,
edit, view, and delete (CRUD).


## API Reference

#### Insert note

```http
  POST /notes
```

Body Request
```json
{
    "title": "Your title",
    "tags": "Your tags note",
    "body": "Your body note"
}
```


#### Get all notes

```http
  GET /notes
```

#### Get item

```http
  GET /notes/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### Edit note

```http
  PUT /notes/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to update |

Body Request
```json
{
    "title": "Your title",
    "tags": "Your tags note",
    "body": "Your body note"
}
```

#### Delete note

```http
  DELETE /notes/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to delete |




## Installation

Install my-project with npm

```bash
  npm install my-project
  cd my-project
```
    
## Run Locally

Clone the project

```bash
  git clone https://github.com/taqiyyaghazi/notes-app-back-end-hapijs
```

Go to the project directory

```bash
  cd notes-app-back-end-hapijs
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start-dev
```


## Tech Stack

**Node.js :** Hapi.js, nanoid, nodemon, eslint-config-google



