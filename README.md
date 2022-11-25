# Set up MongoDB Drivers → Go

This guide shows you how to create an application that uses the Go driver to connect to a MongoDB Atlas cluster.

# Set up Your Project

# Initialize with Go Mod

Create a new directory and initialize your project with go mod.

1.  mkdir go-quickstart
2.  cd go-quickstart
3.  go mod init go-quickstart

# Add MongoDB as a Dependency

    Use go get to add the Go driver as a dependency.
    go get go.mongodb.org/mongo-driver/mongo.

# `⚙️ GoDotEnv

A Go (golang) port of the Ruby dotenv project (which loads env vars from a .env file).

# `⚙️ Installation

    go get github.com/joho/godotenv

# Usage

    1.  Add your application configuration to your .env file in the root of your project:
    S3_BUCKET=YOURS3BUCKET
    SECRET_KEY=YOURSECRETKEYGOESHERE

    func main() {
    err := godotenv.Load()
    if err != nil {
        log.Fatal("Error loading .env file")
    }

    s3Bucket := os.Getenv("S3_BUCKET")
    secretKey := os.Getenv("SECRET_KEY")

    // now do something with s3 or whatever
    }

# `ScreenShot`

<img src="1.png">
