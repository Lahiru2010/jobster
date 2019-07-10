<template>
    <div class="main-menu">
        <div>
  <b-navbar toggleable="lg"  variant="info">
    <b-navbar-brand href="#" class="logo-img">
        <img src="../assets/logo.svg" alt="">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="center">
        <b-nav-item href="#"><span class="icon briefcase"></span><span class="nav-label">Find a job</span></b-nav-item>
        <b-nav-item href="#"><span class="icon manager"></span><span class="nav-label">For employers</span></b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">


      <b-nav-item href="#" class="highlight">Post job free</b-nav-item>
      <b-nav-item href="#">Sign in</b-nav-item>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" >
.bg-info{
    background-color: #FFFFFF !important;
}

.navbar-nav{
  .nav-item{
    a{
          padding: 0 10px;
      .icon{
        display: block;
        float: left;
        width: 40px;
        height: 40px;
        &.briefcase{ background-image: url('../assets/icon-find-jobs.svg'); background-repeat: no-repeat; background-position: center;}
        &.manager{background-image: url('../assets/icon-manager.svg'); background-repeat: no-repeat; background-position: center;}
      }
      .nav-label{
        display: block;
        float: left;
        line-height: 40px;}
    }

    &.highlight{
          background-color: #fd3272;
    border-radius: 22px;
    padding: 0 10px;
    padding: 4px 10px 6px 10px;
    color: #ffffff;
    margin-right: 6px;

    a{
      
    color: #ffffff;
    }
    }
  }
  &.center{
    margin:0 auto;
  }
}
</style>
