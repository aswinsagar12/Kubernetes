Welcome to my Kubernetes Repository! 👋

This repository is a collection of my experiments, examples, and projects as I deep-dive into the world of Kubernetes. Here, I explore Kubernetes concepts, configurations, and best practices. This repository is a work-in-progress as I continuously learn and practice. Contributions and feedback are welcome!

🛠️ Repository Contents
- Basic Kubernetes Objects: Examples of Pods, Deployments, Services, ConfigMaps, and Secrets.
- Networking: Practicing with Services, Ingress resources, and network policies.
- Storage: Configurations for Persistent Volumes and Persistent Volume Claims.
- Resource Management: Examples of CPU and memory resource requests and limits.
- Helm Charts: Custom Helm charts for deploying applications in Kubernetes.
- Advanced Topics: Includes configurations for StatefulSets, DaemonSets, Jobs, and CronJobs.
- CI/CD Integrations: Kubernetes configurations for automating deployments in CI/CD pipelines.

🚀 Getting Started
To replicate and run these configurations on your own setup:

1. Install Minikube: A local Kubernetes cluster can be set up with Minikube.
2. Set Up kubectl: Install the Kubernetes CLI tool kubectl for managing the cluster.

Clone This Repository:

```bash
git clone https://github.com/aswinsagar12/kubernetes.git
cd kubernetes
```

Apply Kubernetes Files:

```bash
kubectl apply -f <filename>.yaml
```

🌱 Current Focus Areas
- Understanding core concepts such as Pods, Services, and Ingress.
- Working with StatefulSets for stateful applications.
- Setting up networking and access controls for secure deployments.
- Experimenting with resource management to optimize performance.

🚀 Ingress Demo Application
To set up and run an Ingress demo application, follow these steps:

1. **Enable the Ingress Add-on in Minikube:**
   ```bash
   minikube addons enable ingress
   ```

2. **Build the Flask Application Docker Image:**
   Change to the Flask application directory and build the Docker image:
   ```bash
   cd Flask
   docker build -t flaskapp:v1 .
   ```
   Verify the image was built successfully:
   ```bash
   docker images
   ```

3. **Apply Kubernetes Configuration Files:**
   Once the image is built, return to the repository directory and apply the necessary Kubernetes configurations for the Service, Deployment, and Ingress:
   ```bash
   kubectl apply -f service.yaml
   kubectl apply -f deployment.yaml
   kubectl apply -f ingress.yaml
   ```

4. **Validate the Application:**
   Check if the application is running correctly by accessing it through the Ingress resource.

📚 Learning Resources
As I progress, I'm referencing these Kubernetes resources:

- Kubernetes Official Documentation
- Kubernetes on GitHub
- Kubernetes Patterns

🤝 Contributions
This repository is primarily for my own learning, but if you have ideas or suggestions, feel free to submit issues or pull requests!
```