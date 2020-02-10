<template>
  <div>
    <!--헤더-->
    <div style="width:100%; height:156px;" class="border"></div>

    <!--케러셀-->
    <div style="width:100%; height:300px;" class="border">
      <b-carousel
      style="height:100%;"
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
      >
        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/pc_img_1569230790.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/pc_img_1581063837.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/pc_img_1580262479.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/pc_img_1580722950.jpg"></b-carousel-slide>


      </b-carousel>

    </div>

    <!--스와이프js 이 상품 어때요-->
    <div style="width:100%; height:auto;">
      <h4 class="h4_title">
        이 상품 어때요?
      </h4>
      <swiper :options="swiperOption" style="height:100%;">
          <!-- slides -->
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1579768407245l0.jpg"
                class="slide_img mb-2"
            />
            <div class="swipe_txt_div">
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
            </div>

          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1530173860335l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1573625779529l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/152836638432l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580718086498l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1555383371707l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/156982370323l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>

          <!-- 슬라이더 네비게이션
          <div class="swiper-pagination"  slot="pagination"></div>
           -->
        </swiper>
    </div>

    <!-- 일일 특가 -->
    <div style="width:100%; height:auto;" >
      <div style="height: auto; margin-top:80px; margin-bottom:80px; margin-left:0; width:100%; padding:4%; ">
        <div class="mb-2">
          <h1 style="color:#faa536; font-size:18px; font-weight:bold; margin-bottom: 0px;">바이딜 특가</h1>
          <span style="color:#999; font-size:14px; ">오직 바이딜에서만 만나볼 수 있는 특가!</span>
        </div>
        
        <div>
            <div style="width:100%; ">
              <a href="http://dev.buymall.dubu4.com:3000/store/product/391">
                  <img src="https://i.ibb.co/yh8Pf9F/mask.png" style="width:100%; height:auto; max-height:500px;"></img>
              </a>
              <div class="pl-1 pt-2">
                <div style="font-size:17px;">
                  <a href="http://dev.buymall.dubu4.com:3000/store/product/391" style="color:black; display:block; font-weight:bold; font-size:15px;">
                      이하니 마스크
                  </a>
                
                  <!--<span style="color:#ccc; font-size:15px; position:relative; top:-5px;">피부를 깨우는 깊고 진한 빛, 엘리닉</span>-->
                </div>
                <div style="font-weight:bold; position:relative; top:-5px;" class="mt-1">
                  <span style="font-size:18px; color:#faa536;">35%</span>
                  <span class="pl-1 pr-1" style="font-size:18px;">990,000원</span> 
                  <span style="text-decoration:line-through; font-size:13px; font-weight:normal; color:#ccc;">1,510,000원</span>
                    
                </div>
              </div> 
            </div>
        </div>
        
      </div>
    </div>

    <!--스와이프js 알뜰상품-->
    <div style="width:100%; height:auto;">
      <h4 class="h4_title">
        이 상품 어때요?
      </h4>
      <swiper :options="swiperOption" style="height:100%;">
          <!-- slides -->
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1581035849947l0.jpg"
                class="slide_img mb-2"
            />
            <div class="swipe_txt_div">
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
            </div>

          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1463383662742l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1551770890894l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/152836638432l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580718086498l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1555383371707l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/156982370323l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>

          <!-- 슬라이더 네비게이션
          <div class="swiper-pagination"  slot="pagination"></div>
           -->
        </swiper>
    </div>

    <!--카테고리 + 스와이프-->
    <div style="height:850px; width:100%;" class="border"></div>

    <!--친구초대 배너-->
    <div style="height:140px; width:100%; background-color: rgb(230, 237, 242);">
      
    </div>

    <!--스와이프js 오늘의 신상품-->
    <div style="width:100%; height:auto;">
      <h4 class="h4_title">
        이 상품 어때요?
      </h4>
      <swiper :options="swiperOption" style="height:100%;">
          <!-- slides -->
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1475633955339l0.jpg"
                class="slide_img mb-2"
            />
            <div class="swipe_txt_div">
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
            </div>

          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1535621135770l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1546926213189l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1564985588431l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580718086498l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1555383371707l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/156982370323l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>

          <!-- 슬라이더 네비게이션
          <div class="swiper-pagination"  slot="pagination"></div>
           -->
        </swiper>
    </div>

    <!--스와이프js 간편한 아침식사-->
    <div style="width:100%; height:auto;" class="mb-5">
      <h4 class="h4_title">
        이 상품 어때요?
      </h4>
      <swiper :options="swiperOption" style="height:100%;">
          <!-- slides -->
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1577944920407l0.jpg"
                class="slide_img mb-2"
            />
            <div class="swipe_txt_div">
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
            </div>

          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1571376859614l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1578034910943l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/152836638432l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580718086498l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/1555383371707l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>
          <swiper-slide class="slide_div">
            <img src="https://img-cf.kurly.com/shop/data/goods/156982370323l0.jpg"
                class="slide_img mb-2"
            />
            <div>
              <span class="d-block" style="width:80%; font-weight:500;">발렌타인데이 카드 7종</span>
              <span class="d-block" style="width:80%; font-weight:600;">5,600원</span>
              <span class="d-block" style="color:#aaa; width:80%; text-decoration:line-through;">7000원</span>
              
            </div>
          </swiper-slide>

          <!-- 슬라이더 네비게이션
          <div class="swiper-pagination"  slot="pagination"></div>
           -->
        </swiper>
    </div>

    <div>
      <img src="http://img-cf.kurly.com/shop/data/main/15/pc_img_1568875999.png" style="width:100%;">
    </div>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  data () {
    return {
      swiperOption: {
        // swiper 옵션, 콜백함수 모두 동일하게 사용
        slidesPerView: 4,
      spaceBetween: 30,
      freeMode: true,
      }
    }
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.swiper
    }
  },
  mounted() {
    // 현재 swiper 인스턴스를 확인
    console.log('this is current swiper instance object', this.swiper)
    this.swiper.slideTo(3, 1000, false)
  },
  methods: {
    onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
@import url('https://fonts.googleapis.com/css?family=Gothic+A1:500,600&display=swap');
  .slide_div{
    width:38% !important;
    height: auto;
    margin-right: 15px !important;
  }
  .slide_div:nth-child(1) {
    margin-left: 5% !important;
  }
  .slide_img{
    width:100%;
    height: auto;
  }
  .swipe_txt_div{
    height: 120px;
  }
  .h4_title{
    text-align: center;
    padding-top: 80px;
    padding-bottom: 35px;
    font-family: 'Gothic A1', sans-serif;
    font-size:28px;
    font-weight: 500;
  }

  .carousel-inner{
    height: 100% !important;
  }
  .img-fluid{
    height: 100% !important;
    object-fit: cover;
  }
</style>
