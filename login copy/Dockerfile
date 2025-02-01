# Set the working directory
WORKDIR /app

# Copy project files (including mvnw)
COPY . .

# Ensure mvnw is executable
RUN chmod +x mvnw

# Build the project with the Maven Wrapper
RUN ./mvnw package -DskipTests

# Specify the command to run your application
CMD ["java", "-jar", "target/login-0.0.1-SNAPSHOT.jar"]
