# sungwanwi_gisun
@charset "UTF-8";

header {
	position: relative;
	z-index: 1;
}
#skipLink a{display:block;position:fixed;top:-999px;padding:8px 0;width:150px;text-align:center;color:#fff;background:#000;z-index:999999}
#skipLink a:focus, #skipLink a:hover, #skipLink a:focus, #skipLink a:active{left:0px;top:0px}
#skipLink dt{position:absolute;height:0;width:0;left:-9999px;overflow:hidden;font-size:0;line-height:0;}

/* S: 재보궐 띠배너 */
.top_banner {
	display: flex;
	width: 100%;
	height: 70px;
	background: #F1F1F1 url("/images/n24/rvt/header/bg_header.png") no-repeat center top / auto 70px;
}
.top_banner .inner {
	position: relative;
	display: flex;
	width: 1330px;
	margin: 0 auto;
	padding: 12px 0 12px 43px;
	justify-content: flex-start;
	align-items: center;
}
.top_banner .inner::before {
	content: '';
	position: absolute;
	top: 9px;
	left: -14px;
	width: 54px;
	height: 54px;
	background: url("/images/n24/rvt/header/bg_logo_vote_mark.png") no-repeat center / auto 54px;
}
.top_banner .banner_logo {
	display: flex;
	justify-content: flex-start;
	margin-right: 60px;
	width: 137px;
	height: 47px;
	background: url("/images/n24/rvt/header/vote_date_2025.png") no-repeat left top / 100% auto;
}
.top_banner .banner_vote_box {
	display: flex;
}
.top_banner .banner_vote .tit {
	display: inline-block;
	padding: 4px 4px 3px;
	margin-right: 8px;
	font-size: 14px;
	border-radius: 5px;
	color: #fff;
	background: #2f3b52;
}
.top_banner .banner_vote+.banner_vote {
	margin-left: 54px;
}
.top_banner .banner_vote_box:nth-child(2) .date {
	font-size: 14px;
}
.top_banner .banner_vote_box:nth-child(2) .date b {
	font-size: 18px;
}
.top_banner .banner_vote .date {
	display: inline-block;
	font-size: 16px;
	font-weight: 700;
	color: #2F3B52;
	letter-spacing: -0.025em;
}
.top_banner .banner_vote .date b {
	font-weight: 800;
	font-size: 22px;
}
.top_banner .banner_text {
	position: absolute;
	top: 50%;
	right: 0;
	transform: translateY(-50%);
	width: 201px;
	height: 37px;
	background: url("/images/n24/rvt/header/img_header_banner_1390.png") no-repeat left top /auto 100%
}
.top_banner .banner_vote {
	position: relative;
}
.top_banner .banner_vote .banner_tooltip {
	display: none;
	z-index: 10;
	position: absolute;
	top: 28px;
	left: 50%;
	transform: translateX(-50%);
	padding: 26px 17px 17px;
	margin-left: -106px;
	width: 252px;
	height: 194px;
}
.top_banner .banner_vote .banner_tooltip::before {
	content: '';
	z-index: -1;
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: url('/images/n24/rvt/header/bg_msgbox.png') no-repeat left top / 100% auto;
}
.top_banner .banner_vote+.banner_vote .banner_tooltip {
	margin-left: -164px;
}
/* 20250304 마우스 오버 삭제 처리 
.top_banner .banner_vote:hover .banner_tooltip{display:block;} */
.top_banner .banner_tooltip .bold_txt {
	position: relative;
	display: flex;
	align-items: center;
	min-height: 24px;
	padding-left: 27px;
	font-size: 14px;
	font-weight: 600;
	color: #181818;
	letter-spacing: -1px;
}
.top_banner .banner_tooltip .bold_txt::before {
	content: '';
	z-index: -1;
	position: absolute;
	top: 1px;
	left: 0;
	width: 24px;
	height: 24px;
	background: url('/images/n24/rvt/header/icon_top_exc.png') no-repeat left top / 100% auto;
}
.top_banner .banner_tooltip .gray_txt {
	display: block;
	margin-top: 10px;
	font-size: 12px;
	font-weight: 300;
	color: #666;
	line-height: 1.25
}
.top_banner .banner_tooltip .gray_txt+.gray_txt {
	margin-top: 4px
}
@media all and (max-width:1024px) {
	.top_banner {
		position: relative;
		width: auto
	}

	.top_banner .date_box_txt {
		display: flex;
		margin-left: 12px;
		align-items: center;
		font-weight: 800;
	}

	.top_banner .date_box_txt .date {
		font-size: 24px;
		font-weight: 400;
		font-family: 'ghanachoco';
	}

	.top_banner .banner_vote+.banner_vote {
		margin-left: 20px;
	}
}
@media all and (max-width:385px) {
	.top_banner .banner_vote .tit {
		margin-bottom: 0px;
	}

	.top_banner .banner_vote .date .mblock {
		display: none;
	}

	.top_banner .inner {
		padding: 10px 10px;
	}
}
@media all and (max-width:285px) {
	.top_banner .banner_vote_box .top_banner .banner_vote .date b {
		font-size: 12px;
	}

	.top_banner .banner_vote .date {
		font-size: 11px;
	}
}
/* E : 재보궐 띠배너 */

.header_wrap {
	height: 84px;
	background-color: #fff;
	border-bottom: 1px solid #DEDEDE;
}
.header_wrap .inner {
	display: flex;
	width: 1330px;
	height: 100%;
	margin: 0 auto;
	justify-content: space-between;
	align-items: center;
}
.header_wrap .logo {
	display: flex;
	align-items: center;
	width: 204px;
	transition: width 0.2s;
	padding: 20px 0px;
}
.header_wrap .logo > a {
	width:100%;
}
.header_wrap .logo img {
	width: 100%;
}
.header_wrap .top_side {
	position: relative;
	display: flex;
	padding: 15px 0;
	align-items: center;
	font-size: 13px;
	font-weight: 700;
	color: #555;
}

.header_wrap .top_side_link:nth-child(1) {
	position: relative;
	display: block;
	padding-right: 20px;
}
.header_wrap .top_side_link:nth-child(1):after {
	position: absolute;
	top: 2px;
	right: 10px;
	content: '';
	display: block;
	width: 1px;
	height: 14px;
	background: #CCC;
}
.header_wrap .top_side_link:nth-child(2) {
	position: relative;
}
.header_wrap .tooltip_btn {
    position: relative;
    width: 20px;
    height: 20px;
    margin-left: 5px;
    background: url("/images/n24/rvt/header/btn_mymenu_icon.png") center no-repeat;
	background-size: contain;
    right: 0px;
    text-indent: -9999px;
}

