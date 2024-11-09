<template>
  <v-data-table hover="true" search color="pink" :headers="headers" :items="items" hide-default-footer="true"
    :items-per-page="-1">

    <template v-slot:item.logo="{ item }">
      <v-img :src="item.logo" height="32" width="32" cover></v-img>

    </template>

    <template v-slot:item.MyKnowledge="{ item }">

      <v-progress-linear bg-color="indigo-darken-0" color="indigo-darken-2" :model-value="item.MyKnowledge"></v-progress-linear>

    </template>


  </v-data-table>
</template>
<script>
import awx from '@/assets/technologylogo/awx.png'
import containerd from '@/assets/technologylogo/containerd.png'
import sonarqube from '@/assets/technologylogo/sonarqube.png'
import rabbitmq from '@/assets/technologylogo/rabbitmq.png'
import helm from '@/assets/technologylogo/helm.png'
import kustomize from '@/assets/technologylogo/kustomize.png'
import harbor from '@/assets/technologylogo/harbor.png'
import metallb from '@/assets/technologylogo/metallb.png'
import lxc from '@/assets/technologylogo/lxc.png'
import nginx from '@/assets/technologylogo/nginx.png'
import robotlogo from '@/assets/technologylogo/robot-logo.png'
import kubespray from '@/assets/technologylogo/kubespray.png'
import poetry from '@/assets/technologylogo/poetry.png'
import kvm from '@/assets/technologylogo/kvm.png'
import celery from '@/assets/technologylogo/celery.png'
import minio from '@/assets/technologylogo/minio.png'
import websockets from '@/assets/technologylogo/websocket.png'
import typer from '@/assets/technologylogo/typer.png'
import streamlit from '@/assets/technologylogo/streamlit.png'
import sphinx from '@/assets/technologylogo/sphinx.png'
import hugo from '@/assets/technologylogo/hugo.png'
import foreman from '@/assets/technologylogo/foreman.svg'
import maas from '@/assets/technologylogo/maas.png'



export default {
  name: 'MyComponent',
  data() {
    return {
      awx,
      containerd,
      sonarqube,
      rabbitmq,
      helm,
      kustomize,
      harbor,
      metallb,
      lxc,
      nginx,
      robotlogo,
      kubespray,
      poetry,
      kvm,
      celery,
      minio,
      websockets,
      typer,
      streamlit,
      sphinx,
      hugo,
      foreman,
      maas,
      headers: [
        { title: '', value: 'logo' },
        { title: 'Technology', value: 'Technology' },
        { title: 'Recently worked version', value: 'Recently_worked_version' },
        { title: 'MyKnowledge', value: 'MyKnowledge' },
      ],
      items: [
        {
          logo: awx,
          Technology: 'Ansible AWX',
          Recently_worked_version: '23.0',
          MyKnowledge: '90'
        },
        {
          logo: containerd,
          Technology: 'containerd',
          Recently_worked_version: '1.7',
          MyKnowledge: '90'
        },
        {
          logo: lxc,
          Technology: 'LXC',
          Recently_worked_version: '5.0',
          MyKnowledge: '90'
        },
        {
          logo: sonarqube,
          Technology: 'SonarQube',
          Recently_worked_version: '9.9',
          MyKnowledge: '90'
        },
        {
          logo: rabbitmq,
          Technology: 'RabbitMQ',
          Recently_worked_version: '3.12',
          MyKnowledge: '90'
        },
        {
          logo: kubespray,
          Technology: 'Kubespray',
          Recently_worked_version: '2.16',
          MyKnowledge: '90'
        },
        {
          logo: helm,
          Technology: 'Helm',
          Recently_worked_version: '3.14',
          MyKnowledge: '90'
        },
        {
          logo: kustomize,
          Technology: 'Kustomize',
          Recently_worked_version: '5.4',
          MyKnowledge: '90'
        },
        {
          logo: metallb,
          Technology: 'MetalLB',
          Recently_worked_version: '0.12',
          MyKnowledge: '90'
        },

        {
          logo: nginx,
          Technology: 'Nginx Ingress',
          Recently_worked_version: '1.25.3',
          MyKnowledge: '90'
        },
        {
          logo: robotlogo,
          Technology: 'Robot Framework',
          Recently_worked_version: '6.1',
          MyKnowledge: '90'
        },


        {
          logo: minio,
          Technology: 'Minio',
          Recently_worked_version: 'RELEASE.2024-06-11T03-13-30Z',
          MyKnowledge: '90'
        },
        {
          logo: poetry,
          Technology: 'Poetry',
          Recently_worked_version: '1.8',
          MyKnowledge: '90'
        },

        {
          logo: celery,
          Technology: 'Celery',
          Recently_worked_version: '5.4',
          MyKnowledge: '90'
        },
        {
          logo: websockets,
          Technology: 'Websockets',
          Recently_worked_version: '12',
          MyKnowledge: '90'
        },
        {
          logo: typer,
          Technology: 'Typer',
          Recently_worked_version: '0.12',
          MyKnowledge: '90'
        },
        {
          logo: streamlit,
          Technology: 'Streamlit',
          Recently_worked_version: '1.35',
          MyKnowledge: '90'
        },
        {
          logo: sphinx,
          Technology: 'Sphinx',
          Recently_worked_version: '7.3',
          MyKnowledge: '90'
        },
        {
          logo: hugo,
          Technology: 'Hugo',
          Recently_worked_version: '0.127',
          MyKnowledge: '90'
        },
        {
          logo: kvm,
          Technology: 'KVM',
          Recently_worked_version: '-',
          MyKnowledge: '90'
        },
        {
          logo: foreman,
          Technology: 'Foreman',
          Recently_worked_version: '3.10',
          MyKnowledge: '90'
        },
        {
          logo: maas,
          Technology: 'MAAS',
          Recently_worked_version: '3.4',
          MyKnowledge: '90'
        },

      ]
    };
  }
}


</script>