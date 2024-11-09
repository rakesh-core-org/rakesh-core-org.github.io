<template>
    <div>
        <!-- <v-img :src=require("@/assets/technologylogo/mssql.png")></v-img> -->
        <v-row no-gutters>
            <v-col cols="1">
                <v-img :width="30" :height="30" :src="imageSrc" alt="devops logo"></v-img>
            </v-col>
            <v-col cols="5" >
                <h2>DevOps</h2>
            </v-col>
        </v-row>
        <ul>
            <li>Configured and maintained Kubernetes clusters (on-premise and AKS), utilizing PV, PVC, secrets, services, StatefulSets, Deployments, and Ingress components.</li>
            <li>Implemented KEDA for HPA based on external metrics, custom Helm charts for 18 applications, and kustomize files.</li>
            <li>Utilized MetalLB for load balancing in on-premise clusters, and Velero with minIO for cluster backups.</li>
            <li>Experience in <a href="">kind</a> kubernetes cluster for local testing</li>
            <li>Managed environment-specific secrets with HashiCorp Vault and injected secrets into Kubernetes pods.</li>
            <li>Solid experience utilizing LXC containers for local testing and development environments.</li>
            <li>Deployed multiple clusters using Kubespray and performed local testing with kind Kubernetes clusters.</li>
            <li>Managed Docker Swarm clusters with 80+ production servers, monitoring 400+ containers and 100+ servers using Splunk and Grafana Loki.</li>
            <li>Created and maintained Docker Swarm environments, including volumes, networks, and plugins.</li>
            <li>Automated workflows and administration with GitHub, GitHub Actions, and GitHub Enterprise; migrated GitLab pipelines to GitHub Actions.</li>
            <li>Implemented self-hosted GitHub using ARC and GitLab runners, and managed secrets via github</li>
            <li>Used Argo CD for GitOps workflows, ensuring consistent application configuration, and rotated TLS SAN certificates in Kubernetes ingress controllers.</li>
            <li>Measured code quality with SonarQube and automated code formatting with pre-commit hooks.</li>
            <li>Configured Jenkins slaves and wrote pipeline jobs for CI/CD</li>
            <li>utilizing Django channels for live notifications and OpenTelemetry for tracing and monitoring.</li>
            <li>Implemented opentelemetry in microservices for tracing and monitoring </li>
            <li>Channalised all python setup using poetry </li>
            <li>Automated functional test using robot framework</li>
            <li>Experienced in using AWX and ansible-runners in Python, customizing ansible-execution environments.</li>
            <li>Having good experience in mongodb </li>
            <li>Experience in using celery for distributing tasks and for scheduling tasks</li>
            <li>Utilized Hugo for static site generation, Sphinx for documentation, and Mermaid for creating diagrams and flowcharts.</li>
        </ul>
    </div>
</template>

<script>
import imageSrc from '@/assets/technologylogo/devops.png'

export default {
  name: 'MyComponent',
  data() {
    return {
      imageSrc
    };
  }
}
</script>