/* 모바일 메뉴 */
.m_menu {
	display: none;
}
.m_menu.m_on {
    background: url("/images/n21/mavt/m_menu_close.png") center no-repeat;
    background-size: 24px;
}
#gnb.m_on {
    display: block;
	position: absolute;
	top:58px;
	left:0;
	width:100%;
	height: auto;
	background-color: #fff;
	padding:28px 16px;
	box-shadow:0 2px 9px #ccc;
}
#gnb.m_on .depth1 {
	width:100%;
	height:auto;
	flex-direction: column;
}
#gnb.m_on .depth1 .depth1_li {
	width: 100%;
	padding: 0 12px 16px;
	border-bottom: 1px solid #DEDEDE;
	margin-top:22px;
}
#gnb.m_on .depth1 .depth1_li .depth1_li_link {
	justify-content: flex-start;
}

/* 상단공지사항 */
.top_notice_wrap {
	position: relative;
	top: 0;
	left: 0;
	width: 100%;
	background-color: #2F3B52;
}
.top_notice_wrap.close .top_notice_inner {
	height:0;
}
.top_notice_inner {
	position: relative;
	width: 1330px;
	height:38px;
	margin: 0 auto;
	padding: 0 20px;
	overflow: hidden;
}
.top_notice_link {
	position: relative;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	padding: 8px 0;
	height: 100%;
	display: block;
	overflow: hidden;
	height: 36px;
}
.top_notice_link::before {
	content: '';
	position: absolute;
	top: 50%;
	left: 0;
	width: 20px;
	height: 20px;
	border-radius: 100%;
	background: #EEEAE4 url("/images/n24/rvt/header/icon_top_notice.svg") no-repeat center;
	background-size: 100%;
	-webkit-transform: translateY(-50%);
	transform: translateY(-50%);
}
.top_notice_title {
	display: inline-block;
	position: relative;
	padding: 0 20px 0 30px;
	font-size: 14px;
	font-weight: 500;
	color: #fff;
	line-height: 1.35;
	letter-spacing: -0.01em;
	text-align: left;
	max-width: 510px;
	display: block;
	overflow: hidden;
	white-space: nowrap;
	text-overflow: ellipsis;
}
.top_notice_swiper {
	width: calc(100% - 60px);
	overflow: hidden;
}
.top_notice_swiper .swiper-wrapper {
	height: 38px;

}
.top_notice_swiper .swiper-slide {
	display: flex;
	padding: 0 77px 0 15px;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	justify-content: center;
	background-color: transparent;
}
.top_notice_swiper .swiper-slide-active::before {
	content: '';
	position: absolute;
	top: 50%;
	right: -1px;
	-webkit-transform: translateY(-50%);
	transform: translateY(-50%);
	width: 1px;
	height: 50%;
	background: rgba(255, 255, 255, 0.25);
}
.top_notice_swiper .btn-prev,
.top_notice_swiper .btn-next,
.top_notice_swiper .btn-close,
.top_notice_swiper .btn-stop {
	overflow: hidden;
	position: relative;
	left: auto;
	right: auto;
	top: auto;
	-webkit-transform: none;
	transform: none;
	margin: 0;
	width: 20px;
	height: 20px;
	border-radius: 50%;
	margin-left: 4px;
}
.top_notice_swiper .btn-prev {
	background: url("/images/n24/rvt/header/btn_topbnr_prev_pc.png") no-repeat left top/100% auto;
}
.top_notice_swiper .btn-next {
	background: url("/images/n24/rvt/header/btn_topbnr_next_pc.png") no-repeat left top/100% auto;
}
.top_notice_swiper .btn-close {
	display: none;
	background: url("/images/n24/rvt/header/btn_topbnr_close.png") no-repeat left top/100% auto;
}
.top_notice_wrap .swiper-controller {
	z-index: 10;
	position: absolute;
	top: 50%;
	-webkit-transform: translateY(-50%);
	transform: translateY(-50%);
	right: 4px;
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	-webkit-box-orient: horizontal;
	-webkit-box-direction: normal;
	-ms-flex-direction: row;
	flex-direction: row;
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
	-webkit-box-pack: end;
	-ms-flex-pack: end;
	justify-content: flex-end;
	width: 68px;
	height: 20px;
}
.top_notice_swiper .swiper-controller .btn-stop {
	background: url("/images/n24/rvt/header/btn_topbnr_stop.png") no-repeat left center/100% auto;
}
.top_notice_swiper .swiper-controller .btn-stop.active {
	background: url("/images/n24/rvt/header/btn_topbnr_play.png") no-repeat center center/100% auto;
}
.top_notice_close {
	z-index: 2;
	position: absolute;
	top: 50%;
	bottom: auto;
	right: 52px;
	-webkit-transform: translateY(-50%);
	transform: translateY(-50%);
	padding: 0;
	width: 20px;
	height: 20px;
	background: url("/images/n24/rvt/n24/common/btn_topbnr_close_m.png") no-repeat left top/100% auto;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}

@media screen and (min-width: 1024px) {
	.top_notice_close {
		top: auto;
		bottom: -51px;
		right: 0;
		padding: 7px 13px 8px 13px;
		width: auto;
		height: auto;
		border-radius: 0px 0px 0px 10px;
		background: #2F3B52;
	}
}
.top_notice_close .btn_text {
	position: absolute;
	top: 0;
	left: 0;
	font-size: 1px;
}

@media screen and (min-width: 1024px) {
	.top_notice_close .btn_text {
		display: inline-block;
		position: relative;
		padding-right: 27px;
		font-size: 13px;
		font-weight: 500;
		color: #fff;
		line-height: 1;
		letter-spacing: -0.01em;
		white-space: nowrap;
	}

	.top_notice_wrap .top_notice_close .btn_text::before {
		content: '';
		position: absolute;
		top: 0;
		right: 0;
		width: 14px;
		height: 14px;
		background: url("/images/n24/rvt/header/btn_banner_open.png") no-repeat left top/100% auto;
	}
	.top_notice_wrap.active .top_notice_close .btn_text::before {
		background: url("/images/n24/rvt/header/bg_banner_close.png") no-repeat left top/100% auto;
	}

	.wrap.is-pull-up .top_notice_close .btn_text::before {
		background: url("/images/n24/rvt/n24/common/btn_banner_open.png") no-repeat left top/100% auto;
	}
}

/******************** GNB ********************/
#gnb {
	position: relative;
	height: 84px;
	flex: 1 0;
	padding: 0px 90px;
	transition: padding 0.3s;
}

#gnb .depth1 {
	display: flex;
	height: 100%;
	justify-content: space-between;
}

#gnb .depth1_li {
	position: relative;
	display: flex;
	width: 100px;
	height: 100%;
	transition: width 0.3s;
	padding: 30px 0;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center;
	box-sizing: border-box;	
}

#gnb .depth1_li:first-child {
	
}

#gnb .depth1_li:nth-child(3) .depth2.active {
	width: 160px;
}

#gnb .depth1_li:nth-child(4) {
	width: 180px;
}

#gnb .depth1_li_link {
	display: flex;
	justify-content: center;
	width: 100%;
	color: #333;
	font-size: 18px;
	text-align: center;
	font-weight: 700;
}

