<template>
  <v-data-table hover="true" search color="pink" :headers="headers" :items="items" hide-default-footer="true"
    :items-per-page="-1">

    <template v-slot:item.logo="{ item }">
      <v-img :src="item.logo" height="32" width="32" cover></v-img>

    </template>

    <template v-slot:item.MyKnowledge="{ item }">

      <v-progress-circular bg-color="indigo-darken-0" color="indigo-darken-2" :width="4" :size="40" :model-value="item.MyKnowledge">
        <template v-slot:default> {{ item.MyKnowledge }}% </template>
      </v-progress-circular>

    </template>


  </v-data-table>
</template>
<script>
import awx from '@/assets/technologylogo/awx.png'
import splunk from '@/assets/technologylogo/splunk.png'
import gitlab from '@/assets/technologylogo/gitlab.png'
import kind from '@/assets/technologylogo/kind.png'
import thanos from '@/assets/technologylogo/thanos.png'
import podman from '@/assets/technologylogo/podman.png'
import sssd from '@/assets/technologylogo/sssd.png'
import bitbucket from '@/assets/technologylogo/bitbucket.svg'
import istio from '@/assets/technologylogo/istio.png'
import Nexus from '@/assets/technologylogo/nexus.png'
import NFS from '@/assets/technologylogo/nfs.png'
import velero from '@/assets/technologylogo/velero.jpg'
import terraform from '@/assets/technologylogo/terraform.png'
import sqlserver from '@/assets/technologylogo/sqlserver.png'
import oracle from '@/assets/technologylogo/oracle.png'
import tls from '@/assets/technologylogo/tls.png'
import dockerswarm from '@/assets/technologylogo/docker-swarm.png'
import jira from '@/assets/technologylogo/jira.png'
import confluence from '@/assets/technologylogo/confluence.png'
import precommit from '@/assets/technologylogo/pre-commit.svg'




export default {
  name: 'MyComponent',
  data() {
    return {
      awx,

      headers: [
        { title: '', value: 'logo' },
        { title: 'Technology', value: 'Technology' },
        { title: 'Recently worked version', value: 'Recently_worked_version' },
        { title: 'MyKnowledge', value: 'MyKnowledge' },
      ],
      items: [

        {
          logo: gitlab,
          Technology: 'Gitlab',
          Recently_worked_version: '14.0',
          MyKnowledge: '60'
        },
        {
          logo: bitbucket,
          Technology: 'Bitbucket',
          Recently_worked_version: '6.10',
          MyKnowledge: '60'
        },
        {
          logo: kind,
          Technology: 'Kind',
          Recently_worked_version: '0.23',
          MyKnowledge: '80'
        },

        {
          logo: dockerswarm,
          Technology: 'Docker swarm',
          Recently_worked_version: '-',
          MyKnowledge: '60'
        },
        {
          logo: podman,
          Technology: 'Podman',
          Recently_worked_version: '5.1',
          MyKnowledge: '50'
        },
        {
          logo: thanos,
          Technology: 'Thanos',
          Recently_worked_version: '0.23.2',
          MyKnowledge: '70'
        },
        {
          logo: splunk,
          Technology: 'splunk',
          Recently_worked_version: '7.3',
          MyKnowledge: '40'
        },
        {
          logo: sssd,
          Technology: 'sssd',
          Recently_worked_version: '-',
          MyKnowledge: '60'
        },

        {
          logo: istio,
          Technology: 'Istio',
          Recently_worked_version: '1.19',
          MyKnowledge: '30'
        },
        {
          logo: Nexus,
          Technology: 'Nexus',
          Recently_worked_version: '3.45',
          MyKnowledge: '30'
        },
        {
          logo: NFS,
          Technology: 'NFS',
          Recently_worked_version: 'v4',
          MyKnowledge: '70'
        },
        {
          logo: velero,
          Technology: 'Velero',
          Recently_worked_version: '1.9',
          MyKnowledge: '50'
        },
        // { 
        //   logo: terraform,
        //   Technology: 'Terraform',
        //   Recently_worked_version: '-',
        //   MyKnowledge: '90'
        // },
        {
          logo: sqlserver,
          Technology: 'SQL server',
          Recently_worked_version: '2016,2019',
          MyKnowledge: '50'
        },
        {
          logo: oracle,
          Technology: 'Oracle database',
          Recently_worked_version: '12c',
          MyKnowledge: '40'
        },
        {
          logo: tls,
          Technology: 'TLS',
          Recently_worked_version: '1.3',
          MyKnowledge: '60'
        },

        {
          logo: jira,
          Technology: 'Jira',
          Recently_worked_version: '9.4',
          MyKnowledge: '80'
        },
        {
          logo: confluence,
          Technology: 'Confluence',
          Recently_worked_version: '1.19',
          MyKnowledge: '90'
        },
        {
          logo: precommit,
          Technology: 'Pre-commit',
          Recently_worked_version: '3.7',
          MyKnowledge: '90'
        },
      ]
    };
  }
}
</script>