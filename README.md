GitHub Repository -> SonarQube Static Code Analysis -> Build Docker Image -> Trivy Image Scan
                                    |                       |
                                    |                       |
                                    v                       v
                             Build Passing?           No Vulnerabilities Found?
                                    |                       |
                                    |                       |
                                    v                       v
                           Yes -> Deploy to EKS <- Yes <- Continue Deployment
                                    |                       |
                                    |                       |
                                    v                       v
                     SBOM Container Packages Scan     Falco to Monitor Processes Inside Containers
