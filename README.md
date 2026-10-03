FastAPI Starter
Deploy your FastAPI project to Vercel with zero configuration.

Deploy with Vercel

Live Example: https://vercel-plus-fastapi.vercel.app/

Visit the FastAPI documentation to learn more.

Project Structure
This example follows the larger applications pattern from the FastAPI docs:

app/
├── __init__.py
├── main.py              # FastAPI application entry point
├── templates/
│   └── index.html       # Landing page template
├── api/
│   ├── __init__.py
│   ├── main.py          # API router assembly
│   ├── deps.py          # Shared dependencies
│   └── routes/
│       ├── __init__.py
│       └── items.py     # Item endpoints
└── core/
    ├── __init__.py
    └── config.py        # Application settings
Getting Started
Install the required dependencies using uv:

uv sync
Running Locally
vercel dev
API Endpoints
Method	Path	Description
GET	/	Landing page
GET	/api/v1/items/	List sample items
GET	/api/v1/items/{item_id}	Get item by ID
GET	/docs	Interactive API docs (Swagger UI)
Deploying to Vercel
Deploy your project to Vercel with the following command:

npm install -g vercel
vercel --prod
Or git push to your repository with our git integration.

To view the source code for this template, visit the example repository.
