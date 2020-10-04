<template>
    <div class="dashboard-content">

        <info-box></info-box>
        <dashboard-chart></dashboard-chart>
        <dashboard-orders></dashboard-orders>
        <dashboard-others></dashboard-others>




    </div>
</template>

<script>
     import Info from '../components/Info.vue';
     import DashboardChart from '../components/DashboardChart.vue';
     import DashboardOrders from '../components/DashboardOrders.vue';
     import DashboardOthers from '../components/DashboardOthers.vue';
    // import Traffic from '../dashboard/Traffic.vue';
    // import TrafficSales from '../dashboard/TrafficSales.vue';
    // import Socials from '../dashboard/Socials.vue';

    export default {
         components: {
                 InfoBox: Info,
                 DashboardChart,
                 DashboardOrders,
                 DashboardOthers,
        //         // SocialNetworks: Socials,
        //         // TrafficChart: Traffic,
        //         // TrafficSales: TrafficSales
         }
    }
</script>

<style>

</style>