<template>
    <div class="content">
        <Menu></Menu>
    <div class="container">
        <div class="row clearfix">
            <div class="col-md-12">
                <div class="search-box-container">
                    <div class="search-box">
                        <input type="text" name="" id="" class="text-search" placeholder="job title, keywords, or company">
                        <input type="button" value="Search" class="btn-search">
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="container">
        <div class="row clearfix">
            <div class="col-md-12">
                <div class="category-set">
                    <div class="category-item">
                        <a href="#">IT-Sware/DB/QA/Web/Graphics/GIS</a>
                    </div>
                     <div class="category-item">
                        <a href="#">IT-HWare/Networks/Systems</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Accounting/Auditing/Finance</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Banking/Insurance</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Sales/Marketing/Merchandising</a>
                    </div>
                     <div class="category-item">
                        <a href="#">HR/Training</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Corporate Management/Analysts</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Office Admin/Secretary/Receptionist</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Civil Eng/Interior Design/Architecture</a>
                    </div>
                     <div class="category-item">
                        <a href="#">IT-Telecoms</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Customer Relations/Public Relations</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Logistics/Warehouse/Transport</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Eng-Mech/Auto/Elec</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Manufacturing/Operations</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Media/Advert/Communication</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Hotels/Restaurants/Food</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Hospitality/Tourism</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Sports/Fitness/Recreation</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Hospital/Nursing/Healthcare</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Legal/Law</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Supervision/Quality Control</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Apparel/Clothing</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Ticketing/Airline/Marine</a>
                    </div>
                     <div class="category-item">
                        <a href="#">Teaching/Academic/Library</a>
                    </div>
                     <div class="category-item all-categories">
                        <a href="#">View all categories</a>
                    </div>
                     
                </div>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
import Menu from './Menu.vue'
export default {
    components:{
        Menu:Menu
    }

}
</script>

<style lang="scss">
.content{
    min-height: 1000px;
}

.search-box-container{
    width: 100%;    margin-top: 20px;
    .search-box{
        width: 100%;
        position: relative;

        .text-search{
            position:absolute;    
            top: 0;
            left: 0;
            width: 100%;        
            padding: 10px 120px 11px 13px;
            font-size: 14px;
            height: 40px;
            border-radius: 4px;
            border:none;
            border:1px solid transparent;
            box-shadow: 0px 0px 6px #d5ddec;
            outline: none;


                &::-webkit-input-placeholder { /* Chrome/Opera/Safari */
                color: #a3afc5;
                }
                &::-moz-placeholder { /* Firefox 19+ */
                color: #a3afc5;
                }
                &:-ms-input-placeholder { /* IE 10+ */
                color: #a3afc5;
                }
                &:-moz-placeholder { /* Firefox 18- */
                color: #a3afc5;
                }
        }

        .btn-search{
            position:absolute;
            top:0;
            right: 0;
            border:none;
            background-color: #ff194e;
            border:1px solid #ff194e;
            color: #ffffff;
            padding: 0 26px;    
            font-size: 14px;
            color: #ffffff;
            height: 40px;
            border-radius: 0 4px 4px 0;
            cursor: pointer;
            outline: none;
        }

    }
}

.category-set{
    margin-top:40px;
    text-align: left;
.category-item{
    display: inline-block;   
    display:block;
    float: left;
    width: 20%;
    a{
        display:block;
        color: #365669;
    background-color: #fff;
    border-radius: 10px;    
        font-size: 10px;
        font-weight: 600;
        line-height: 12px;
        padding: 6px 10px;
    margin: 4px; 
        width: fit-content;

        &:hover{
            text-decoration: none;
            color:#ff194e;
    background: #ffe5ec;
        }
    }
    &.all-categories{
        a{
        background-color: orange;
        color:#fff;
        width: fit-content;
        }
    }
}
}
</style>
