Bring calmness to your builds
Cargo is the build tool for Rust. It bundles all common actions into a single command. No boilerplate required.

Install
With tens of thousands of packages, there’s a good chance crates.io has the solution you’re looking for. Stand on the shoulders of giants, and move your team from repetition to innovation.

Test
Bring confidence to your code through Rust’s excellent testing tools. cargo test is Rust’s unified solution to testing. Write tests next to your code, or in separate files: it provides a solution for all testing needs.

Deploy
cargo build creates lean binaries for every platform. With a single command your code can target Windows, Linux, macOS, and the web. All part of a modern interface, with no need for bespoke build files.

...

#!/bin/bash

# Function to display a message with a calm tone
calm_echo() {
    echo -e "\033[0;32m$1\033[0m"
}

# Install dependencies using Cargo
calm_echo "Installing dependencies with Cargo..."
cargo build

# Run tests using Cargo
calm_echo "Running tests with Cargo..."
cargo test

# Build the project for multiple platforms
calm_echo "Building the project for multiple platforms with Cargo..."
cargo build --target x86_64-unknown-linux-gnu
cargo build --target x86_64-pc-windows-msvc
cargo build --target x86_64-apple-darwin

# Deploy the project (example: copying the binaries to a deployment folder)
calm_echo "Deploying the project..."
mkdir -p deploy_folder
cp target/debug/your_binary deploy_folder/  # Adjust 'your_binary' with your actual binary name

calm_echo "Deployment completed successfully!"
