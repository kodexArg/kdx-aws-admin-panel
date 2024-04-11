# KDX-AWS-Admin-Panel

Welcome to the KDX-AWS-Admin-Panel project! This application serves a page designed to simplify cloud management tasks for AWS EC2 instances. It acts as an interface that allows users to start or stop EC2 instances with ease, and even schedule these tasks for better automation and efficiency.

This project is specially designed for users without access to complex systems, who only need a simple interface to manage these instances within their organization.

### Features

- **EC2 Instance Management**: Start or stop your EC2 instances directly from the web interface.
- **Scheduling**: Plan your instances to start or stop at specific times, optimizing resource usage and reducing costs.
- **Notifications**: (Coming Soon) Receive updates on the status of your EC2 instances through Telegram notifications.

### Technologies

- **Frontend**: HTMX for dynamic interactivity without needing to reload the page.
- **Backend**: [FastAPI](https://fastapi.tiangolo.com/) for API creation with Python, offering a high-performance solution for the backend.
- **AWS SDK**: [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) for AWS interaction, allowing direct management of AWS services from the application.
- **Notifications**: (Planned) [python-telegram-bot](https://python-telegram-bot.org/) for sending alerts and updates.

```
.
├── app.py
├── static
│   ├── css
│   │   └── tailwind.min.css
│   └── js
│       └── htmx.js
└── templates
    └── index.html
```

### Environment Setup

Configure several environment variables to handle AWS authentication securely. Create a `.env` file at the root of the project as follows:

```
AWS_ACCESS_KEY_ID=your_aws_access_key_id
AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
AWS_DEFAULT_REGION=your_aws_region
```

**Note**: Replace the values with your own AWS credentials, which must have the minimum permissions necessary to start, stop, and query the EC2 instances you need to modify.

## TODO:
[ ] JSON for the AWS user
[ ] Implement python-telegram-bot
[ ] Implement HTMX for frontend interactivity

## Contributing

The KDX-AWS-Admin-Panel is an open project, and contributions are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.