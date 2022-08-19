<template>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.2/css/all.min.css" integrity="sha512-1sCRPdkRXhBV2PBLUdRb4tMg1w2YPf37qatUFeS7zlBy7jJI8Lf4VHwWfZZfpXtYSLy85pkm9GaYVYMfw5BC1A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<div class="Dashboard">
  <main-section></main-section>
  <header-section></header-section>
  <sidebar-section></sidebar-section>
  <footer-section></footer-section>
</div>

</template>

<script>
import MainSection from './components/MainSection';
import HeaderSection from './components/HeaderSection';
import SidebarSection from './components/SidebarSection';
import FooterSection from './components/FooterSection';


export default {
  name: 'App',
  components: {
    MainSection,
    HeaderSection,
    SidebarSection,
    FooterSection,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  top: 0px;
}

.Dashboard {
  box-sizing: border-box ;
  display: grid;
  height: 100%;
  margin: -8px; /* Permet d'afficher les éléments sur l'ensemble de la page*/
  padding-right: 30px;
  grid-template-rows: 1fr 4fr 2fr;
  grid-template-columns: 1fr 2fr 1fr;
  grid-template-areas: 
  "Sidebar Header Header"
  "Sidebar Main Main"
  "Sidebar Footer Footer";
}

.Main {
  grid-area: Main;
  background: #ebedef;
}

.Sidebar {
  grid-area: Sidebar;
  background: #303c54;
  color: #9ea6b2;
}

.Header {
  grid-area: Header;
}

.Footer {
  grid-area: Footer;
  background: #ebedef;
}
</style>
