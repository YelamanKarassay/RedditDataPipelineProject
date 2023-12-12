# Reddit Data Pipeline Project

## Overview

The Reddit Data Pipeline Project is designed to stream data from Reddit using Python, process it through Apache Kafka, analyze it with Apache Spark, and orchestrate the entire pipeline using Docker. This project aims to demonstrate real-time data processing and analytics capabilities.

## Features

- **Real-Time Data Streaming**: Streams live data from Reddit.
- **Message Brokering with Kafka**: Efficient handling and queuing of streaming data.
- **Data Processing with Spark**: Real-time data analysis and processing.
- **Dockerized Environment**: Each component runs in a Docker container for easy setup and deployment.

## Prerequisites

Before you begin, ensure you have the following installed:
- Docker and Docker Compose
- Git (for version control)

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YelamanKarassay/RedditDataPipelineProject.git
   cd RedditDataPipelineProject
   ```

2. **Set up Environment Variables**:
   - Copy the `.env.example` file to a new file named `.env`.
   - Fill in your Reddit API credentials and other necessary environment variables.

3. **Build and Run with Docker Compose**:
   ```bash
   docker-compose up --build
   ```

## Usage

Once the system is running:
- The Reddit Streaming Application will start streaming posts and comments from the specified criteria.
- Kafka will queue these messages, which will then be processed by the Spark application.
- The processed data can be viewed in the logs or extended to be stored in a database or displayed on a dashboard.

## Architecture

Refer to the [architecture.md](/docs/architecture.md) file for a detailed description of the project's architecture.

## Contributing

Contributions to the project are welcome. Please follow the standard fork, branch, and pull request workflow.

## License

This project is licensed under the [LICENSE.md](LICENSE) - see the LICENSE file for details.

## Acknowledgments

- Reddit API for providing the data source.
- Open-source communities of Apache Kafka, Apache Spark, and Docker for their invaluable resources.
