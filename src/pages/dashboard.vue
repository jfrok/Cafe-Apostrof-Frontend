<script setup>
import AnalyticsAward from '@/views/dashboard/AnalyticsAward.vue'
import AnalyticsBarCharts from '@/views/dashboard/AnalyticsBarCharts.vue'
import AnalyticsDepositWithdraw from '@/views/dashboard/AnalyticsDepositWithdraw.vue'
import AnalyticsSalesByCountries from '@/views/dashboard/AnalyticsSalesByCountries.vue'
import AnalyticsTotalEarning from '@/views/dashboard/AnalyticsTotalEarning.vue'
import AnalyticsTotalProfitLineCharts from '@/views/dashboard/AnalyticsTotalProfitLineCharts.vue'
import AnalyticsTransactions from '@/views/dashboard/AnalyticsTransactions.vue'
import AnalyticsUserTable from '@/views/dashboard/AnalyticsUserTable.vue'
import AnalyticsWeeklyOverview from '@/views/dashboard/AnalyticsWeeklyOverview.vue'
import CardStatisticsVertical from '@core/components/cards/CardStatisticsVertical.vue'

const totalProfit = {
  title: 'Total Profit',
  color: 'secondary',
  icon: 'ri-pie-chart-2-line',
  stats: '$25.6k',
  change: 42,
  subtitle: 'Weekly Project',
}

const newProject = {
  title: 'New Project',
  color: 'primary',
  icon: 'ri-file-word-2-line',
  stats: '862',
  change: -18,
  subtitle: 'Yearly Project',
}
</script>

<template>
  <VRow class="match-height">
    <VCol
      sm="6"
      cols="12"
    >
      <v-card class="card" elevation="0">
        <div class="d-flex flex-column align-center ga-10">
          <header>
            <div class="head-title">
              <h1 class="h1 text-blue-cool-600">campaigns started today</h1>
              <span>5</span>
            </div>

          </header>
          <div class="campaigns">
<!--            <campaignStyle v-for="c in 5 " :key="c" name="Competition Worldwide" creater="CriticalCritics"-->
<!--                           platform="tiktok" status="Active" />-->
          </div>
        </div>
      </v-card>
    </VCol>
<!--    <VCol-->
<!--      cols="12"-->
<!--      md="4"-->
<!--    >-->
<!--      <AnalyticsAward />-->
<!--    </VCol>-->

<!--    <VCol-->
<!--      cols="12"-->
<!--      md="8"-->
<!--    >-->
<!--      <AnalyticsTransactions />-->
<!--    </VCol>-->

    <VCol
      cols="12"
      md="4"
    >
      <AnalyticsWeeklyOverview />
    </VCol>

    <VCol
      cols="12"
      md="4"
    >
      <AnalyticsTotalEarning />
    </VCol>

<!--    <VCol-->
<!--      cols="12"-->
<!--      md="4"-->
<!--    >-->
<!--      <VRow class="match-height">-->
<!--&lt;!&ndash;        <VCol&ndash;&gt;-->
<!--&lt;!&ndash;          cols="12"&ndash;&gt;-->
<!--&lt;!&ndash;          sm="6"&ndash;&gt;-->
<!--&lt;!&ndash;        >&ndash;&gt;-->
<!--&lt;!&ndash;          <AnalyticsTotalProfitLineCharts />&ndash;&gt;-->
<!--&lt;!&ndash;        </VCol>&ndash;&gt;-->

<!--&lt;!&ndash;        <VCol&ndash;&gt;-->
<!--&lt;!&ndash;          cols="12"&ndash;&gt;-->
<!--&lt;!&ndash;          sm="6"&ndash;&gt;-->
<!--&lt;!&ndash;        >&ndash;&gt;-->
<!--&lt;!&ndash;          <CardStatisticsVertical v-bind="totalProfit" />&ndash;&gt;-->
<!--&lt;!&ndash;        </VCol>&ndash;&gt;-->

<!--&lt;!&ndash;        <VCol&ndash;&gt;-->
<!--&lt;!&ndash;          cols="12"&ndash;&gt;-->
<!--&lt;!&ndash;          sm="6"&ndash;&gt;-->
<!--&lt;!&ndash;        >&ndash;&gt;-->
<!--&lt;!&ndash;          <CardStatisticsVertical v-bind="newProject" />&ndash;&gt;-->
<!--&lt;!&ndash;        </VCol>&ndash;&gt;-->

<!--        <VCol-->
<!--          cols="12"-->
<!--          sm="6"-->
<!--        >-->
<!--          <AnalyticsBarCharts />-->
<!--        </VCol>-->
<!--      </VRow>-->
<!--    </VCol>-->

<!--    <VCol-->
<!--      cols="12"-->
<!--      md="4"-->
<!--    >-->
<!--      <AnalyticsSalesByCountries />-->
<!--    </VCol>-->

<!--    <VCol-->
<!--      cols="12"-->
<!--      md="8"-->
<!--    >-->
<!--      <AnalyticsDepositWithdraw />-->
<!--    </VCol>-->

    <VCol cols="12">
      <AnalyticsUserTable />
    </VCol>
  </VRow>
</template>
