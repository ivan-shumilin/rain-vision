# RainSense: AI-Powered Rain Detection System

![Python](https://img.shields.io/badge/Python-3.12-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-orange.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-red.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100.0-green.svg)
![Docker](https://img.shields.io/badge/Docker-24.0.5-blue.svg)
![Poetry](https://img.shields.io/badge/Poetry-1.7.1-purple.svg)

RainSense is a computer vision project that uses artificial intelligence to detect and analyze rainfall in real-time. The system processes video streams and images to identify the presence and intensity of rain, providing accurate weather monitoring capabilities.

## Features

- Real-time rain detection
- Rain intensity classification (light/medium/heavy)
- Weather condition logging
- Web interface for monitoring
- API integration capabilities
- Support for IP cameras
- Historical data analysis

## Tech Stack

- Python 3.12
- OpenCV
- TensorFlow/PyTorch
- FastAPI
- PostgreSQL
- NumPy
- Pandas
- Docker & Docker Compose
- Poetry

## Prerequisites

- Docker
- Docker Compose
- Poetry (for local development)

## Installation & Running

1. Clone the repository:
```bash
git clone https://github.com/yourusername/rainsense.git
cd rainsense
```

2. Create environment file:
```bash
cp .env.example .env
```

3. Build and start the containers:
```bash
docker-compose up --build
```

4. Access the application:
- Web Interface: http://localhost:8000
- API Documentation: http://localhost:8000/docs
- API ReDoc: http://localhost:8000/redoc

## Project Structure

```
rainsense/
├── app/
│   ├── main.py           # FastAPI application
│   ├── models/           # ML models
│   ├── static/           # Static files
│   ├── templates/        # HTML templates
│   └── utils/            # Utility functions
├── docker/
│   ├── Dockerfile        # Main application Dockerfile
│   └── poetry.lock       # Poetry lock file
├── pyproject.toml        # Poetry project configuration
├── docker-compose.yml    # Docker Compose configuration
├── .env.example         # Example environment variables
└── README.md            # Project documentation
```

## Development

For local development:

1. Install Poetry:
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

2. Install dependencies:
```bash
poetry install
```

3. Start the development environment:
```bash
docker-compose -f docker-compose.dev.yml up --build
```

4. Run tests:
```bash
poetry run pytest
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- OpenCV community
- TensorFlow team
- All contributors and supporters

## Contact

TG: https://t.me/shumilinivan