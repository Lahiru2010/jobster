<template>
  <div class="content">
    <Menu></Menu>
    <div class="container search">
      <div class="row clearfix">
        <div class="col-md-12">
          <div class="search-box-container clearfix">
            <div class="col-search">
              <div class="search-section">
                <div class="search-description">
                  <div class="tite">Like what you do. Where you do it.</div>
                  <div class="title-bold">And get paid more.</div>
                </div>
                <div class="search-box">
                  <input
                    type="text"
                    name
                    id
                    class="text-search"
                    placeholder="job title, keywords, or company"
                  />
                  <input type="button" value="Search" class="btn-search" />
                </div>
                <div class="post-job">
                  <a href="#">
                    Post a job
                    <span class="icon-arrow"></span>
                  </a>
                </div>
              </div>
            </div>
            <div class="col-details">
              <div class="details-section">
                <div class="resume-description">
                  <div class="title">Make your search easy.</div>
                  <div class="title-bold">Upload Your Resume</div>
                  <div class="sub-title">Don't have a resume? Build one in 3 steps.</div>
                  <div class="resume-submit">
                    <button class="btn-resume">
                      <span class="icon-upload"></span>Upload/Build Resume
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container section">
      <div class="row clearfix">
        <div class="col-md-12">
          <div class="category-section">
            <div class="section-title">Trending Searches</div>
            <div class="section-content">
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
    </div>

    <div class="container section">
      <div class="row">
        <div class="col-md-12">
          <div class="recommended">
            <div class="section-title">
              Recommended jobs
              <div class="list-type">
                <div class="btn-type-tile" v-bind:class="{'active':this.gridTypeList==false}" @click="setTileType()"></div>
                <div class="btn-type-list" v-bind:class="{'active':this.gridTypeList==true}" @click="setListType()"></div>
              </div>
            </div>
            <div class="section-content">
              <div class="rec-set" v-bind:class="{'list':this.gridTypeList==true}">
                <div class="rec-item" v-for="index in 60" v-bind:key="index">
                  <div class="rec-box">
                    <a href="#">
                      <div class="comp-logo">
                        <div class="image">
                          <img src="../assets/company-logo.png" alt />
                        </div>
                      </div>
                      <div class="comp-details clearfix">                          
                        <div class="list-col-left">
                            <div class="company-details">
                        <div class="name">Interaction Designer</div>
                        <div class="company">Salesforce</div>
                        
                        </div>
                        
                        <div class="location">Colombo, Sri Lanka</div>
                        </div>
                        <div class="list-col-right">
                        <div class="ago">
                            <div v-if="gridTypeList==false">1 week ago</div>
                            <div v-if="gridTypeList==true">
                            <div class="posted-date"><span class="ago-label">Posted on</span>21-03-2019</div>
                            <div class="expired-date"><span class="ago-label">Expiry Date</span>21-03-2019</div>
                            </div>
                        </div>
                        </div>
                      </div>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container section post-jobs-container">
      <div class="row">
        <div class="col-md-12">
          <div class="post-jobs clearfix">
            <div class="col-details">
              <div class="details-section">
                <div class="title">Employers</div>
                <div class="sub-title">Looking to Post a Job?</div>
                <div
                  class="desc"
                >We have end-to-end solutions that can keep up with you and your standards.</div>
                <div class="submit-job">
                  <button class="btn-post-job">Post a Job</button>
                </div>
              </div>
            </div>
            <div class="col-image">
              <div class="image-section"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-container">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="logo-row">
              <img src="../assets/logo.svg" alt />
            </div>
            <div class="col-row clearfix">
              <div class="f-col-5">
                <div class="f-col">
                  <div class="col-title">jobbly.lk</div>
                  <div class="nav-list">
                    <a href>About us</a>
                    <a href>Blog</a>
                    <a href>Sitemap</a>
                  </div>
                </div>
              </div>
              <div class="f-col-5">
                <div class="f-col">
                  <div class="col-title">Job Seekers</div>
                  <div class="nav-list">
                    <a href>Browse jobs</a>
                    <a href>Upload resume</a>
                    <a href>Create an account</a>
                  </div>
                </div>
              </div>
              <div class="f-col-5">
                <div class="f-col">
                  <div class="col-title">Employers</div>
                  <div class="nav-list">
                    <a href>Post a job</a>
                    <a href>Search resume</a>
                    <a href>My dashboard</a>
                  </div>
                </div>
              </div>
              <div class="f-col-5">
                <div class="f-col">
                  <div class="col-title">Community</div>
                  <div class="nav-list">
                    <a href>Help/Contact us</a>
                    <a href>Terms of use</a>
                    <a href>Privacy policy</a>
                    <a href>Guidelines</a>
                    <a href>FAQs</a>
                    <a href>Cookie Notice</a>
                  </div>
                </div>
              </div>
              <div class="f-col-5">
                <div class="f-col">
                  <div class="col-title">Work with us</div>
                  <div class="nav-list">
                    <a href>Careers</a>
                    <a href>Advertise</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="rights-row">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="right">© 2019 Jobbly. All rights reserved.</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Menu from "./Menu.vue";
