
# ECE DevOps course

Materials for the DevOps course at ECE.

## Modules

1. Introduction to DevOps
2. Source Control Management (SCM)
3. Infrastructure as code (IaC) | with Ansible
4. Continuous Testing
5. Continuous Integration & Continuous Delivery (CI/CD) | with GitHub Actions and Heroku
6. Containerization | with Docker
7. Containers orchestration | with Kubernetes
8. Cloud-native applications. Microservice architecture | with Istio
9. Monitoring | with Prometheus and Grafana

## Assignment

The course assignment is consist of:

1. Participation
2. Project
3. MCQ exam (multiple choice questions)

## Usage

### Reading slides' content

Navigate inside the [`./devops`](devops) folder to read the raw material and access the labs. The module's folders contain following files:

- `index.md` - materials for the module
- `slides.pdf` - PDF slides
- `lab.md` - labs description
- `homework.md` - homework description
- `assets` folder - assets provided for the labs
- `image` folder - images used in the `.md` files

### Access online slides

The slides are available on Netlify as a static website - [ece-devops-2021-fall.netlify.app](https://ece-devops-2021-fall.netlify.app/).

[![Netlify Status](https://api.netlify.com/api/v1/badges/33fe7da7-8056-40c4-abc1-50563277ba50/deploy-status)](https://app.netlify.com/sites/amazing-goldstine-aa6378/deploys)

### Build slides locally as a static website

Run the following commands to get the site up and running.

```
# Clone the repository
git clone https://github.com/adaltas/ece-devops-2021-fall.git devops
cd devops/slide-builder
# Download the dependencies
npm install
# Start the development server
npm run develop
# If you have problem, try
npm run clean && npm run develop
```

## Author

Sergei Kudinov   
sergei@adaltas.com     
Developer and Big Data Engineer at [Adaltas](https://www.adaltas.com/)
