
<template>

    <header :class="{'scrolled-nav' : scrollPosition}" >
        
        <nav class="branding">
            LOGO

            <ul v-show="!mobile" class="navigation">
            <li class="link">
                <router-link class="router-link" to="/">Home</router-link>
            </li>
            <li class="link">
                <router-link class="router-link" to="/about">About Me</router-link>
            </li>
            <li class="link">
                <router-link class="router-link" to="/projects">Services</router-link>
            </li>
            <li class="link">
                <router-link class="router-link" to="/contact">Contact</router-link>
            </li>
        </ul>

        </nav>

    

        <div class="icon">
            <img src="/images/menu.png" style="width: 40px; height: 40px;" @click="toggleMobileNav" v-show="mobile"  :class="{'icon-active': mobileNav}">
        </div>

        <transition name="mobileNav">
            <ul v-show="mobileNav" class="dropdown-nav">
                <li class="link">
                    <router-link class="router-link" to="/">Home</router-link>
                </li>
                <li class="link">
                    <router-link class="router-link"  to="/about">About Me</router-link>
                </li>
                <li class="link">
                    <router-link class="router-link"  to="/projects">Services</router-link>
                </li>
                <li class="link">
                    <router-link class="router-link"  to="/contact">Contact</router-link>
                </li>
            </ul>
        </transition>

    </header>
    
</template>
<script >
    export default{
        name: "Navbar",
        data(){
            return{
                scrollPosition: null,
                mobile: null,
                mobileNav: null,
                windowWidth: null
            }
        },
        created(){
            window.addEventListener("resize", this.checkScreen);
            this.checkScreen();
        },
        methods: {
            toggleMobileNav(){
                this.mobileNav = !this.mobileNav;
            },
            checkScreen(){
            this.windowWidth = window.innerWidth;
            if(this.windowWidth <= 750){
                this.mobile = true;
                return;
            }
            this.mobile = false;
            this.mobileNav = false;
            return;
        }
        }
    };
    
</script>
<style>
*{
  padding: 0;
  margin: 0;
}
  header{
    background: rgba(0, 0, 0, .8);
    z-index: 99;
    width: 100%;
    position: fixed;
    transition: .5s ease all;
    color: white;

  }
  nav{
    display: flex;
    flex-direction: row;
    padding: 12px 0;
    transition: 0.5s ease all;
    width: 90%;
    margin: 0 auto;
    @media(min-width: 1140px){
    max-width: 1140px;
  }
  }
  ul, .link .router-link{
      font-weight: 500;
      color: #fff;
      list-style: none;
      text-decoration: none;
    
  }
  li{
    text-transform: uppercase;
    padding: 16px;
    margin-left: 16px;
  }
  .navigation{
    display: flex;
    align-items: center;
    flex: 1;
    justify-content: flex-end;
  }
  .router-link{
    font-size: 14px;
    transition: .5s ease all;
    padding-bottom: 4px;
    border-bottom: 1px solid transparent;
    &:hover{
      color: #00afea;
      border-color: #00afea;
    }
  }
  .icon{
    display: flex;
    align-items: center;
    position: absolute;
    top: 0;
    right: 24px;
    height: 100%;
  }
  .branding{
    display: flex;
    align-items: center;
  }
  .icon-active{
    transform: rotate(180deg);
  }
  .dropdown-nav{
    display: flex;
    flex-direction: column;
    position: fixed;
    width: 100%;
    max-width: 250px;
    height: 100%;
    background: white;
    top: 0;
    left: 0;
    li{
        margin-left: 0;
        .router-link{
            color: black;
        }
    }
  }
</style>