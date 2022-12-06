<template>
<!--
    The header is divided in 2 sections, one above the other, the "header-top" and the "header-bottom"
-->
<header>
    <div class="container-top">
        <!-- Top section -->
        <section class="header-top">
            
            <!-- Logo -->
            <div class="logo">
                <img src="../assets/img/dark-logo.png" alt="">
            </div>
            
            <!-- Nav options -->
            <div class="nav-section">
                <nav>
                    <a href="">Home<i class="fa-solid fa-chevron-down"></i></a> 
                    <a href="">Pages<i class="fa-solid fa-chevron-down"></i></a> 
                    <a href="">Courses<i class="fa-solid fa-chevron-down"></i></a> 
                    <a href="">Features<i class="fa-solid fa-chevron-down"></i></a> 
                    <a href="">Blog<i class="fa-solid fa-chevron-down"></i></a> 
                    <a href="">Shop<i class="fa-solid fa-chevron-down"></i></a> 
                </nav>
                
                <!-- Account -->
                <div class="account">
                    <i class="fa-regular fa-circle-user"></i>
                </div>
                
                <!-- Search bar -->
                <span class="search-section">
                    <input type="text" id="searchbar" placeholder="Search..." />
                    <i class="fa-solid fa-magnifying-glass"></i>
                </span>
            </div>
        </section>
    </div>

    <!-- This div sets the max with -->
    <div class="container-header">
            
        <!-- Bottom section -->
        <section class="header-bottom">
            
            <!-- Quote text -->
            <div class="text-presentation">
                
            </div>
            
            <!-- Big Pic -->
            <div class="big-pic-presentation">
                
            </div>
            
            <!-- Clients Logos -->
            <div class="clinents-logos">
                
            </div>
        </section>

    </div>
</header>
</template>

<script>
export default {
    name: 'HeaderPage',
}
</script>

<style scoped lang="scss">
header{ 
    width: 100%;
}

.container-top {
    width: 100%;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 20px;
    display: flex;
    justify-content: center;
    box-shadow: 0 .1px 15px rgb(197, 196, 196);
    
    .header-top {
        border: 2px solid yellow;
        height: 75px;
        width: 1150px;
        display: flex;
        justify-content: space-between;
        
        .logo {
            height: 75px;
            width: 200px;
            display: flex;
            align-items: center;
        }

        .nav-section {
            border: 2px solid black;
            height: 75px;
            width: 850px;
            display: flex;
            align-items: center;
            justify-content: space-between;

            nav{
                display: flex;
                gap: 1.6rem;

                a {
                    text-decoration: none;
                    font-family: 'Inter', sans-serif;
                    color: #0b0b0b;
                    display: flex;
                    align-items: center;
                    font-stretch: 2px;
    
                    i {
                        margin-left: 7px;
                        font-size: 12px;
                    }
                }
            }

            input {
                padding: 1rem .8rem;
                font-size: 1rem;
                border-radius: 3px;
                 font-family: 'Inter', sans-serif;
                background-color: #F5F5F5;
                border: none;
            }
        }
    }
}

.container-header {
    border: 2px solid black;
    margin: 0 auto;
    margin-top: 75px;
    height: 950px;
    width: 1365px;
    display: flex;
    justify-content: center;
}






</style>