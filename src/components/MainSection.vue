<template>
    <div class="Main">
      <users-section></users-section>
      <income-section></income-section>
      <conversion-rate-section></conversion-rate-section>
      <sessions-section></sessions-section>
      <traffic-section></traffic-section>
    </div>
</template>



<script>
import UsersSection from './MainComponents/UsersSection.vue';
import IncomeSection from './MainComponents/IncomeSection.vue';
import ConversionRateSection from './MainComponents/ConversionRateSection.vue';
import SessionsSection from './MainComponents/SessionsSection.vue';
import TrafficSection from './MainComponents/TrafficSection.vue';

export default {
  name: 'App',
  components: {
    UsersSection,
    IncomeSection,
    ConversionRateSection,
    SessionsSection,
    TrafficSection,
  },
};
</script>


<style scoped>

.Main {
  box-sizing: border-box ;
  height: 100%;
  width: 150wh;
  padding: 1rem 1rem 0 1rem;
  display: grid;
  grid-template-rows: 0.60fr 1.40fr;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 1rem 1rem;
  grid-template-areas: 
  "Users Income ConversionRate Sessions"
  "Traffic Traffic Traffic Traffic";
}


.Users {
  grid-area: Users;
  border-radius: 4px;
}

.Income {
  grid-area: Income;
  border-radius: 4px;
}

.ConversionRate {
  grid-area: ConversionRate;
  border-radius: 4px;
}

.Sessions {
  grid-area: Sessions;
  border-radius: 4px;
}

.Traffic {
  grid-area: Traffic;

}


</style>