#gnb .depth1_li .depth2:before {
	content: '';
	display: block;
	position: absolute;
	top: 0px;
	left: 50%;
	width: 0%;
	height: 2px;
	background: #66558A;
	transition: 2s;
	z-index: 0;
}

#gnb .depth1_li:last-child .depth2 {
	border-right: 1px solid #f5f5f5;
}

#gnb .depth2 {
	display: none;
	position: absolute;
	top: 83px;
	z-index: 10;
	width: 100%;
	height: 122px;
	padding: 35px 0 40px;
	min-height: 122px;
	/*border-left: 1px solid #F5F5F5;*/
}

#gnb .depth2_li {
	display: flex;
	align-items: center;
	margin-bottom: 15px;
	letter-spacing: -1px;
}

#gnb .depth2_li:last-child {
	margin-bottom: 0px;
}

#gnb .depth2_li_link {
	position: relative;
	display: block;
	margin: 0 auto;
	font-size: 16px;
	font-weight:500;
	z-index: 100;
}

#gnb .depth2_li_link:after {
	position: absolute;
	display: block;
	content: '';
	width: 0%;
	height: 9px;
	left: -2px;
	bottom: -1px;
	transition: width 0.2s;
	background: #DAD8F2;
	z-index: 1;
}

#gnb .depth2_li_txt {
	position: relative;
	z-index: 900;
}
.gnb_bg {
	display: none;
	position: absolute;
	z-index: 9;
	width: 100%;
	height: 122px;
	background: #fff;
	border-top: 1px solid #F5F5F5;
	box-shadow: 0px 4px 10px 0px rgba(0, 0, 0, 0.10);
	top:190px;
}
.rvt_sub_area .gnb_bg{
	top:152px;
}
.gnb_bg.gnb_search_rvt {
	top:82px;
}
.gnb_bg.active {
	display: block;
}
.gnb_bg.mymenu_active {
	display: block;
	top: 0px;
	width: 100%;
	height: 100%;
	opacity: 0.8;
	z-index: 998;
	background: #000;
}
.gnb_bg.tooltip_active {
	display: block;
	top: 0px !important;
	width: 100%;
	height: 100%;
	opacity: 0.6;
	z-index: 999;
	background: #000;
}

@media all and (min-width: 1024px) {
	/*header.active .header_wrap .logo {
		width: 180px;
	}
	header.active .header_wrap .logo img {
		width: 180px;
	}
	
	header.active #gnb {
		padding: 0 60px;
	}*/
	#gnb .depth1_li:hover .depth1_li_link,
	#gnb .depth1_li:focus .depth1_li_link {
		color: #66558A;
	}
	#gnb .depth1_li:hover .depth2:before,
	#gnb .depth1_li:focus .depth2:before {
		content: '';
		display: block;
		width: 100%;
		left: 0px;
	}

	#gnb .depth2.active {
		display: block;
	}

	#gnb .depth2:hover {
		background: #FCF8FE;
	}

	#gnb .depth2_li:hover .depth2_li_link:after {
		width: 105%;
		transition: 0.2s;
	}

	.gnb_bg.active {
		display: block;
	}

}
/* E: GNB */

