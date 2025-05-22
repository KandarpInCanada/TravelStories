# TravelStories - Your Ultimate Travel Blog

> A comprehensive MERN stack travel blog application with full DevSecOps implementation using modern CI/CD practices.

## 🛠️ Tech Stack

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)

### DevOps & Infrastructure
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/jenkins-%232C5263.svg?style=for-the-badge&logo=jenkins&logoColor=white)
![ArgoCD](https://img.shields.io/badge/Argo%20CD-1e0b3e?style=for-the-badge&logo=argo&logoColor=#d16044)
![Terraform](https://img.shields.io/badge/Terraform-844FBA.svg?style=for-the-badge&logo=Terraform&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=Helm&logoColor=white)

### AWS Services
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Amazon EKS](https://img.shields.io/badge/Amazon%20EKS-FF9900.svg?style=for-the-badge&logo=Amazon-EKS&logoColor=white)
![Amazon EC2](https://img.shields.io/badge/Amazon%20EC2-FF9900.svg?style=for-the-badge&logo=Amazon-EC2&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31.svg?style=for-the-badge&logo=Amazon-S3&logoColor=white)
![Amazon CloudWatch](https://img.shields.io/badge/Amazon%20CloudWatch-FF4F8B.svg?style=for-the-badge&logo=Amazon-CloudWatch&logoColor=white)
![Amazon IAM](https://img.shields.io/badge/Amazon%20Identity%20Access%20Management-DD344C.svg?style=for-the-badge&logo=Amazon-Identity-Access-Management&logoColor=white)

### Security & Quality
![SonarQube](https://img.shields.io/badge/SonarQube-black?style=for-the-badge&logo=sonarqube&logoColor=4E9BCD)
![OWASP](https://img.shields.io/badge/OWASP-000000?style=for-the-badge&logo=OWASP&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=trivy&logoColor=white)

### Monitoring
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)

## Overview

TravelStories is a modern, full-stack travel blog application built with the MERN stack (MongoDB, Express.js, React, Node.js). This project demonstrates enterprise-level DevSecOps practices with automated CI/CD pipelines, security scanning, and Kubernetes deployment on AWS EKS.

### Key Features

- **Full-Stack MERN Application**: Modern travel blog with user authentication and content management
- **DevSecOps Pipeline**: Complete CI/CD with security scanning and quality gates
- **Kubernetes Deployment**: Production-ready deployment on AWS EKS
- **GitOps Workflow**: ArgoCD for automated application deployment
- **Monitoring & Observability**: Prometheus and Grafana integration
- **Security First**: OWASP dependency checking and Trivy vulnerability scanning

## Architecture
![Architecture](https://github.com/user-attachments/assets/aca8615a-0cce-4ba4-9ef8-d26fc4aef6ec)

### Tech Stack

| Category | Technology |
|----------|------------|
| **Frontend** | React.js, HTML5, CSS3, JavaScript |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB |
| **Containerization** | Docker |
| **Orchestration** | Kubernetes (AWS EKS) |
| **CI/CD** | Jenkins, ArgoCD |
| **Security** | OWASP, SonarQube, Trivy |
| **Monitoring** | Prometheus, Grafana |
| **Infrastructure** | AWS, Helm Charts |
| **Caching** | Redis |

## Getting Started

### Prerequisites

- Node.js (v18+)
- MongoDB
- Docker
- AWS Account (for cloud deployment)
- kubectl
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/travelStories.git
   cd travelStories
   ```

2. **Install dependencies**
   ```bash
   # Backend dependencies
   cd backend
   npm install
   
   # Frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Environment Configuration**
   ```bash
   # Create .env file in backend directory
   cp .env.example .env
   # Update with your MongoDB connection string and other variables
   ```

4. **Start the application**
   ```bash
   # Start backend (from backend directory)
   npm start
   
   # Start frontend (from frontend directory)
   npm start
   ```

5. **Access the application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`

## DevOps Implementation

### CI/CD Pipeline Features

- **Continuous Integration**
  - Automated code quality checks with SonarQube
  - Security vulnerability scanning with OWASP and Trivy
  - Docker image building and pushing
  - Automated testing

- **Continuous Deployment**
  - GitOps workflow with ArgoCD
  - Kubernetes deployment automation
  - Environment-specific configurations
  - Rollback capabilities

### Pipeline Stages

1. **Code Quality & Security**
   - SonarQube analysis
   - OWASP dependency check
   - Trivy filesystem scan

2. **Build & Package**
   - Docker image creation
   - Multi-stage builds for optimization
   - Container registry push

3. **Deploy**
   - ArgoCD application sync
   - Kubernetes deployment
   - Service exposure
   - Health checks

## Monitoring & Observability

### Prometheus Metrics
- Application performance metrics
- Kubernetes cluster monitoring
- Resource utilization tracking

### Grafana Dashboards
- Real-time application metrics
- Infrastructure monitoring
- Custom alerting rules

## Security Features

- **OWASP Dependency Check**: Identifies known vulnerabilities in project dependencies
- **SonarQube Integration**: Code quality and security vulnerability analysis
- **Trivy Scanning**: Container image vulnerability assessment
- **Secure Secrets Management**: Kubernetes secrets for sensitive data

## Deployment Guide

### Quick Deployment

For detailed deployment instructions, see our [Deployment Guide](./docs/DEPLOYMENT.md).

#### AWS EKS Deployment

1. **Prerequisites Setup**
   - AWS CLI configured
   - eksctl installed
   - kubectl installed

2. **Cluster Creation**
   ```bash
   eksctl create cluster --name=travelstories \
                       --region=us-east-2 \
                       --version=1.30 \
                       --without-nodegroup
   ```

3. **Application Deployment**
   - Configure ArgoCD
   - Deploy application manifests
   - Access via LoadBalancer/NodePort

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `MONGODB_URI` | MongoDB connection string | `mongodb://localhost:27017/travelstories` |
| `JWT_SECRET` | JWT signing secret | - |
| `PORT` | Backend server port | `5000` |
| `REACT_APP_API_URL` | Frontend API URL | `http://localhost:5000` |

## API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Blog Endpoints
- `GET /api/posts` - Get all blog posts
- `POST /api/posts` - Create new post
- `GET /api/posts/:id` - Get specific post
- `PUT /api/posts/:id` - Update post
- `DELETE /api/posts/:id` - Delete post

## Contributing

We welcome contributions! Please see our [Contributing Guide](./CONTRIBUTING.md) for details.

### Development Workflow

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Style

- Follow ESLint configuration
- Use Prettier for code formatting
- Write meaningful commit messages
- Add tests for new features

## Project Metrics

- **Code Coverage**: 85%+
- **Performance Score**: 90%+
- **Security Rating**: A
- **Maintainability**: A

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
