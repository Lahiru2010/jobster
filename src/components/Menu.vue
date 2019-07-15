<template>
    <div class="main-menu">
        <div>
  <b-navbar toggleable="lg"  variant="info">
    <b-navbar-brand href="#" class="logo-img">
        <img src="../assets/logo.svg" alt="">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="menu-items">
        <b-nav-item href="#"><span class="icon briefcase"></span><span class="nav-label">Find a job</span></b-nav-item>
        <b-nav-item href="#"><span class="icon manager"></span><span class="nav-label">For employers</span></b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto right-menu">


      <b-nav-item href="#" class="highlight">Post job free</b-nav-item>
      <b-nav-item href="#" class="nav-btn">Sign in</b-nav-item>

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
@import "../scss/custom.scss";
.main-menu{
  
    font-size: 14px;
    font-weight: 600;

.navbar-nav{
  .nav-item{
    
    line-height: 18px;
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
        line-height: 40px;
    color:$font-color;}
    }

    &.highlight{

    a{
          color: #ffffff;
    background-color: #00639f;
    border-radius: 22px;
    padding: 0 10px;
    padding: 4px 14px 5px 14px;
    color: #ffffff;
    margin-right: 6px;
    color: #ffffff;
    }
    }

    &.nav-btn{
      padding: 4px 0 5px 0;
    }
  }
  &.menu-items{
    margin-left: 20px;
  }
&.right-menu{
  margin-right: 16px;
}
  
}
.navbar-toggler{
    border:none;
    outline: none;
    padding: 5px 8px;
    border: 1px solid #ffaabe;
    margin-right: 16px;
    
      border-color: #ffaabe !important;
    .navbar-toggler-icon{
      background-image: url('../assets/icon-navbar-toggle.svg');
      background-repeat: no-repeat;
    background-size: initial;
    }

    &:hover{
    background-color: #fff2f5;
      border-color: #ffaabe;;
    }
  }
@media screen and (max-width: 991px) {

  .navbar-collapse{
        border-top: 1px solid #d5ddec;
    margin-top: 10px;
    
    padding: 10px;

    .navbar-nav.menu-items{
      margin-left: 0;

      .nav-item{
        
        padding: 5px 0;
        a{    display: block;
    clear: both;
    content: ""; overflow: auto;
    padding: 0;
        }

        
      }
    }

    .navbar-nav.right-menu{
      
      .nav-item{
        
    padding: 16px 0;


a{
  
        color: $font-color;
}
    &.highlight{

    a{
        background-color: transparent;
        color: $font-color;
        padding:0px 10px;;
    }
    }

      }

    }
  } 
}
}
</style>