export default {
    data(){
        return{
            gridTypeList:false
        }
    },
  components: {
    Menu: Menu
  },
  methods:{
      setListType:function(){
          this.gridTypeList=true;
      },
      setTileType:function(){
          this.gridTypeList=false;
      }
  }
};
</script>

<style lang="scss">
@import "../scss/custom.scss";
.content {
  min-height: 1000px;
}

.container.section {
  margin: 40px auto;
  .section-title {
    font-size: 16px;
    margin-bottom: 20px;
    color: $font-color;
    font-weight: 600;
    text-align: left;
  }

  .section-content {
    width: 100%;
    margin: 0 -3px;
  }
}
.container.search {
  margin-top: 40px;
  .search-box-container {
    width: 100%;
    // height: 280px;
    background-color: #ffffff;
    border-radius: 6px;

    height: 100%;
    .col-search {
      width: 60%;
      float: left;
      height: 100%;

      .search-section {
        padding: 40px;

        .search-description {
          margin: 10px 0 20px 0;
          color: $font-color;
          .title {
            font-size: 20px;
          }

          .title-bold {
            font-size: 28px;
            font-weight: 600;
          }
        }

        .search-box {
          width: 100%;
          position: relative;
          height: 40px;
          .text-search {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            padding: 10px 120px 11px 13px;
            font-size: 14px;
            height: 40px;
            border-radius: 4px;
            border: none;
            border: 1px solid transparent;
            box-shadow: 0px 0px 6px #d5ddec;
            outline: none;

            &::-webkit-input-placeholder {
              /* Chrome/Opera/Safari */
              color: #a3afc5;
            }
            &::-moz-placeholder {
              /* Firefox 19+ */
              color: #a3afc5;
            }
            &:-ms-input-placeholder {
              /* IE 10+ */
              color: #a3afc5;
            }
            &:-moz-placeholder {
              /* Firefox 18- */
              color: #a3afc5;
            }
          }

          .btn-search {
            position: absolute;
            top: 0;
            right: 0;
            border: none;
            background-color: $secondary-theme-color;
            border: 1px solid $secondary-theme-color;
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
        .post-job {
          margin-top: 20px;
          a {
            text-decoration: none;
            color: $font-color;
            position: relative;
            display: block;
            font-size: 14px;
            font-weight: 600;
            width: fit-content;
            .icon-arrow {
              display: block;
              position: absolute;
              top: 6px;
              right: -16px;
              width: 12px;
              height: 12px;
              background-image: url("../assets/icon-arrow-right.svg");
              background-repeat: no-repeat;
              //   background-size: contain;
              @include transition(right 0.1s ease-in-out);
            }

            &:hover {
              color: $secondary-theme-color;
              .icon-arrow {
                background-position-y: -12px;
                right: -18px;
              }
            }
          }
        }
      }

      @media screen and (max-width: 768px) {
        width: 100%;
        height: auto;
      }
    }
    .col-details {
      width: 40%;
      float: left;
      height: 100%;
      background-color: $secondary-theme-color;
      border-radius: 0 6px 6px 0;
      color: $secondary-font-color;
      .details-section {
        padding: 40px;
        @media only screen and (max-width: 991px) and (min-width: 768px) {
             padding:20px !important;
         }
        

        .resume-description {
          margin: 10px 0 20px 0;
          .title {
            font-size: 16px;
          }
          .title-bold {
            font-size: 22px;
            font-weight: 600;
          }
          .sub-title {
            font-size: 14px;
          }
          .resume-submit {
            margin-top: 20px;
            .btn-resume {
              background-color: #ffffff;
              border: none;
              color: #ff194e;
              padding: 10px 20px;
              border-radius: 6px;
              font-weight: 600;
              font-size: 14px;
              outline: none;
              background-image: linear-gradient(
                to right top,
                #ffffff,
                #fcfcfc,
                #f9f9f9,
                #f7f7f7,
                #f4f4f4
              );
              position: relative;

              padding-left: 42px;

              .icon-upload {
                display: block;
                position: absolute;
                width: 20px;
                height: 20px;
                background-image: url("../assets/icon-upload.svg");
                background-repeat: no-repeat;
                background-size: contain;
                left: 12px;
              }
            }
          }
        }
        
      }
       @media screen and (max-width: 768px) {
        width: 100%;
        height: auto;

        
      border-radius: 0 0 6px 6px;
      }
    }
  }
}

.category-set {
  margin: 0 -4px;
  text-align: left;
  .category-item {
    display: inline-block;
    display: block;
    float: left;
    width: 20%;
      @media only screen and (max-width: 1200px) and (min-width: 991px) {
           
    width: 25%;
         }
    @media only screen and (max-width: 990px) and (min-width: 768px) {
           
    width: 33.33%;
         }
           @media only screen and (max-width: 767px) and (min-width: 342px) {
           
    width: 50%;
         }

    a {
      display: block;
      color: #365669;
      background-color: #fff;
      border-radius: 10px;
      font-size: 11px;
      font-weight: 600;
      line-height: 12px;
      padding: 6px 10px;
      margin: 4px;
      width: fit-content;
      text-overflow: ellipsis;
      overflow: hidden;
      white-space: nowrap;
    border: 1px solid #e4ecfb;
      &:hover {
        text-decoration: none;
        color: $secondary-theme-color;
        background: #ffe5ec;
        border-color: #ffcfdb;
      }
    }
    &.all-categories {
      a {
        background-color: orange;
        color: #fff;
        width: fit-content;
      }
    }
  }
}

.recommended {
  .section-title {
    position: relative;
    .list-type {
      position: absolute;
      top: 0;
      right: 6px;

      .btn-type-tile {
        width: 20px;
        height: 20px;
        background-image: url("../assets/icon-grid-type.png");
        background-position: 0px 0px;
        float: left;
        margin-right: 8px;
        cursor: pointer;
        &:hover,
        &.active {
          background-position: 0px -20px;
        }
      }
      .btn-type-list {
        width: 20px;
        height: 20px;
        background-image: url("../assets/icon-grid-type.svg");
        background-position: 20px 0px;
        float: left;
        cursor: pointer;
        &:hover,
        &.active {
          background-position: -20px -20px;
        }
      }
    }
  }
  .rec-set {
    .rec-item {
      width: 25%;
      float: left;
      .rec-box {
        padding: 3px;
        a {
          display: block;
          width: 100%;
          position: relative;
          padding-left: 70px;
          text-decoration: none;
          background-color: #ffffff;
          border: 1px solid #e4ecfb;
          border-radius: 4px;
          color: inherit;
          text-align: left;
        }
        .comp-logo {
          width: 70px;
          height: 100px;
          position: absolute;
          left: 0;
          .image {
            width: 54px;
            height: 54px;
            background-color: #d6dbe4;
            border-radius: 100px;
            margin: 12px auto;
            img {
              width: 100%;
            }
          }
        }
        .comp-details {
          padding-left: 6px;
          padding-top: 10px;
          .name {
            font-size: 14px;
            font-weight: 600;
            color: $font-color;
          }
          .company {
            font-size: 12px;
            font-weight: 600;
            color: #ff194e;
          }
          .location {
            font-size: 12px;
            color: #b5b5b5;
          }
          .ago {
            font-size: 12px;
            text-align: right;
            padding: 0 10px 10px 0;
            padding-bottom: 10px;
            color: #bfbfbf;
          }
        }
      }
    }

    &.list{
        .rec-item{
      width: 100%;

      .rec-box {
        padding: 3px;
        a {
          display: block;
          width: 100%;
          position: relative;
          padding-left: 60px;
          text-decoration: none;
          background-color: #ffffff;
          border: 1px solid #e4ecfb;
          border-radius: 4px;
          color: inherit;
          text-align: left;
        }
        .comp-logo {
          width: 60px;
          height: 100%;
          position: absolute;
          left: 0;
          .image {
            width: 38px;
            height: 38px;
            background-color: #d6dbe4;
            border-radius: 100px;
            margin: 5px auto;
            img {
              width: 100%;
            }
          }
        }
        .comp-details {
          padding-left: 6px;
          padding-top: 10px;

          .list-col-left{
              width: 50%;
              float: left;
              margin-top: -6px;

              .company-details{
                  width: 70%;
    float: left;
          .name {
            font-size: 12px;
            font-weight: 600;
            color: $font-color;
          }
          .company {
            font-size: 12px;
            font-weight: 600;
            color: #ff194e;
          }}
           .location {
            font-size: 12px;
            color: $font-color;
            float: left;
    margin-top: 10px;
          }
          }
          .list-col-right{
              width: 50%;
              float: left;
         
          .ago {
            font-size: 10px;
            text-align: right;
            padding: 0 10px 10px 0;
            padding-bottom: 10px;
            color: $font-color;

            .ago-label{
                font-weight: 600;
                margin-right: 4px;
            }
          }
          }
        }
      }
      }
    }
  }
}

.post-jobs-container {
  .post-jobs {
    background-color: $font-color;
    border-radius: 6px;
    color: $secondary-font-color;

    height: 100%;
    .col-details {
      width: 70%;
      float: left;
      .details-section {
        // padding: 40px;
        padding: 60px 40px;


        .title {
          font-size: 16px;
          font-weight: 600;
        }
        .sub-title {
          font-size: 26px;
          font-weight: 600;
          color: #00fdff;
        }
        .desc {
          font-size: 14px;
        }
        .submit-job {
          margin-top: 20px;
          .btn-post-job {
            background-color: transparent;
            border: 1px solid #00fdff;
            color: #00fdff;
            padding: 10px 40px;
            border-radius: 4px;
            font-size: 14px;
            outline: none;
          }
        }
      }
    }

    .col-image {
      width: 30%;
      height: 100%;
      float: left;
      background-image: url("../assets/professional2.jpg");
      background-size: cover;
      background-repeat: no-repeat;
      border-radius: 0 6px 6px 0;
    }
  }
}

.footer-container {
  background-color: #fff;
  min-height: 300px;

  .logo-row {
    margin: 40px 0 20px 0;
    img {
      width: 140px;
    }
  }

  .col-row {
    .f-col-5 {
      width: 20%;
      float: left;

      .f-col {
        padding: 10px;

        .col-title {
          font-size: 16px;
          font-weight: 600;
          margin-bottom: 6px;
          color: $font-color;
        }
        .nav-list {
          a {
            display: block;
            color: $font-color;
            font-size: 14px;
            line-height: 26px;
            text-decoration: none;
            @include transition(all 0.1s ease-in-out);

            &:hover {
              color: $secondary-theme-color;
            }
          }
        }
      }

      &:first-child {
        .f-col {
          padding-left: 0px;
        }
      }
    }
  }
}
.rights-row {
  font-size: 12px;
  padding: 20px 0;
  border-top: 1px solid #eceeef;
  color: $font-color;
  margin-top: 40px;
}
</style>
