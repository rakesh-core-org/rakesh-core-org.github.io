<template>
  <div>
    <v-card title="History" variant="plain"></v-card>
    <v-timeline side="end">

      <v-timeline-item dot-color="cyan" size="small">
        <template v-slot:opposite>
          <v-tooltip text="~2 years">
            <template v-slot:activator="{ props }">
              <div v-bind="props" :class="`pt-1 headline font-weight-bold text-cyan`">June-2016 to May-2018</div>
              <p :class="`pt-1 subtitle font-weight-light mb-4 text-cyan`">Chennai, TN, India</p>
              <v-card min-width="600">
                <v-card-text>
                 
                  <v-data-table hover="true" search color="pink" :headers="bctheaders" :items="bctitems"
                    hide-default-footer="true" :items-per-page="-1">
                  </v-data-table>

                </v-card-text>
              </v-card>
            </template>
          </v-tooltip>
        </template>

        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-cyan`">
          Bhawancybertek
        </h2>

        <v-card class="mx-auto my-8" elevation="2" min-width="600">
          <v-card-item>
            <v-card-subtitle>
              Individual contribution
            </v-card-subtitle>
          </v-card-item>

          <v-card-text>
            <ul>

              <li>Automated oracle 12c Database installation using Ansible which saves 7 hours of manual work.</li>
              <li>Implemented health Check Automation for SQL server using PowerShell and CSS which reduced manual work of 3 hours per day</li>
            </ul>

          </v-card-text>
        </v-card>

      </v-timeline-item>


      <v-timeline-item dot-color="green" size="small">
        <template v-slot:opposite>
          <v-tooltip text="3 years">
            <template v-slot:activator="{ props }">
              <div v-bind="props" :class="`pt-1 headline font-weight-bold text-green`">May-2018 to June-2021</div>
              <p :class="`pt-1 subtitle font-weight-light mb-4 text-green`">Coimbatore, TN, India</p>
              <v-card min-width="600">
                <v-card-text>
                  <v-data-table hover="true" search color="pink" :headers="boschheaders" :items="boschitems"
                    hide-default-footer="true" :items-per-page="-1">
                  </v-data-table>
                </v-card-text>
              </v-card>
            </template>
          </v-tooltip>
        </template>

        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-green`">
          Robert Bosch
        </h2>



        <v-card class="mx-auto my-8" elevation="2" min-width="600">
          <v-card-item>
            <v-card-subtitle>
              Individual contribution
            </v-card-subtitle>
          </v-card-item>

          <v-card-text>
            <ul>
              <li>Designed and developed a Self-service portal for Jenkins Provisioning – Saves 4 hours of manual work per day</li>
              <li>Designed and developed an distributed application with Django Rest API, VueJs and  deployed in Kubernetes on premise for launching any Docker application container (XaaS -
                Anything as a Service)</li>
              <li>Implemented efficient monitoring solution of servers and Docker logs using Grafana/promtail/loki – saves debugging time</li>
            </ul>

          </v-card-text>
        </v-card>

      </v-timeline-item>


      <v-timeline-item dot-color="orange" size="small">
        <template v-slot:opposite>
          <v-tooltip text="3+ years">
            <template v-slot:activator="{ props }">
              <div v-bind="props" :class="`pt-1 headline font-weight-bold text-orange`">June-2021 to till date</div>
              <p :class="`pt-1 subtitle font-weight-light mb-4 text-orange`">Bengaluru, KA, India (WFH)</p>
              <v-card min-width="600">
                <v-card-text>
                  <v-data-table hover="true" search color="pink" :headers="amdheaders" :items="amditems"
                    hide-default-footer="true" :items-per-page="-1">
                  </v-data-table>

                </v-card-text>
              </v-card>
            </template>
          </v-tooltip>
        </template>

        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-orange`">
          Advanced Micro Devices
        </h2>
        



        <v-card class="mx-auto my-8" elevation="2" min-width="600">
          <v-card-item>
            <v-card-subtitle>
              Individual contribution
            </v-card-subtitle>
          </v-card-item>

          <v-card-text>
            <ul>

              <li>Migrated applications from on-premise to azure cloud</li>
              <li>Migration of on-premise kubernetes cluster to AKS with minimal downtime</li>
              <li>Developed a datacenter support virtual assistant using streamlit, langgraph and llama3</li>
              <li>Deployed a multi-node Openstack cloud for multi lab setup</li>
              <li>Architected and Developed an application for infrastructure tracking using microservice architecture.</li>
              <li>Migrated Gitlab to github including workflows</li>
            </ul>

          </v-card-text>
        </v-card>

      </v-timeline-item>



      <v-timeline-item dot-color="purple" size="small">
        <template v-slot:opposite>
          <v-tooltip text="3+ years">
            <template v-slot:activator="{ props }">
              <div v-bind="props" :class="`pt-1 headline font-weight-bold text-purple`"></div>
 
            </template>
          </v-tooltip>
        </template>

        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-purple`">
          What next?
        </h2>



        <v-card class="mx-auto my-8" elevation="2" min-width="600">

        </v-card>

      </v-timeline-item>


    </v-timeline>
  </div>
</template>

<script>
export default {
  data() {
    return {
      bctheaders: [
        { title: 'Role', value: 'role' },
        { title: 'Projects', value: 'projects' },
        { title: 'Team Size', value: 'team_size' },
        { title: 'Skills', value: 'skills'}
        
      ],
      bctitems: [
        {
          role: 'DBA',
          projects: 'ATC',
          team_size: '5 [24*5]',
          skills: 'Oracle 12c, SQL Server, PowerShell'
          
        },
        {
          role: 'DevOps',
          projects: 'Internal',
          team_size: '2 [24*5]',
          skills: 'Ansible, docker, jenkins, docker-compose, git'
          
        },
      ],
      boschheaders: [
        { title: 'Role', value: 'role' },
        { title: 'Projects', value: 'projects' },
        { title: 'Team Size', value: 'team_size' },
        { title: 'Skills', value: 'skills'}
        
      ],
      boschitems: [
        {
          role: 'DevOps',
          projects: 'JMaaS',
          team_size: '5 [24*5]',
          
        },
        {
          role: 'DevOps',
          projects: 'XaaS',
          team_size: '2 [24*5]',
          
        },
        {
          role: 'Cloud',
          projects: 'BIaaS',
          team_size: '5 [24*5]',
          
        },
      ],

      amdheaders: [
        { title: 'Role', value: 'role' },
        { title: 'Projects', value: 'projects' },
        { title: 'Team Size', value: 'team_size' },
        { title: 'Skills', value: 'skills'}
        
      ],
      amditems: [
        {
          role: 'Cloud/SRE',
          projects: 'DevCloud',
          team_size: '5 [24*5]',
          
        },
        {
          role: 'DevOps',
          projects: 'xTrack360',
          team_size: '1 [24*5]',
          
        },
        {
          role: 'AI',
          projects: 'Internal',
          team_size: '1 [24*5]',
          
        },
      ],

    };
  },
}
</script>

<style>
td,
th {
  text-align: left;
}
</style>