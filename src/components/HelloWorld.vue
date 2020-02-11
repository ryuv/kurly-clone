<template>
  <div style="width:100%;">
    <!--헤더-->
    <div style="width:100%; height:156px;" class="border"></div>

    <!--데스크톱 케러셀-->
    <div class="desktop_banner" style="width:100%; height:300px;">
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

    <!--모바일 케러셀-->
    <div class="mobile_banner" style="width:100%;">
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
        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/mobile_img_1580465698.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/mobile_img_1581063837.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/mobile_img_1581302984.jpg"></b-carousel-slide>

        <b-carousel-slide style="height:100%;" img-src="https://img-cf.kurly.com/shop/data/main/1/mobile_img_1569230790.jpg"></b-carousel-slide>


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
    <div style="width:100%; height:auto;" class="mt-5">
      <div class="row buydeal" style="height: auto; width:100%; margin:0 !important; ">
        <div class="buydeal-text col-xs-12 col-sm-4 col-md-4 col-lg-4 mb-2">
          <h1 style="color:#faa536; font-size:18px; font-weight:bold; margin-bottom: 0px;">바이딜 특가</h1>
          <span style="color:#999; font-size:14px; ">오직 바이딜에서만 만나볼 수 있는 특가!</span>
        </div>
        
        <div class="col-xs-12 col-sm-8 col-md-8 col-lg-8">
            <div style="width:100%;">
              <a href="http://dev.buymall.dubu4.com:3000/store/product/391">
                  <img src="https://img-cf.kurly.com/shop/data/goods/1580806698409z0.jpg" style="width:100%; height:auto;"></img>
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
    <div style="width:100%; height:auto;" class="mb-5">
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
    <div class="category_swipe" style="height:auto; width:100%;">
      <h4 class="h4_title">
        MD의 추천
      </h4>
      <swiper :options="TextSwiperOption" class="txt_swiper" style="height:auto; border-top:1px solid #f7f7f7; border-bottom:1px solid #f7f7f7;" >
        <swiper-slide class="Text_swiper_slide swiper_active_custom" style="margin-left:4%;">
          <span class="swiper_span swiper_span_active_custom">
            채소
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
             과일·견과·쌀 
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            수산·해산·건어물
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            정육·계란
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            국·반찬·메인요리
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            샐러드·간편식
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            면·양념·오일
          </span>
        </swiper-slide>
        <swiper-slide class="Text_swiper_slide">
          <span class="swiper_span">
            음료·우유·떡·간식
          </span>
        </swiper-slide>
      </swiper>
      <div class="mt-3" style="width:100%;height:auto;">
        <div class="text-center d-flex row" style="margin:0 !important;">
          <div class="d-inline-block col-4" style="">
            <img src="https://img-cf.kurly.com/shop/data/goods/1532654724641l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">깐대파 500g</span><br>
              <span style="font-weight:600;">2,900원</span>
            </div>
            <span></span>
          </div>
          <div class="d-inline-block col-4" >
            <img src="https://img-cf.kurly.com/shop/data/goods/1535438202749l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">흙생강 100g</span><br>
              <span style="font-weight:600;">1,800원</span>
            </div>
            <span></span>
          </div>
          <div class="d-inline-block col-4" >
            <img src="https://img-cf.kurly.com/shop/data/goods/157655557851l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">깐도라지 100g</span><br>
              <span style="font-weight:600;">2,800원</span>
            </div>
            <span></span>
          </div>
        </div>
        <div class="text-center d-flex row" style="margin:0 !important;">
          <div class="d-inline-block col-4">
            <img src="https://img-cf.kurly.com/shop/data/goods/1542003260105l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">GAP 밀양 깻잎 3속</span><br>
              <span style="font-weight:600;">1,120원</span>
            </div>
            <span></span>
          </div>
          <div class="d-inline-block col-4">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580708666582l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">GAP 밀양 깻잎 3속</span><br>
              <span style="font-weight:600;">1,120원</span>
            </div>
            <span></span>
          </div>
          <div class="d-inline-block col-4">
            <img src="https://img-cf.kurly.com/shop/data/goods/1580447356481l0.jpg" style="width:100%;">
            <div style="height:88px; width:100%; font-size:0.9em; text-align:left;">
              <span class="d-inline-block pt-1">당귀잎 35g</span><br>
              <span style="font-weight:600;">1,850원</span>
            </div>
            <span></span>
          </div>
        </div>
        
      </div>
    </div>

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
        slidesPerView: 3,
      spaceBetween: 30,
      freeMode: true,
      },
      TextSwiperOption: {
        // swiper 옵션, 콜백함수 모두 동일하게 사용
        slidesPerView: 2,
        spaceBetween: 30,
        freeMode: true,
      }
    }
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
    width:25% !important;
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

  .Text_swiper_slide{
    width:auto !important;
    padding-top:6px; 
    padding-bottom:6px;
  }

  .swiper_active_custom{
    border-bottom:2px solid #5f0080;
    font-weight: bold;
  }

  .swiper_span_active_custom{
    color:#5f0080 !important;

  }

  .h4_title{
    text-align: center;
    padding-top: 80px;
    padding-bottom: 35px;
    font-family: 'Gothic A1', sans-serif;
    font-size:28px;
    font-weight: 500;
  }

  @media (max-width: 575px) {
    .h4_title{
      font-size: 18px;
      text-align: left;
      padding-left: 4%;
      padding-bottom: 5px;
      font-weight: bold;
    }

    .slide_div{
      width:38% !important;
    }

    .category_swipe{
      padding:0;
    }

    .txt_swiper{
      width:100% !important;
    }

    .desktop_banner{
      display: none;
    }
    .mobile_banner{
      display: block !important;
    }
  }



  @media (min-width: 768px) {
    .buydeal-text{
      text-align: right;
    }

    .buydeal{
      padding-left: 10%;
      padding-right: 10%;
    }
  }
  @media (min-width: 577px) {
    .carousel-inner{
      height: 100% !important;
    }
  }

  
  .img-fluid{
    height: 100% !important;
    object-fit: cover;
  }

  .swiper_span{
    font-size: 0.8em;
    color:#999;
  }

  .category_swipe{
    padding:4%;
  }
  .txt_swiper{
    width:50%;
  }
  .mobile_banner{
    display: none;
  }
</style>
