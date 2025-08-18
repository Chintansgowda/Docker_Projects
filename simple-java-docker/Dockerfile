# 1. Use base image with Java Development Kit (JDK) version 17 (alpine = lightweight Linux distro)
FROM openjdk:17-jdk-alpine

# 2. Set an environment variable inside the container (can be accessed with $user)
ENV user=chintan

# 3. Set working directory inside the container (all next commands run from here)
WORKDIR /app

# 4. Copy Main.java file from your local "src" folder into the container's /app directory
COPY src/Main.java /app

# 5. Compile the Java program into bytecode (.class file) inside the container
RUN javac Main.java

# 6. Define the default command to run when container starts
#    → Runs the Java program by calling the Main class
ENTRYPOINT ["java","Main"]
