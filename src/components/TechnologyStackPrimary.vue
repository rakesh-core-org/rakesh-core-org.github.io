<template>
  <v-data-table hover="true" search color="pink" :headers="headers" :items="items" hide-default-footer="true"
    :items-per-page="-1">

    <template v-slot:item.logo="{ item }">
      <v-img :src="item.logo" height="32" width="32" cover></v-img>

    </template>

    <template v-slot:item.MyKnowledge="{ item }">

      <v-progress-linear bg-color="indigo-darken-0" color="indigo-darken-2" :model-value="item.MyKnowledge">
      </v-progress-linear>

    </template>


  </v-data-table>
</template>
<script>
import kubernetes from '@/assets/technologylogo/kubernetes.png'
import docker from '@/assets/technologylogo/docker-logo.png'
import azure from '@/assets/technologylogo/azure-logo.png'
import openstack from '@/assets/technologylogo/openstack.png'
import ansible from '@/assets/technologylogo/ansible.png'
import harbor from '@/assets/technologylogo/harbor.png'
import python from '@/assets/technologylogo/python.png'
import django from '@/assets/technologylogo/django.svg'
import fastapi from '@/assets/technologylogo/fastapi.svg'
import github from '@/assets/technologylogo/github.png'
import githubactions from '@/assets/technologylogo/github-actions.png'
import jenkins from '@/assets/technologylogo/jenkins.png'
import ceph from '@/assets/technologylogo/ceph.png'
import vault from '@/assets/technologylogo/vault.svg'
import vuejs from '@/assets/technologylogo/vuejs.png'
import mongodb from '@/assets/technologylogo/mongodb.png'
import postgresql from '@/assets/technologylogo/postgresql.png'
import argocd from '@/assets/technologylogo/argocd.png'
import keycloak from '@/assets/technologylogo/keycloak.png'
import grafana from '@/assets/technologylogo/grafana.png'
import prometheus from '@/assets/technologylogo/prometheus.png'
import loki from '@/assets/technologylogo/loki.png'
import opentelemetry from '@/assets/technologylogo/opentelemetry.png'
import langchain from '@/assets/technologylogo/langchain.jpg'


export default {
  name: 'MyComponent',
  data() {
    return {
      kubernetes,
      docker,
      azure,
      openstack,
      ansible,
      harbor,
      python,
      django,
      fastapi,
      github,
      githubactions,
      jenkins,
      ceph,
      vault,
      vuejs,
      mongodb,
      postgresql,
      argocd,
      keycloak,
      grafana,
      prometheus,
      loki,
      opentelemetry,
      langchain,
      headers: [
        { title: '', value: 'logo' },
        { title: 'Technology', value: 'Technology' },
        { title: 'Recently worked version', value: 'Recently_worked_version' },
        { title: 'MyKnowledge', value: 'MyKnowledge' },
      ],
      items: [
        {
          logo: kubernetes,
          Technology: 'Kubernetes',
          Recently_worked_version: 'v1.5',
          MyKnowledge: '90'
        },
        {
          logo: docker,
          Technology: 'Docker',
          Recently_worked_version: 'v1.5',
          MyKnowledge: '90'
        },
        {
          logo: azure,
          Technology: 'Azure cloud',
          Recently_worked_version: '-',
          MyKnowledge: '60'
        },
        {
          logo: openstack,
          Technology: 'Openstack',
          Recently_worked_version: 'Zed',
          MyKnowledge: '80'
        },
        {
          logo: ansible,
          Technology: 'Ansible',
          Recently_worked_version: '2.17',
          MyKnowledge: '90'
        },
        {
          logo: harbor,
          Technology: 'Harbor',
          Recently_worked_version: '2.10',
          MyKnowledge: '90'
        },
        {
          logo: python,
          Technology: 'Python',
          Recently_worked_version: '3.11',
          MyKnowledge: '80'
        },
        {
          logo: django,
          Technology: 'Django',
          Recently_worked_version: '5.0',
          MyKnowledge: '80'
        },
        {
          logo: fastapi,
          Technology: 'Fastapi',
          Recently_worked_version: '0.110',
          MyKnowledge: '80'
        },
        {
          logo: github,
          Technology: 'Github',
          Recently_worked_version: '-',
          MyKnowledge: '90'
        },
        {
          logo: githubactions,
          Technology: 'Github actions',
          Recently_worked_version: '-',
          MyKnowledge: '90'
        },
        {
          logo: jenkins,
          Technology: 'Jenkins',
          Recently_worked_version: '2.282',
          MyKnowledge: '90'
        },
        {
          logo: ceph,
          Technology: 'Ceph',
          Recently_worked_version: 'Reef',
          MyKnowledge: '90'
        },
        {
          logo: vault,
          Technology: 'Hashicorp vault',
          Recently_worked_version: '1.16',
          MyKnowledge: '90'
        },
        {
          logo: vuejs,
          Technology: 'vuejs',
          Recently_worked_version: '3.4',
          MyKnowledge: '90'
        },
        {
          logo: mongodb,
          Technology: 'mongodb',
          Recently_worked_version: '7.0',
          MyKnowledge: '90'
        },
        {
          logo: postgresql,
          Technology: 'Postgres',
          Recently_worked_version: '16',
          MyKnowledge: '90'
        },
        {
          logo: argocd,
          Technology: 'ArgoCD',
          Recently_worked_version: '2.11',
          MyKnowledge: '90'
        },
        {
          logo: keycloak,
          Technology: 'Keycloak',
          Recently_worked_version: '25.0',
          MyKnowledge: '90'
        },
        {
          logo: grafana,
          Technology: 'Grafana',
          Recently_worked_version: '11.0',
          MyKnowledge: '90'
        },
        {
          logo: prometheus,
          Technology: 'Prometheus',
          Recently_worked_version: '2.52',
          MyKnowledge: '90'
        },
        {
          logo: loki,
          Technology: 'Loki',
          Recently_worked_version: '2.9',
          MyKnowledge: '90'
        },
        {
          logo: opentelemetry,
          Technology: 'Opentelemetry',
          Recently_worked_version: '1.25',
          MyKnowledge: '90'
        },
        {
          logo: langchain,
          Technology: 'Langchain',
          Recently_worked_version: '0.2',
          MyKnowledge: '90'
        },
      ]
    };
  }
}


</script>
