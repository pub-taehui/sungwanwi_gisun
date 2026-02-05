# sungwanwi_gisun
지선이

$(window).resize(function(){
	responsiveSize();
});

$(window).on('load', function(){
	responsiveSize();
})

/*Resposive*/
function responsiveSize(){
	windowWidth = $(window).width();
	windowHeight = $(window).height();

	if($(".mainPop").length > 0){
		if($(".mainPop").css("display") == "block"){
			$("#overlay").show();
		}
		setTimeout(function(){
			$(".mainPop").each(function(){
				var mainPopWeight = $(this).width();
				var mainPopW = ($(window).width() - $(this).width()) / 2;
				var mainPopH = ($(window).height() - $(this).height()) / 2;
				
				//좌측상단으로 이동
				mainPopW = 10;
				mainPopH = 28;

				$(this).css("left",mainPopW);
				$(this).css("top",mainPopH-18);
				
				$(this).find(".btnClose").click(function(){
					$(this).parents(".mainPop").hide();
					$('body').css("overflow", "auto");
					if($(".mainPop").css("display") == "none"){
						$("#overlay").hide();
					}
				});
/*				$(this).find(".btnCloseDay").click(function(){
					$(this).parents(".mainPop").hide();
					$('body').css("overflow", "auto");
					if($(".mainPop").css("display") == "none"){
						$("#overlay").hide();
						$("#overlay").css("z-index","10");
					}
				});*/
				$("#overlay").click(function(){
					$(".mainPop").hide();
					$('body').css("overflow", "auto");
					if($(".mainPop").css("display") == "none"){
						$("#overlay").hide();
					}
				});
			});

		},100);
	}
	
	//재보궐 퀵메뉴 2025
	if(windowWidth < 1520) {
		$(".btn_right_quick_wrap").show().addClass("active");
		$(".btn_right_quick").text("자주찾는 메뉴 열기");
		$(".rquick_list .btn_rquick > a").attr("tabindex",-1);
		if(windowWidth < 1024){
			$(".btn_right_quick_wrap").hide();
		}
	} else {
		$(".btn_right_quick_wrap").hide().removeClass("active");
		$(".btn_right_quick").text("자주찾는 메뉴 닫기");
		$(".right_quick_wrap").css("top","50%");
		$(".rquick_list .btn_rquick > a").removeAttr("tabindex");
	}
	
}

// iframe onload일 때 조회수 증가
function iframeViews() {
	// 조회수 증가
	var mlIdx = $("#mlIdx").val();
	
	$.ajax({
		type: "POST",
		cache: false,
		data: {"mlIdx" : mlIdx},
		url: "/site/ml/MainLayerPopupOpenUpdate.do",
		success: function(data) {
			
		}
	});
}


/* 메인 슬라이더 */
$(document).ready(function(){
const swiper = commonUI.slider('.main_slide_banner_wrap',
	     {
			loop: true,
	         speed:700,
	         slidesPerView: 3,
	         spaceBetween: 25,
	         observer:true,
	         observeParents: true,
	         autoplay: {
	             delay: 3000,
	             disableOnInteraction: false,
	         },
	         pagination: {
	             el: '.main_slide_banner_wrap .slider-page',
	             type: "fraction",
	         },
	         breakpoints: {
	             280: {
	                 slidesPerView: 1,
	                 spaceBetween: 12,
	             },
	             320: {
	                 slidesPerView: 2,
	                 spaceBetween: 12,
	             },
	             768: {
	                 slidesPerView: 2,
	                 spaceBetween: 12,
	             },
	             1024: {
	                 slidesPerView: 3,
	                 spaceBetween: 25,
	             },
	         },
	     });

	     const swiper2 = commonUI.slider('.main_rolling_banner_wrap',
	     {
	    	 loop: false,
	         speed:700,
	         spaceBetween: 6,
	         slidesPerView: 1,
	         centeredSlides: true,
	         observer:true,
	         observeParents: true,
	         autoplay: {
	             delay: 3000,
	             disableOnInteraction: false,
	         },
	         pagination: {
	             el: ".main_rolling_banner_wrap .swiper-pagination",
	             clickable: true,
	         },
	     });

	     const swiperNotice = commonUI.slider(".top_notice_swiper", 
	     {
	         loop: false,
	         loopedSlides: 1,
	         speed: 1500,
	         slidesPerView: 2,
	         observer:true,
	         observeParents: true,
	         autoplay: {
	             delay: 5000,
	             disableOnInteraction: false,
	         },
	         navigation: {
	             nextEl: ".top_notice_swiper .swiper-button-next",
	             prevEl: ".top_notice_swiper .swiper-button-prev",
	         },
	         // Responsive breakpoints
	         breakpoints: {
	             280: {
	                 direction: "vertical",
	                 slidesPerView: 1,
	             },
	             768: {
	                 direction: "vertical",
	                 slidesPerView: 1,
	             },
	             1024: {
	                 direction: "horizontal",
	                 slidesPerView: 2,
	             },
	         },
	     });

	     $(".btn_right_quick").click(function(e){
	    	 e.preventDefault();
	    	 var innerWidth = window.innerWidth;
	    	 var btnRightQuickWrap = $(".btn_right_quick_wrap");
	    	 var rightQuickWrap = $(".right_quick_wrap");
	    	 var btnRightQuick = $(".rquick_list .btn_rquick > a");
	    	 btnRightQuickWrap.toggleClass("active");
	    	 if(btnRightQuickWrap.hasClass("active")) {
	    		 $(this).text("자주찾는 메뉴 열기");
	    		 btnRightQuick.attr("tabindex", -1);
	    		 rightQuickWrap.attr("aria-hidden",true);
	    	 } else {
	    		 $(this).text("자주찾는 메뉴 닫기");
	    		 btnRightQuick.removeAttr("tabindex");
	    		 rightQuickWrap.removeAttr("aria-hidden");
	    	 }
	     });
	     
	     /* 퀵메뉴
	     $(window).resize(function(){
	         var innerWidth = window.innerWidth;
	         //console.log(innerWidth);
	         if(innerWidth <= 1440) {
	             $(".right_quick_wrap").hide();
	             $(".sns_menu").fadeOut();
	         } else if(innerWidth > 1440){
	             $(".right_quick_wrap").show();
	             $(".sns_menu").fadeIn();
	         }
	     }); */
	     
	     $(".top_notice_swiper .btn-close, .top_notice_close").click(function(e){
	    	 e.preventDefault();
	    	 var top_wrap = $(".top_notice_wrap");
	    	 top_wrap.toggleClass("active");
	    	 if(top_wrap.hasClass("active")) {
	    		 $(this).children(".btn_text").text("알림창닫기");
	    		 $(".top_notice_wrap .top_notice_inner").slideDown(200);
	    		 $(".gnb_bg").css("top","190px");
	    	 } else {
	    		 $(this).children(".btn_text").text("알림창열기");
	    		 $(".top_notice_wrap .top_notice_inner").slideUp(200);
	    		 $(".gnb_bg").css("top","152px");
	    	 }
	     });
});

	    
