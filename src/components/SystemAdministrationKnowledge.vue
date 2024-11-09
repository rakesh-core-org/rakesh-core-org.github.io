<template>
    <div>
        <v-row no-gutters>
            <v-col cols="1">
                <v-img :width="40" :height="40" :src="imageSrc" alt="devops logo"></v-img>
            </v-col>
            <v-col cols="9" >
                <h2>System administration and SRE</h2>
            </v-col>
        </v-row>

        <ul>
            
            <li>Proficient in virtualization technology, specifically KVM/QEMU/Libvirt</li>
            <li>Experienced with IPMI/Redfish BMC.</li>
            
            <li>Proficient in configuring and sharing mount points between Windows and Linux systems, and setting up YUM repositories (Local, Satellite, Remote).</li>
            <li>Ansible play-books for server management and Managing the Cluster configuration</li>
            <li>Skilled in deploying security patches and automating YUM configuration and RPM installation using Ansible, reducing 3 hours of manual work.</li>
            <li>Skilled in configuring SSSD for LDAP connectivity on Linux servers, and managing local user creation and testing with OpenLDAP and Keycloak.</li>
            <li>Proficient in monitoring server health and logs using Grafana Loki, and IPMI monitoring using SNMP exporter.</li>
            <li>Supported migration of Openstack ironic servers from one lab to another </li>

        </ul>
    </div>

</template>

<script>
import imageSrc from '@/assets/technologylogo/system.png'

export default {
  name: 'MyComponent',
  data() {
    return {
      imageSrc
    };
  }
}
</script>