# US CDI (US Chronic Disease Indicators) Data

## Setup Project

*Note this was developed using Python 3.12.1, earlier versions may not work*


#### Optional: Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```


### Install dependencies

```bash
pip install -r requirements.txt
```

### Configuration

Sensitive information is stored in a `.env` file. This is not included in the repository for security reasons.

Create a `.env` file in the root of the project and the PostgreSQL connection information.

```bash
DATABASE_USER=username
DATABASE_PASSWORD=password
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_NAME=postgres
```

### Run the application

From the root of the project run the following command:

```bash
flask --app app/main run
```

Or, in VS Code, you can run and debug the project with the `Python Debugger: Flask` launch configuration.

![VS Code Debugging](./docs/vs_code_launch.png)


## API endpoints

```curl
GET /api/questions
GET /api/questions/1
GET /api/questions/1?grouping=6
GET /api/data_types
GET /api/datasources
GET /api/footnotes
GET /api/groupings
GET /api/locations
GET /api/questions
GET /api/ranges
GET /api/data
GET /api/topics
GET /api/units
```


## Libraries and assets used

Design:
- Figma
 - MingCute icon set

Frontend:
- JavaScript
- HTML
- CSS
- Plotly.js

Backend:
- Python
- Flask
- SQLAlchemy
- PostgreSQL
