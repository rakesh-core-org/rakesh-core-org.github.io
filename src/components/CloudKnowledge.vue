<template>
    <div>
        <v-row no-gutters>
            <v-col cols="1">
                <v-img :width="30" :height="30" :src="imageSrc" alt="devops logo"></v-img>
            </v-col>
            <v-col cols="5" >
                <h2>Cloud</h2>
            </v-col>
        </v-row>

        <ul>
            <li>Deployed OpenStack Zed version from scratch using OpenStack-Ansible.
            </li>
            <li>Customized images using OpenStack Disk Image Builder (DIB) and developed custom DIB elements.
            </li>

            <li>Extended OpenStack Ironic inspection package to retrieve GPU details.
            </li>
            <li>Managed the enrollment of OpenStack Ironic metal nodes.
            </li>
            <li>Handled various OpenStack services, including Nova, Ironic, Neutron, Glance, Keystone, Placement, and Horizon.
            </li>
            <li>Experience in handling <font color="red">ceph</font> cluster for storage (Blob and object store)</li>

            <li>Experience in configuring cisco and arista network switch for DMZ location</li>
            <li>Deployed virtual machines and VM scale sets with auto scale-up and scale-down capabilities.</li>
            <li>Designed Network Security Groups to manage inbound and outbound network access.</li>
            <li>Created resource groups, virtual networks, and subnets.</li>
            <li>Worked with Azure storage accounts, including blobs and disks.</li>

            <li>Experienced in app service/container service and hosting public web applications.</li>
            <li>Utilized Azure Container Registry for container management.</li>
            <li>Worked with Azure Cloud Shell and Azure CLI</li>
            <li>Integrated Azure storage with Django for file uploads.</li>
            <li>Created new DNS records for custom applications</li>
            <li>Experienced in using VBMC for simulating virtual machines as metal nodes.</li>
        </ul>
    </div>
</template>

<script>
import imageSrc from '@/assets/technologylogo/openstack.png'

export default {
    name: 'MyComponent',
    data() {
        return {
            imageSrc
        };
    }
}
</script>