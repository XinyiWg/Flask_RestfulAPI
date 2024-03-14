<!-- @format -->

# Flask RESTful API Project

This project is a Flask-based RESTful API that provides CRUD (Create, Read, Update, Delete) operations for managing resources. It utilizes SQLAlchemy for interacting with the database, Flask-Migrate for managing database migrations, Flask-Smorest for creating RESTful endpoints, Marshmallow for object serialization and deserialization, and Swagger/OpenAPI for API documentation. Insomnia is used for testing the API endpoints.

The project also includes a Dockerfile for building a Docker image of the application.

Note: the JWT authentication and authorization features are still under development.
Will update soon:))

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone <repository_url>
   ```

2. **Install dependencies:**

   Navigate to the project directory and install the required dependencies using pip:

   ```bash
   cd <project_directory>
   pip install -r requirements.txt
   ```

## Environment Configuration

This project uses a `.flaskenv` file to manage Flask application environment variables.

3. **Set up the database:**
   To configure the database URL, you can pass it as an argument to the create_app function in your app.py or set it as an environment variable.

   ```bash
   export DATABASE_URL="postgresql://username:password@localhost/dbname"
   ```

   ```bash
   flask db init
   flask db migrate -m "Description of changes"
   flask db upgrade
   ```

4. **Run the application:**

   Start the Flask development server:

   ```bash
   flask run
   ```

   The API will be accessible at `http://localhost:5000`.

## Accessing Swagger UI

Swagger UI is a graphical interface for visualizing and interacting with the API endpoints of this project. To access Swagger UI:

```
http://localhost:<host_port>/swagger-ui
```

## API Endpoints

Check the swagger documentation for the API endpoints and their usage.

## Docker Integration

This project includes a Dockerfile for building a Docker image of the application.

### Building the Docker Image

To build the Docker image, run the following command in the project root directory:

```bash
docker build -t <image_name> .
```

Create a new container from the image and start it:

```bash
docker run -p <host_port>:<container_port> <image_name>
```

Run an existing container:

```bash
docker start my_container
```

```

```
