# KDX-AWS-Admin-Panel

Welcome to the KDX-AWS-Admin-Panel project! This project is an innovative landing page designed to simplify cloud management tasks for AWS EC2 instances. It serves as a user-friendly interface that enables users to start or stop EC2 instances with ease, and even schedule these tasks for better automation and efficiency. 

## Project Overview

The KDX-AWS-Admin-Panel is currently under development and embodies a concept aimed at enhancing user interaction with AWS resources. The project leverages a modern tech stack, incorporating Astro for the frontend to ensure a lightning-fast, static site generation, and FastAPI for the backend, offering a high-performance, easy-to-use framework to build APIs with Python.

This project is uniquely tailored for users seeking a straightforward interface to manage EC2 instances without delving into the complexities of AWS management consoles or extensive CLI commands.

### Features

- **EC2 Instance Management**: Start or stop your EC2 instances directly from the web interface.
- **Scheduling**: Plan your instances to start or stop at specific times, optimizing resource usage and reducing costs.
- **Notifications**: (Upcoming) Receive updates on your EC2 instances' status through Telegram notifications.

### Key Technologies

- **Frontend**: [Astro](https://astro.build/)
- **Backend**: [FastAPI](https://fastapi.tiangolo.com/)
- **AWS SDK**: [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) for AWS interaction
- **Notifications**: (Planned) [python-telegram-bot](https://python-telegram-bot.org/) for sending alerts and updates

## Getting Started

To get started with the KDX-AWS-Admin-Panel, clone this repository and ensure you have the prerequisites installed on your system.

### Prerequisites

- Python 3.8 or later
- Node.js and npm (for Astro frontend)

### Environment Setup

The project requires setting up several environment variables to handle AWS authentication and database connectivity securely. Please create a `.env` file in the project root with the following variables:

```dotenv
AWS-CONNECTION-STRING=your_aws_token_here
DDBB_USER=your_database_user
DDBB_PASS=your_database_password
DDBB_HOST=your_database_host
DDBB_NAME=your_database_name
```

**Note**: Replace `your_aws_token_here` and the database credentials with your actual AWS connection string and database details.

### Installation

1. **Backend Setup**:

   Navigate to the backend directory and install the required Python dependencies.

   ```bash
   cd backend
   pip install -r requirements.txt
   ```

2. **Frontend Setup**:

   Navigate to the frontend directory and install the necessary npm packages.

   ```bash
   cd ../frontend
   npm install
   ```

### Running the Application

To launch the KDX-AWS-Admin-Panel, you need to start both the frontend and backend servers.

- **Start the Backend**:

  ```bash
  uvicorn main:app --reload
  ```

- **Start the Frontend**:

  ```bash
  npm start
  ```

Now, navigate to `http://localhost:3000` in your browser to access the KDX-AWS-Admin-Panel landing page.

## Contributing

The KDX-AWS-Admin-Panel is an open project, and contributions are welcome. If you're interested in improving the project or adding new features, please feel free to fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