/* 나만의 메뉴 */
.tooltip{display:none;border:solid 1px #009fa1;border-radius:20px;position:absolute;top:52px;right:0;width:420px;line-height:24px;background:#fff url("/images/n21/rvt/tooltip_bg.png") 25px 6% no-repeat;z-index:11;box-shadow:4px 4px 0 rgba(0,0,0,.3);}
.tooltip:before{display:block;content:'';position:absolute;top:-13px;right:26px;width:22px;height:13px;background:url("/images/n21/rvt/tooltip_point_bg.png") 50% 50% no-repeat;}
.tooltip>div{position:relative;text-align:left;}
.tooltip .upper{padding:30px 0 0 140px;height:160px;}
.tooltip .lower{background:#f2f2f2;padding:25px 30px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;}
.tooltip .lower dl{margin-bottom:25px;}
.tooltip .lower dt.title{font-size:18px;font-weight:bold;}
.tooltip .lower ul li{position:relative;font-size:14px;padding-left:10px;}
.tooltip .lower ul li:first-child{margin-bottom:10px;}
.tooltip .lower ul li:before{display:block;content:"*";position:absolute;left:0;top:0;color:#009fa1;}
.tooltip>div em{display:inline-block;font-size:22px;color:#333;line-height:30px;margin-bottom:5px;}
.tooltip>div b{font-weight:800;color:#333;}
.tooltip>div span{display:block;font-size:16px;color:#333;}

.tooltip_giude{display:none;}

.area_my_menu>.inner{display:block; position: relative;width:1100px;;margin:0 auto;}
.area_my_menu{display:none;position:fixed;top:0px; left:0;right:0;background:#85766C; padding:50px 0;z-index:999;}
.area_my_menu>.inner li{box-sizing: border-box;}
.area_my_menu>.inner .tit{text-align:left;padding:25px 0;max-width:1280px;position:relative;box-sizing:border-box; margin-bottom:0;}
.area_my_menu>.inner .tit:after{display:block;content:'';clear:both;}
.area_my_menu>.inner .tit>p{position:absolute;left:0;top:0;width:100px;height:126px;background:url("/images/n21/avt/area_my_menu_bg.png") 0 50% no-repeat;}
.area_my_menu>.inner .tit>div{vertical-align:middle;padding-top:30px;margin-left:140px;}
.area_my_menu>.inner .tit>div:after{display:block;content:'';clear:both;}
.area_my_menu>.inner .tit>div>strong{float:left;width:250px;height:56px;vertical-align:bottom;padding:0 25px 0 0;box-sizing:border-box;color:#fff;font-size:46px;line-height:46px;position:relative;}
.area_my_menu>.inner .tit>div>strong:after{position:absolute;right:0;top:-8px;display:block;content:'';width:23px;height:29px;background:url("/images/n21/avt/my_menu_txt_bg.png") 100% 0 no-repeat;}
.area_my_menu>.inner .tit>div>span{float:right;height:46px;border-bottom:1px solid #fff;color:#fff;width:calc(100% - 250px);box-sizing:border-box; padding-top:15px;text-align:right;font-size:18px;}
.area_my_menu .menu_card{margin:0 -5px 50px -5px;}
.area_my_menu .menu_card:after{display:block;clear:both;content:'';}
.area_my_menu .menu_card>div{padding:0 5px;margin:5px 0;float:left;width:20%;box-sizing: border-box;}

.area_my_menu .menu_card>div>div{position:relative;border:solid 2px rgba(255,255,255,0.3); border-radius:10px;background:url("/images/n21/rvt/menu_card_add.png") 50% 50% no-repeat;}
.area_my_menu .menu_card>div>div .mascot{position:absolute;top:0;left:10px;height:100%; }
.area_my_menu .menu_card>div:nth-child(1)>div .mascot{width:73px;background:url("/images/n21/rvt/menu_card_icon1_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(2)>div .mascot{width:87px;background:url("/images/n21/rvt/menu_card_icon2_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(3)>div .mascot{width:74px;background:url("/images/n21/rvt/menu_card_icon3_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(4)>div .mascot{width:92px;background:url("/images/n21/rvt/menu_card_icon4_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(5)>div .mascot{width:68px;background:url("/images/n21/rvt/menu_card_icon5_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(6)>div .mascot{width:74px;background:url("/images/n21/rvt/menu_card_icon6_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(7)>div .mascot{width:83px;background:url("/images/n21/rvt/menu_card_icon7_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(8)>div .mascot{width:75px;background:url("/images/n21/rvt/menu_card_icon8_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(9)>div .mascot{width:71px;background:url("/images/n21/rvt/menu_card_icon9_off.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(10)>div .mascot{width:88px;background:url("/images/n21/rvt/menu_card_icon10_off.png") 0 50% no-repeat;}

.area_my_menu .menu_card>div:nth-child(1)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon1_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(2)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon2_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(3)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon3_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(4)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon4_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(5)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon5_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(6)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon6_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(7)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon7_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(8)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon8_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(9)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon9_on.png") 0 50% no-repeat;}
.area_my_menu .menu_card>div:nth-child(10)>div>div .mascot{background:url("/images/n21/rvt/menu_card_icon10_on.png") 0 50% no-repeat;}

.area_my_menu .menu_card>div>div>.add{display:block;width:100%;height:130px;line-height:130px;border-radius:10px;margin:-2px -2px -2px 0;text-indent:-99999em;}
.area_my_menu .menu_card>div>div>div{background:#fff;display:block;height:130px;line-height:130px;border-radius:10px;margin:-2px;padding:0 20px;text-align:left;z-index:-1;}
.area_my_menu .menu_card>div>div>div div{padding-left:80px;width:100%;display:inline-block;vertical-align:middle;line-height:24px;}
.area_my_menu .menu_card>div>div>div div em{display:block;color:#3f57bf;font-size:15px; font-weight:600;}
.area_my_menu .menu_card>div>div>div div span{display:block;color:#555;font-size:18px;}
.area_my_menu .menu_card>div>div .del{position:absolute;top:0;right:0;width:40px;height:39px;background:url("/images/n21/rvt/btn_menu_card_del.png") 50% 50% no-repeat;text-indent:-99999px;}
.area_my_menu>.inner ul:after{display:block;clear:both;content:'';}
.area_my_menu>.inner ul li{position:relative;width:16.66%;float:left;border-left:solid 1px #F5F3F1;text-align:center;}
.area_my_menu>.inner ul li:first-child{border-left:none;}
.area_my_menu>.inner ul li a{position:relative;display:inline-block;padding:0 5px;color:#fff; line-height:26px; font-size:20px;}
.area_my_menu>.inner ul li a span{font-size:18px;display:inline-block;vertical-align:top;width:31px;height:26px;padding-left:30px;}
.area_my_menu>.inner ul li a:hover:before{display:block;content:'';position:absolute;bottom:0;left:0;width:100%;height:8px;background:rgba(172,179,200,1);animation-name: user_ex5; animation-duration: .5s;z-index:-1;}
.area_my_menu>.inner ul li a:not(:hover):before{display:block;content:'';position:absolute;bottom:0;left:0;width:0;height:8px;background:rgba(172,179,200,1);animation-name: user_ex5_2; animation-duration: .1s;z-index:-1;}

@keyframes user_ex5{
	from { width:0 }
	to { width:100%; }
}
@keyframes user_ex5_2{
	from { width:100% }
	to { width:0; }
}

.area_my_menu>.inner ul li:nth-child(1) a span{background:url("/images/n21/rvt/my_menu_area_baro_img1.png") 0 50% no-repeat;}
.area_my_menu>.inner ul li:nth-child(2) a span{background:url("/images/n21/rvt/my_menu_area_baro_img2.png") 0 50% no-repeat;}
.area_my_menu>.inner ul li:nth-child(3) a span{background:url("/images/n21/rvt/my_menu_area_baro_img3.png") 0 50% no-repeat;}
.area_my_menu>.inner ul li:nth-child(4) a span{background:url("/images/n21/rvt/my_menu_area_baro_img4.png") 0 50% no-repeat;}
.area_my_menu>.inner ul li:nth-child(5) a span{background:url("/images/n21/rvt/my_menu_area_baro_img5.png") 0 50% no-repeat;}
.area_my_menu>.inner ul li:nth-child(6) a span{background:url("/images/n21/rvt/my_menu_area_baro_img6.png") 0 50% no-repeat;}
.area_my_menu>.inner>.btn_area_my_menu_close{position:absolute;top:10px;right:0;width:28px;height:28px;background:url("/images/n21/rvt/btn_area_my_menu_close.png") 50% 50% no-repeat;text-indent:-99999px;}




@media screen and (max-width: 1120px) {
	.top_banner .banner_text {
		display: none;
	}
}

@media screen and (max-width: 1024px) {
	
}

@media screen and (max-width: 768px) {
	.header_wrap {
		height: 58px;
	}
	.header_wrap .inner {
		position: relative;
		width: 100%;
		padding: 12px 16px;
	}
	.header_wrap .logo {
		width: 160px;
		padding: 0;
	}
	.top_banner .banner_vote:hover .banner_tooltip {
		display:none;
	}
	.header_wrap .tooltip_btn {
		display:none;
	}
	.top_banner {
		width: 100%;
		height: 80px;
	}
	.top_notice_inner {
		width: calc(100% - 60px);
		padding: 0 15px;
	}
	.top_notice_swiper .swiper-slide {
		padding: unset;
	}
	.top_banner .inner::before {
		display:none;
	}
	.banner_vote>span {
		display: block;
	}
	/* GNB */
	#gnb {
		display: none;
	}
	#gnb .depth2 {
		position: static;
		height:auto;
		min-height:auto;
		padding:20px 6px 0;
	}
	#gnb .depth2_li_link {
		margin:0;
	}	
	#gnb .depth2_li_link + .depth2_li_link {
		margin-top:12px;
	}
	#gnb.m_on .depth1 .depth1_li {
		justify-content:flex-start;
	}
	#gnb.m_on .depth1 .depth1_li:first-child {
		margin-top:0;
	}
	#gnb.m_on .depth1 .depth1_li.m_on .depth2 {
		display:block;
	}
	#gnb.m_on .depth1 .depth1_li.m_on .depth1_li_link {
		color:#66558A;
	}
	.header_wrap .top_side .nec_home {
		display: none;
	}
	.top_notice_close {
		display: none;
	}
	.header_wrap .top_side {
		position: absolute;
		right: 16px;
	}
	.header_wrap .top_side_link:nth-child(2) {
		display:none;
		/* position: relative;
		width: 20px;
		height: 20px;
		padding-top: 0;
		background: url("/images/n24/rvt/header/star.png") center no-repeat;
		background-size: 20px; */
	}
	#gnb.m_on .depth1 .depth1_li::after {
		content:'';
		display:flex;
		position:absolute;
		top:0;left:0;
		width:100%;
		height:100%;
		z-index:10;
		pointer-events:none;
	}
	#gnb.m_on .depth1 .depth1_li:nth-child(3) .depth1_li_link {
		pointer-events:none;
	}
	#gnb.m_on .depth1 .depth1_li:nth-child(3)::after{
		background: url("/images/n24/rvt/header/icon_gnb_open.png") top right no-repeat;
		background-size:24px;
	}
	#gnb.m_on .depth1 .depth1_li.m_on:nth-child(3)::after {
		background: url("/images/n24/rvt/header/icon_gnb_close.png") top right no-repeat;
		background-size:24px;
	}
	.header_wrap .m_mymenu {
		position: absolute;
		display: block;
		width: 60px;
		bottom: -25px;
		left: -20px;
		z-index: 17;
		padding: 4px 6px;
		border-radius: 2px;
		font-size: 10px;
		font-weight: 700;
		color: #fff;
		background: #2F3B52;
	}
	.header_wrap .m_mymenu:after {
		position: absolute;
		top: -3px;
		left: 26px;
		transform: rotate(45deg);
		display: block;
		content: '';
		width: 8px;
		height: 8px;
		color: #fff;
		background-color: #2F3B52;
	}
	.m_menu {
		display: block;
		width: 24px;
		height: 24px;
		margin-left: 10px;
		background: url("/images/n24/rvt/header/m_menu.png") center no-repeat;
		text-indent: -9999px;
		background-size: 24px;
	}
	.m_menu.m_on {
		background: url("/images/n24/rvt/header/m_menu_close.png") center no-repeat;
		background-size: 24px;
	}
	.top_side .pc-tooltip {
		display: none;
	}
	.tooltip.onlymobile{border:solid 1px red;display:none;position:fixed;top:50%;right:initial;left:50%;border:solid 1px #009fa1;border-radius:20px;width:385px;transform:translate(-50%, -50%);background:#fff url("/images/n21/rvt/tooltip_bg.png") 15px 20px no-repeat;box-shadow:2px 2px 0 rgba(0,0,0,.2);background-size: auto 90px;z-index:1000;}
	.tooltip.onlymobile:before{display:block;content:initial;}
	.tooltip.onlymobile>div{position:relative;text-align:left;}
	.tooltip.onlymobile .upper{padding:30px 0 15px 100px;height:initial;}
	.tooltip.onlymobile .lower{background:#f2f2f2;padding:15px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;}
	.tooltip.onlymobile .lower dl{margin-bottom:15px;}
	.tooltip.onlymobile .lower dt.title{font-size:17px;font-weight:bold;}
	.tooltip.onlymobile .lower dd{font-size:15px;}
	.tooltip.onlymobile .lower ul li{position:relative;font-size:13px;padding-left:10px;}
	.tooltip.onlymobile .lower ul li:first-child{margin-bottom:10px;}
	.tooltip.onlymobile .lower ul li:before{display:block;content:"*";position:absolute;left:0;top:0;color:#009fa1;}
	.tooltip.onlymobile>div em{display:inline-block;font-size:19px;color:#333;margin-bottom:5px;line-height:24px;}
	.tooltip.onlymobile>div b{font-weight:800;color:#333;}
	.tooltip.onlymobile>div span{display:block;font-size:16px;color:#333;}
	.tooltip.onlymobile .btn_close_tooltip{display:block;position:absolute;right:15px;top:15px;width:20px;height:20px;background:url("/images/n21/rvt/btn_close_tooltip.png") 0 0 no-repeat;text-indent:-9999px;background-size:contain;}
	.tooltip_giude{display:block;text-align:right;margin-bottom:15px;}
	.tooltip_giude button {background:#85766C;color:#fff;border-radius:4px;padding:5px 10px;border:1px solid #ffdec8;}
	.tooltip_giude button span{display:inline-block;vertical-align:middle;line-height:24px;}
	.tooltip_giude button i{display:inline-block;vertical-align:middle;width:24px;height:24px;border:solid 1px #fff;border-radius:50%;margin-left:5px;background:url("/images/n21/rvt/btn_mymenu_icon.png") 50% 50% no-repeat;text-indent:-9999em;}
	
	.top_banner .inner {
		flex-wrap: wrap;
		padding: 8px 0 10px 10px;
	}
	.top_banner .banner_logo {
		width: 100%;
		height: 18px;
		background: url("/images/n24/rvt/header/vote_date_mb_2025.png") no-repeat left top;
		background-size: auto 100%;
	}
	.top_banner .banner_vote {
		display: block;
		width: 100%;
		margin-top: 5px;
	}
	.top_banner .banner_vote .tit {
		width: 61px;
		font-size: 11px;
		text-align: center;
		margin-right: 4px;
	}
	.top_banner .banner_vote+.banner_vote {
		margin-left: 0;
		margin-top: 2px;
	}
	.top_banner .banner_vote .date {
		font-size: 11px;
	}
	.top_banner .banner_vote .date b {
		font-size: 14px;
	}
	.top_notice_inner {
		width: calc(100% - 8px);
	}
	.top_notice_swiper .swiper-slide {
		justify-content: flex-start;
	}
	.top_notice_swiper .btn-prev {
		background: url("/images/n24/rvt/header/btn_topbnr_prev_mb.png") no-repeat left top/100% auto;
	}
	.top_notice_swiper .btn-next {
		background: url("/images/n24/rvt/header/btn_topbnr_next_mb.png") no-repeat left top/100% auto;
	}
	.top_notice_swiper .btn-close {
		display: block;
	}
	.top_notice_swiper .btn-stop {
		display: none;
	}
}

@media screen and (max-width: 360px) {
	.main_vote_wrap .icon_vote {
		display: none !important;
	}
	.count_day_wrap {
		width: 100% !important;
		margin-left: 0 !important;
	}
}

@media screen and (max-width: 280px) {
	.top_banner .banner_logo {
		height:16px;
	}
	.top_banner .banner_vote .tit {
		width:56px;
		font-size:10px;
		margin-right:2px;
	}
	.top_banner .banner_vote .date {
		font-size:10px;
	}
	.top_banner .banner_vote .date b {
		font-size:12px;
	}
}

/* 나만의 메뉴 설정하기 */
.my_menu_option{display:none;position:fixed;top:50px;bottom:50px;width:840px;left:50%;margin-left:-420px;padding:50px;border-radius:10px;border-radius:10px;background:#fff;z-index:1000;}
.my_menu_option>strong{display:block;text-align:center;font-size:34px;color:#333;margin-bottom:30px;font-weight:normal;}
.my_menu_option>strong b{font-weight:700;}
.my_menu_option .my_search{position:relative;margin-bottom:40px;padding-right:75px;}
.my_menu_option .my_search div{position:relative;height:64px;border-radius:10px;border:solid 2px #85766C;width:100%;}
.my_menu_option .my_search div input[type="text"]{border:none;height:60px;line-height:60px;padding:0 20px;width:90%;border-radius:13px;outline:none;}
.my_menu_option .my_search div input[type="submit"]{position:absolute;top:50%;right:18px;width:33px;height:32px;margin-top:-16px;background:url("/images/n21/rvt/btn_my_search.png") 50% 50% no-repeat;text-indent:-99999px;}
.my_menu_option .my_search .btn_reflsh{position:absolute;top:0;right:0;width:71px;height:64px;background:url("/images/n24/rvt/icon_refresh.png") 50% 50% no-repeat;background-color:#85766C;background-size:32px;border-radius:10px;text-indent:-99999px;}
.my_menu_option .area_scroll{position:absolute;left:50px;right:50px;top:190px;bottom:65px;overflow:hidden;overflow-y:auto;}
.my_menu_option .p_posi{position:relative;margin-bottom:10px;padding:8px 0;}
.my_menu_option .p_posi h4{display:inline-block;margin-bottom:0;}
.my_menu_option .p_posi select{position:absolute;right:0;border-radius:4px;color:#555;font-size:15px;width:256px;height:40px;background:#fff url("/images/n21/rvt/mymenu_select_bg.png") right 10px center no-repeat;}
.my_menu_option h4{font-size:22px;font-weight:800;color:#856C6C;margin-bottom:10px;}
.my_menu_option h5{font-size:18px;font-weight:800;color:#333;margin:0 0 10px 0;}
.my_menu_option .h4_layer_contents{margin-bottom:20px;}
.my_menu_option .layer_contents_scroll{}/*height:340px;overflow:auto;*/
.my_menu_option .check_con{background:#fafafa;margin-bottom:20px;padding:25px 30px;border-radius:10px;}
.my_menu_option .check_con:after{display:block;clear:both;content:'';}
.my_menu_option .check_con span{font-size:14px;position:relative;float:left;width:33.33%;margin:5px 0;text-align:left;padding-left:25px;}
.my_menu_option .check_con span input[type="checkbox"] { position:absolute; top:50%; left:0; width:18px;height:18px;margin-top:-9px; -webkit-appearance:none;background:url("/images/n21/rvt/my_menu_option_check_off.png") 50% 50% no-repeat;}
.my_menu_option .check_con span input[type="checkbox"]:checked{background:url("/images/n21/rvt/my_menu_option_check_on.png") 50% 50% no-repeat;}
.my_menu_option .check_con span.none{display:block;text-align:center;width:100%;}
.my_menu_option .btnArea{text-align:center;position:absolute;margin:0;padding:10px 0;bottom:0;left:0;width:100%;background:#fff;border-radius:0 0 10px 10px}
.my_menu_option .btnArea button{display:inline-block;font-size:18px;font-weight:700;vertical-align:middle;width:150px;height:50px;line-height:50px;color:#fff;border-radius:4px;}
.my_menu_option .btnArea button.focus{background:#856C6C;}
.my_menu_option .btnArea button.close{background:#6f6f6f;}
.my_menu_option .btn_my_menu_option_close{position:absolute;top:25px;right:-25px;width:50px;height:50px;background:#856C6C url("/images/n24/rvt/icon_layer_close2.png") 50% 50% no-repeat;background-size:24px;border-radius:10px;text-indent:-99999px;}

@media screen and (min-width: 1024px) {
	.my_menu_option .my_search div button[type="submit"] {right: 18px;width: 33px;height: 32px;}
	.my_menu_option .my_search div button[type="submit"]::before {width: 33px;height: 32px;}
}
.my_menu_option .my_search div button[type="submit"] {position: absolute;top: 50%;-webkit-transform: translateY(-50%);transform: translateY(-50%);right:12px;width: 26px;height: 26px;}
.my_menu_option .my_search div button[type="submit"]::before {content: '';position: absolute;top: 50%;left: 0;right: 0;-webkit-transform: translateY(-50%);transform: translateY(-50%);margin: 0 auto;width: 26px;height: 26px;background: url("/images/n24/rvt/icon_search2.png") left top/100% auto;}


@media screen and (max-width:768px){
	/* 모바일 카드반응형 서브페이지 */
	.area_my_menu .inner{display:block; position: relative;}
	.area_my_menu{display:none; position:fixed; top:0px !important; left:0; right:0; background:#85766C; height:100%; overflow-y:auto; padding-top:0; z-index:999;}
	.area_my_menu>.inner li{box-sizing: border-box;}
	.area_my_menu>.inner{position:relative; padding:3% 3% 0 3%;width:auto;overflow:auto; }
	.area_my_menu>.inner .tit{padding:10px 20px;}
	.area_my_menu>.inner .tit>p{display:inline-block;vertical-align:middle;width:55px;height:80px;background:url("/images/n21/rvt/m_area_my_menu_bg.png") 0 50% no-repeat;background-size:55px;}
	.area_my_menu>.inner .tit>div{width:80%;border-bottom:none;padding-top:0;margin-left:54px;}
	.area_my_menu>.inner .tit>div>strong{width:auto;font-weight:normal;display:inline-block;padding:0 30px 0 0;color:#fff;font-size:20px;line-height:1.5;height:auto;}
	.area_my_menu>.inner .tit>div>span{display:block;font-size:14px;width:inherit;height:inherit;line-height:inherit;text-align:inherit;vertical-align:inherit;width:100%;padding:0px 20px 0 0;border-bottom:0;}

	.area_my_menu .menu_card>div{width:33.33%;}
	.area_my_menu .menu_card>div>div{height:80px;background:url("/images/n21/rvt/m_menu_card_add.png") 50% 50% no-repeat;background-size:20px;}
	.area_my_menu .menu_card>div>div .mascot{background-size:100% !important;}
	.area_my_menu .menu_card>div:nth-child(1)>div .mascot{width:36px;background:url("/images/n21/rvt/menu_card_icon1_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(2)>div .mascot{width:43px;background:url("/images/n21/rvt/menu_card_icon2_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(3)>div .mascot{width:36px;background:url("/images/n21/rvt/menu_card_icon3_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(4)>div .mascot{width:46px;background:url("/images/n21/rvt/menu_card_icon4_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(5)>div .mascot{width:34px;background:url("/images/n21/rvt/menu_card_icon5_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(6)>div .mascot{width:36px;background:url("/images/n21/rvt/menu_card_icon6_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(7)>div .mascot{width:41px;background:url("/images/n21/rvt/menu_card_icon7_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(8)>div .mascot{width:37px;background:url("/images/n21/rvt/menu_card_icon8_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(9)>div .mascot{width:35px;background:url("/images/n21/rvt/menu_card_icon9_off.png") 0 50% no-repeat;}
	.area_my_menu .menu_card>div:nth-child(10)>div .mascot{width:44px;background:url("/images/n21/rvt/menu_card_icon10_off.png") 0 50% no-repeat;}

	.area_my_menu .menu_card>div>div>.add{display:block;width:100%;height:80px;line-height:80px;border-radius:10px;text-indent:-99999em;}
	.area_my_menu .menu_card>div>div>div{height:80px;line-height:80px;margin:-2px;padding:0 10px;}
	.area_my_menu .menu_card>div>div>div div{padding-left:50px;width:100%;display:inline-block;vertical-align:middle;line-height:24px;text-align:right;}
	.area_my_menu .menu_card>div>div>div div em{font-size:14px;}
	.area_my_menu .menu_card>div>div>div div span{font-size:15px;}
	.area_my_menu .menu_card>div>div .del{position:absolute;top:-20px;;right:5px;width:25px;height:25px;background:url("/images/n21/rvt/m_btn_menu_card_del.png") 50% 50% no-repeat;background-size:25px;text-indent:-99999px;border-radius:50%;box-shadow:4px 4px 10px rgba(0,0,0,.3);}

	.area_my_menu ul{background:#85766C;margin:0 -3%;padding:3%;}
	.area_my_menu>.inner ul li{position:relative;width:50%;float:left;margin:5px 0;border-left:none;text-align:left;}
	.area_my_menu>.inner ul li a {font-size:14px;}
	.area_my_menu>.inner ul li a span{display:inline-block;vertical-align:middle;width:40px;height:40px;margin-right:5px;border-radius:50%;background-size:20px !important;}

	.area_my_menu>.inner ul li:nth-child(1) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img1.png") 50% 50% no-repeat;}
	.area_my_menu>.inner ul li:nth-child(2) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img2.png") 50% 50% no-repeat;}
	.area_my_menu>.inner ul li:nth-child(3) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img3.png") 50% 50% no-repeat;}
	.area_my_menu>.inner ul li:nth-child(4) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img4.png") 50% 50% no-repeat;}
	.area_my_menu>.inner ul li:nth-child(5) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img5.png") 50% 50% no-repeat;}
	.area_my_menu>.inner ul li:nth-child(6) a span{background:#85b88a url("/images/n21/rvt/m_my_menu_area_baro_img6.png") 50% 50% no-repeat;}
	.area_my_menu>.inner>.btn_area_my_menu_close{position:absolute;top:10px;right:10px;width:20px;height:20px;background:url("/images/n21/rvt/m_btn_area_my_menu_close.png") 50% 50% no-repeat;background-size:25px;text-indent:-99999px;}

	.area_my_menu>.menu_scroll>ul{background:#7a86ba;margin:0 -3%;padding:3% 3% 100px;}
	.area_my_menu>.menu_scroll>ul:after{display:block;clear:both;content:'';}
	.area_my_menu>.menu_scroll>ul li{position:relative;width:50%;float:left;margin:5px 0;}
	.area_my_menu>.menu_scroll>ul li a{display:block;font-size:16px;color:#fff;}
	.area_my_menu>.menu_scroll>ul li span{display:inline-block;vertical-align:middle;width:40px;height:40px;margin-right:5px;border-radius:50%;background-size:20px !important;}
	
	.my_menu_option {top:50%;width:96%;transform:translate(-50%, -50%);margin-left:0;padding:25px;height:95%;}
	.my_menu_option>strong{font-size:22px;margin-bottom:10px;font-weight:700;}
	.my_menu_option .my_search{position:relative;margin-bottom:20px;padding-right:50px;}
	.my_menu_option .my_search div{height:42px;}
	.my_menu_option .my_search div input[type="text"]{height:38px;line-height:38px;padding:0 10px;}
	.my_menu_option .my_search div input[type="submit"]{width:30px;height:30px;margin-top:-15px;background:url("/images/n21/rvt/m_btn_my_search.png") 50% 50% no-repeat;background-size:25px;}
	.my_menu_option .my_search .btn_reflsh{position:absolute;top:0;right:0;width:44px;height:42px;background-size:23px;text-indent:-99999px;}
	.my_menu_option .area_scroll{position:absolute;left:3%;right:3%;top:116px;}
	.my_menu_option .p_posi select{position:inherit;right:inherit;width:100%;margin-top:inherit;background:#fff url("/images/n24/common/bg_selectbox_arrow_s.png") no-repeat 95% center/15px auto;}
	.my_menu_option .check_con{margin-bottom:10px;padding:5%;}
	.my_menu_option .check_con span{width:50%;}
	.my_menu_option .check_con span input[type="checkbox"] { position:absolute;top:0;margin-top:0;}
	.my_menu_option .check_con span label{line-height:18px;display:inline-block;vertical-align:top;}
	.my_menu_option .btn_my_menu_option_close{top:15px;right:15px;width:25px;height:25px;background:url("/images/n21/rvt/m_btn_my_menu_option_close.png") 50% 50% no-repeat;background-size:25px;}
	
	.my_menu_option .btnArea{position:fixed;bottom:0;left:0;right:0;text-align:center;margin:0;padding:0px}
	.my_menu_option .btnArea:after{display:block;clear:both;content:'';}
	.my_menu_option .btnArea button{float:left;font-size:18px;font-weight:700;width:50%;height:50px;line-height:50px;color:#fff;}
	.my_menu_option .btnArea button.focus{border-radius:10px 0 0 0;}
	.my_menu_option .btnArea button.close{border-radius:0 10px 0 0;}
	.my_menu_option .btn_my_menu_option_close:focus{border:4px solid black;}
	.my_menu_option .btn_my_menu_option_close{position:absolute;top:15px;right:15px;width:25px;height:25px;background:url("/images/n21/mrvt/m_btn_my_menu_option_close.png") 50% 50% no-repeat;background-size:25px;text-indent:-99999px;}

	

}





/* ==================== */


.menu_card_wrap {
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	-ms-flex-wrap: wrap;
	flex-wrap: wrap;
	-webkit-box-orient: horizontal;
	-webkit-box-direction: normal;
	-ms-flex-direction: row;
	flex-direction: row;
	-webkit-box-align: start;
	-ms-flex-align: start;
	align-items: flex-start;
	-webkit-box-pack: start;
	-ms-flex-pack: start;
	justify-content: flex-start;
	margin: -12px 0 0 -12px;
	/* max-height:558px; */
	width:100%;
}

@media screen and (min-width: 1024px) {
	.menu_card_wrap {
		margin: -20px 0 0 -20px;
		max-height:none;
		padding-bottom:20px;
	}
}

@media only screen and (min-device-width: 414px) and (max-device-height: 736px) and (-webkit-device-pixel-ratio: 3) {
	.menu_card_wrap {
		overflow-y: scroll;
		/*height: 816px;
		height: 92.30769vw;*/
	}
}

@media screen and (max-width: 375px) {
	.menu_card_wrap {
		overflow-y: scroll;
		/*height: 816px;
		height: 92.30769vw;*/
	}
}

@media screen and (max-width: 320px) {
	.menu_card_wrap {
		/*height: 657.33333px;
		height: 74.35897vw;*/
	}
}

@media only screen and (min-width: 768px) and (max-width: 1024px) { /* min-device-height:1024px를 수정함*/
	.menu_card_wrap {
		overflow-y: scroll;
		/*height: 500px;*/
	}
}

.menu_card_item {
	position: relative;
	margin: 12px 0 0 12px;
	border-radius: 16px;
	width: calc(50% - 12px);
	background: #F8F8F8 url("/images/n24/common/bg_favorite_menu.jpg") no-repeat center/auto 100%;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
	.menu_card_item {
		margin: 20px 0 0 20px;
		width: calc(50% - 20px);
		border-radius: 20px;
	}
}

@media screen and (min-width: 1024px) {
	.menu_card_item {
		margin: 20px 0 0 20px;
		width: calc(20% - 20px);
		border-radius: 20px;
	}
}

.menu_card_item::before {
	content: '';
	z-index: 0;
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	border: 1px dashed #BBBBBB;
	border-radius: inherit;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}

.menu_card_box {
	display: block;
}

@media screen and (max-width: 767px) {
	.menu_card_box {
		height: 26.15385vw;
		/* max-height:102px; */
	}
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
	.menu_card_box {
		height: 120px;
	}
}

@media screen and (min-width: 1024px) {
	.menu_card_box {
		height: 130px;
	}
}

.menu_card_box > button {
	cursor: pointer;
	z-index: 1;
	display: block;
	position: relative;
	width: 100%;
	height: 100%;
}

.menu_card_box .my_menu_category {
	display: inline-block;
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
	-webkit-box-pack: center;
	-ms-flex-pack: center;
	justify-content: center;
	padding: 4px 10px;
	border-radius: 5px;
	font-size: 14px;
	font-weight: 700;
	color: #856C6C;
	line-height: 1.3;
	letter-spacing: -0.01em;
	background: #F7EFE8;
}

@media screen and (max-width: 767px) {
	.menu_card_box .my_menu_category {
		padding: 0.51282vw 2.05128vw;
		font-size: 3.28974vw;
		border-radius: 3px;
	}
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
	.menu_card_box .my_menu_category {
		padding: 2px 8px;
		font-size: 12px;
		border-radius: 5px;
	}
}

.menu_card_box .my_menu_name {
	display: block;
	margin-top: 10px;
	font-size: 18px;
	font-weight: 500;
	color: #121212;
	line-height: 1.3;
	letter-spacing: -0.01em;
	word-break: keep-all;
}

@media screen and (max-width: 767px) {
	.menu_card_box .my_menu_name {
		font-size: 3.40256vw;
	}
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
	.menu_card_box .my_menu_name {
		font-size: 16px;
	}
}

.menu_card_box .btn_menu_delete {
	z-index: 3;
	position: absolute;
	top: 10px;
	right: 10px;
	width: 4.10256vw;
	height: 4.10256vw;
	background: url("/images/n24/common/bg_menu_delete.svg") no-repeat left top/100% auto;
}

@media screen and (min-width: 768px) {
	.menu_card_box .btn_menu_delete {
		width: 20px;
		height: 20px;
	}
}

.menu_card_addition {
	height: inherit;
}

.menu_card_addition a {
	position: relative;
	z-index: 1;
	display: block;
	width: 100%;
	height: 100%;
	border: 2px solid #856C6C;
	-webkit-box-shadow: 0px 4px 4px rgba(133, 108, 108, 0.3);
	box-shadow: 0px 4px 4px rgba(133, 108, 108, 0.3);
	border-radius: 16px;
	background: #FFF;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	overflow:hidden;
}

@media screen and (max-width: 767px) {
	.menu_card_addition a {
		padding: 4.10256vw;
	}
}

@media screen and (min-width: 768px) and (max-width: 1023px) {
	.menu_card_addition a {
		padding: 16px;
	}
}

@media screen and (min-width: 1024px) {
	.menu_card_addition a {
		padding: 20px;
		border-radius: 20px;
	}
}

.menu_card_addition a::before {
	content: '';
	z-index: -1;
	position: absolute;
	bottom: 12px;
	right: 12px;
	width: 78px;
	height: 78px;
	background: #FFF url("/images/n24/common/bg_ballot_mark.png") no-repeat left top/100% auto;
}

/* ==============================================================================================================
= Overlay 효과 배경 기본스타일 지정
============================================================================================================== */
#overlay{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,0.6);}
#overlay.active{display:block;}
#overlay2{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,0.6);z-index:11;}


/* 팝업 */
.mainPop{display:none;position:fixed;left:-1000px;top:-1000px;z-index:999;max-width:1000px;}
.mainPop .title{padding:0 20px;background:#393939;border-top-left-radius:15px;border-top-right-radius:15px;}
.mainPop .title b{display:block;line-height:50px;color:#fff;font-size:18px;}
.mainPop .popImg img,
.mainPop .popImg iframe{display:block;max-width:100% !important;}
.mainPop .closeDay{padding:0 15px;background:#393939;border-bottom-left-radius:15px;border-bottom-right-radius:15px;color:#fff;font-weight:500;line-height:36px;}
.mainPop .closeDay .inputSet input{margin-top:-3px;}
.mainPop .closeDay .btnClose{display:block;position:absolute;right:15px;bottom:11px;width:15px;height:15px;background:url(/images/n21/main/icon_mainPop_close.png) no-repeat;text-indent:-9999em;}
.mainPop .popImg.aTag-f a{position: absolute;top: 3px;left: 3px;width: calc(100% - 6px);height: calc(100% - 6px);}

.popImg {position:relative;  overflow:hidden;}
.popImg iframe,
.popImg object,
.popImg embed {position:absolute; top:0; left:0; width:100%; height:100%;}

.mainPop .closeDay{padding:0 15px;background:#393939;border-bottom-left-radius:15px;border-bottom-right-radius:15px;color:#fff;font-weight:500;line-height:36px;}
.mainPop .closeDay .inputSet input{margin-top:-3px;}
.mainPop .closeDay .btnClose{display:block;position:absolute;right:15px;bottom:11px;width:15px;height:15px;background:url(/images/n21/main/icon_mainPop_close.png) no-repeat;text-indent:-9999em;}


/* 팝업내링크 */
.pop-links{}
.pop-links ul{display:flex;width:100%;}
.pop-links ul li{width:25%;text-align:center;}
.pop-links ul li a{display:block;height:50px; color:#222; background:#fff; border-right:1px solid #ddd; border-top:1px solid #ddd; font-size:17px;font-weight:900; letter-spacing:-1px; display:flex;width:100%; justify-content:center;align-items:center;transition:all 0.2s;}
.pop-links ul li a:hover{font-size:18px;}
.pop-links .link1{background-color: #5d4803;}
.pop-links .link2{background-color: #6ca907;}
.pop-links .link3{background-color:#0f143f;}
.pop-links .link4{background-color:#cf6100;}

@media all and (max-width:640px){
	.pop-links ul{flex-wrap:wrap;}
	.pop-links ul li{width:50%;}
	.pop-links ul li a{font-size:12px;}
	body{font-size:13px;}
}

