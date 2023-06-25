# .NET Core Demo Microservice Solution

This solution is a collection of three microservices with different database (SQL Server, MySQL & MongoDB).
We'll be developing a API Gateway which communicates with all the three microservices for doing the CRUD operations. Finally we'll also develop a Web Application which only communicates with the API Gateway.
This project is a .NET Core 6 application that combines an Ocelot API Gateway with a Blazor UI. It provides a centralized entry point for accessing multiple microservices through the API gateway, and a user-friendly Blazor UI for interacting with the services.

## Endpoints

- **API Gateway Endpoint**: `http://localhost:8001`
  - Description: Entry point for accessing microservices through the Ocelot API Gateway.

- **Blazor UI Endpoint**: `http://localhost:8002`
  - Description: URL to access the Blazor UI for interacting with the services.

## Steps to Run the Project

1. **Clone the Repository**: Clone the project repository to your local machine.

2. **Navigate to the Project Directory**: Open a command prompt or terminal window and navigate to the project directory.

3. **Build the Solution**: Run `dotnet restore Microservices.sln` to build-restore the solution.

4. **Start the Containers**: Execute `docker-compose up -d --build` to start the Docker containers defined in the Docker Compose configuration.

5. **Access the Blazor UI**: Open a web browser and go to `http://localhost:8002` to access the Blazor UI.

6. **Interact with the Services**: Use the Blazor UI to interact with the services exposed by the microservices through the API Gateway.

7. **Stop the Containers**: When finished, stop the Docker containers by running `docker-compose down` in the project directory.

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

