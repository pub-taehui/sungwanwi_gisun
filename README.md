# sungwanwi_gisun
지선이

@charset "UTF-8";

#container {
	position:relative;
}
#container::before,
#container::after {
	content:'';
	position:absolute;
}
#container::before {
	top:0;
	right:0;
	width:272px;
	height:139px;
	background-image:url(/images/n24/rvt/main/bg_main_top_right_circle.png);
	background-repeat:no-repeat;
	background-size:272px 139px;
}
#container::after {
	bottom:0;
	left:0;
	width:218px;
	height:282px;
	background-image:url(/images/n24/rvt/main/bg_main_bottom_left_circle.png);
	background-repeat:no-repeat;
	background-size:218px 282px;
}  
#container.rvt_search::before,
#container.rvt_search::after {
	display:none;
}
#container .main_content_wrap {
    width:1330px;
    margin:0 auto;
    padding:40px 0;
}
.main_content_wrap::before {
    content: '';
    
}
.main_content_wrap::after {
    content: '';
}
.main_top_content {
    position: relative;
    display:flex;
}

.main_vote_wrap {
    position: relative;
    padding:5px 40px 20px;
    display:flex;
    flex-direction:column;
    justify-content: center;
}
.main_vote_wrap::before {
    content:'';
    position:absolute;
    top:-143px;
    left:-51px;
    width:220px;
    height:220px;
    background:url("/images/n24/rvt/main/bg_top_vote_mark.png") no-repeat;
    background-size:100% auto;
    background-position: contaion;
}
.main_vote_wrap .icon_vote {
    height:64px;
    background: url("/images/n24/rvt/main/main_vote_hand.png") no-repeat center 100%/auto;
}
.txt_main_vote{
    display:flex;
    margin-top: 16px;
    font-family: 'Elice';
    font-size:30px;
    color:#222;
    align-items: baseline;
    justify-content: center;
    letter-spacing: -0.01em;
}
.txt_main_vote .txt_main_vote_small{
    font-size:24px;
    margin-right:6px;
}
.count_day{
    position: inherit;
    display:flex;
    margin-top:10px;
    font-family: 'ChakraPetch';
    font-size:64px;
    line-height: 1;
    color:#222;
    justify-content: center;
}
.count_day .data.today{
	font-family: 'Elice';
    font-size:40px;
}
.count_day .dday_dash {
    display: flex;
    margin:0 10px;
    position: relative;
    top:-4px;
}

/* 통합검색 */
.main_search_wrap {
    position: relative;
    margin-top: 18px;
    width: 410px;
}
.main_search_wrap .main_search_keyword {
    position: absolute;
    bottom:0;
}
.main_search_keyword .keyword_list {
    display:flex;
}
.main_search_keyword .keyword_list > li{
    padding-left:16px;
}
.main_search_keyword .keyword_list .keyword {
    font-weight: 500;
    font-size: 14px;
    letter-spacing: -0.01em;
    color: #555;
}
.main_search_wrap .input_main_search {
    position: relative;
    margin-bottom:26px;
    
    overflow: hidden;
}
.main_search_wrap #total_search {
    width: 100%;
    height: 52px;
    border-radius: 23px;
    padding:0 60px 0 20px;
    background: #FFFFFF;
    outline: 3px solid #2F3B52;
    outline-offset: -3px;
    border-radius: 25px;
    font-size:16px;
}
.main_search_wrap #total_search:focus, 
.main_search_wrap #total_search:focus-within {
    outline: 3px dashed #000;
    outline-offset: -3px;
}
.main_search_wrap .btn_total_search:focus, 
.main_search_wrap .btn_total_search:focus-within {
    outline: 2px dashed #000;
    outline-offset: 2px;
}
.main_search_wrap #total_search::placeholder {
    color:#888;
}
.main_search_wrap .btn_total_search{
    position: absolute;
    top:6px;
    right:6px;
    width:40px;
    height:40px;
    background-image: url("/images/n24/rvt/main/btn_total_search.png");
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;
    background-color: #2F3B52;
    border-radius: 50%;
    text-indent: -9999px;
    font-size:1px;
}

/******************* 메인 Tab 탭 ***********************/
.main_tab_wrap + .main_tab_wrap {
    margin-left:40px;
}
.main_tab_wrap {
    position: relative;
    width:400px;
    padding-top:12px;
}
.main_tab_wrap .tabBar {
    position: absolute;
    top:0;
    display: flex;
    align-items: center;
    width:100%;
    height:66px;
    text-align:center;
}
.main_tab_wrap .tabBar.col2 > li {
    width:50%;
}
.main_tab_wrap .tabBar.col3 > li {
    width:33.333%;
}
.main_tab_wrap .tabBar.col3 > li + li> a::before {
	content:'';
	position:absolute;
	top:50%;
	left:0;
	margin-top:-9px;
	width:1px;
	height:18px;
	background-color:rgba(47,59,82,0.2);
}
.main_tab_wrap .tabBar.col3 > li.active + li> a::before {
	display:none;
}
.main_tab_wrap .tabBar > li {
	position:relative;
    display:flex;
    justify-content: center;
    align-items: flex-end;
    height:100%;
}
.main_tab_wrap .tabBar .btn_tab {
	position:relative;
    display: flex;
    width:100%;
    height:43px;
    min-height:38px;
    font-size: 18px;
    font-weigth:500;
    color: #555;
    justify-content: center;
    align-items: center;
}
.main_tab_wrap .tabBar .active {
    display: flex;
}
.main_tab_wrap .tabBar .active .btn_tab {
    height:100%;
    background-color:#39977C;
    color:#fff;
    font-weight: 700;
}
.main_tab_wrap.type2 .tabBar .active .btn_tab {
    background-color:#66558A;
}
.main_tab_wrap .tabBar > li .btn_tab {
    border-top-left-radius: 4px;
    border-top-right-radius: 4px;
    border-bottom-left-radius: 16px;
    border-bottom-right-radius: 16px;
}
.main_tab_wrap .tabBar > li:first-child .btn_tab {
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 16px;
}
.main_tab_wrap .tabBar > li:last-child .btn_tab {
    border-bottom-left-radius: 16px;
    border-bottom-right-radius: 0;
}
.main_tab_wrap .tabContent {
    display: flex;
    height: 313px;
    border-radius: 12px;
    padding-top:54px;
}
.main_tab_wrap.type1 .tabContent {
    background-color:#E4F4EF;
}
.main_tab_wrap.type2 .tabContent {
    background-color:#E5E4F4;
}
.main_tab_wrap .tabPage {
    width: 100%;
}
.main_tab_wrap .tabPage .main_tab_content {
    display: flex;
    padding: 24px 16px 20px;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list {
    display: flex;
    flex-wrap: wrap;
    width:100%;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link {
    display: flex;
    width: calc(50% - 6px);
    height: 64px;
    margin-top:12px;
    border-radius: 8px;
    background: url("/images/n24/rvt/main/tab/bg_tab_no_cont.png") no-repeat center rgba(255, 255, 255, 0.5);
    background-size: contain;
    overflow: hidden;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link:first-child,
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link:nth-child(2) {
    margin-top:0;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link:nth-child(2n){
    margin-left:12px;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link > a {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    width:100%;
    height:100%;
    background-color: #fff;
    padding:0 16px 0 42px;
    font-size: 16px;
    font-weight: 500;
    line-height: 130%;
    letter-spacing: -0.01em;
    color: #222;
    border-radius: 8px;
    /* 탭 아이콘 */
    background-repeat: no-repeat;
    background-size: 22px;
    background-position-x: 16px;
    background-position-y: center;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link.on > a {
    font-weight: 700;
}
.main_tab_wrap.type1 .tabPage .main_tab_content .main_tab_link_list .btn_tab_link.on > a {
    color:#39977C;
    outline: 3px solid #39977C;
    outline-offset: -3px;
}
.main_tab_wrap.type2 .tabPage .main_tab_content .main_tab_link_list .btn_tab_link.on > a {
    color:#66558A;
    outline: 3px solid #66558A;
    outline-offset: -3px;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link.on > a::after {
    content:'';
    position: absolute;
    top:-11px;
    right:-6px;
    width:54px;
    height:54px;
    background-image: url("/images/n24/rvt/main/btn_tab_on_bg.png");
    background-repeat: no-repeat;
    background-size: 54px;
}
.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link > a:focus {
    outline: 3px solid #000;
    outline-offset: -3px;
}

.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link.txt_sp > a {
    letter-spacing: -0.1em;
}

/* 탭 아이콘 */
.main_tab_link_list.tab_info .btn_tab_link[data='후보자정보'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_01.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='정책공약'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_02.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='유효표와 무효표'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_03.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='(사전)투표방법'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_04.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='개표절차'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_05.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='선거사무안내'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_06.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='여론조사'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_07.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='투표용지 정보'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_08.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='정치관계법 사례예시'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_09.png");}
.main_tab_link_list.tab_info .btn_tab_link[data='내 선거구 검색'] > a,
.main_tab_link_list.tab_info .btn_tab_link[data='내 선거구 확인'] > a{background-image:url("/images/n24/rvt/main/tab/info/icon_10.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='후보자정보'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_01_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='정책공약'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_02_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='유효표와 무효표'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_03_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='(사전)투표방법'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_04_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='개표절차'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_05_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='선거사무안내'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_06_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='여론조사'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_07_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='투표용지 정보'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_08_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='정치관계법 사례예시'] > a {background-image:url("/images/n24/rvt/main/tab/info/icon_09_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on[data='내 선거구 검색'] > a,
.main_tab_link_list.tab_info .btn_tab_link.on[data='내 선거구 확인'] > a{background-image:url("/images/n24/rvt/main/tab/info/icon_10_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='사전투표소'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_01.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='선거일투표소'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_02.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='내 투표소 찾기<br/> 연결서비스'] > a,
.main_tab_link_list.tab_vote .btn_tab_link[data='투표소 찾기<br/> 연결서비스'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_03.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='사전투표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link[data='사전투표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_04.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='투표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link[data='투표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_05.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='개표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link[data='개표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_06.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='당선인'] > a,
.main_tab_link_list.tab_vote .btn_tab_link[data='당선인 현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_07.png");}
.main_tab_link_list.tab_vote .btn_tab_link[data='개표단위별 개표결과'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_08.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='사전투표소'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_01_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='선거일투표소'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_02_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='내 투표소 찾기<br/> 연결서비스'] > a,
.main_tab_link_list.tab_vote .btn_tab_link.on[data='투표소 찾기<br/> 연결서비스'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_03_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='사전투표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link.on[data='사전투표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_04_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='투표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link.on[data='투표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_05_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='개표현황'] > a,
.main_tab_link_list.tab_vote .btn_tab_link.on[data='개표 진행현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_06_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='당선인'] > a,
.main_tab_link_list.tab_vote .btn_tab_link.on[data='당선인 현황'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_07_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on[data='개표단위별 개표결과'] > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_08_on.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='정보보안시스템'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_01.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='(사전)투표'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_02.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='개표'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_03.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='방송영상·기사'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_04.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='기타'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_05.png");}
.main_tab_link_list.tab_true .btn_tab_link[data='알기쉬운 선거정보'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_06.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='정보보안시스템'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_01_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='(사전)투표'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_02_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='개표'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_03_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='방송영상·기사'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_04_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='기타'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_05_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on[data='알기쉬운 선거정보'] > a {background-image:url("/images/n24/rvt/main/tab/true/icon_06_on.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='투표율정보'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_01.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='선거통계'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_02.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='선거일정'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_03.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='선거법 질의 및<br> 위반행위 신고'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_04.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='서면/인터넷<br>질의보기'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_05.png");}
.main_tab_link_list.tab_law .btn_tab_link[data='판례보기'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_06.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='투표율정보'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_01_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='선거통계'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_02_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='선거일정'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_03_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='선거법 질의 및<br> 위반행위 신고'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_04_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='서면/인터넷<br>질의보기'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_05_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on[data='판례보기'] > a {background-image:url("/images/n24/rvt/main/tab/law/icon_06_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='선거비용<br>보전안내'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_01.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='후보자 등록신청<br>서류작성 프로그램'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_02.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='정당등록현황'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_03.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='정책연구소'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_04.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='강령·당헌'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_05.png");}
.main_tab_link_list.tab_hubo .btn_tab_link[data='후원회정보'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_06.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='선거비용<br>보전안내'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_01_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='후보자 등록신청<br>서류작성 프로그램'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_02_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='정당등록현황'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_03_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='정책연구소'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_04_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='강령·당헌'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_05_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on[data='후원회정보'] > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_06_on.png");}

/* .main_tab_link_list.tab_info .btn_tab_link:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_01.png");}
.main_tab_link_list.tab_info .btn_tab_link:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_02.png");}
.main_tab_link_list.tab_info .btn_tab_link:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_03.png");}
.main_tab_link_list.tab_info .btn_tab_link:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_04.png");}
.main_tab_link_list.tab_info .btn_tab_link:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_05.png");}
.main_tab_link_list.tab_info .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_06.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_01_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_02_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_03_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_04_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_05_on.png");}
.main_tab_link_list.tab_info .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/info/icon_06_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_01.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_02.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_03.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_04.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_05.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_06.png");}
.main_tab_link_list.tab_vote .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_07.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_01_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_02_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_03_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_04_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_05_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_06_on.png");}
.main_tab_link_list.tab_vote .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/vote/icon_07_on.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_01.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_02.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_03.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_04.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_05.png");}
.main_tab_link_list.tab_true .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_06.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_01_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_02_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_03_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_04_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_05_on.png");}
.main_tab_link_list.tab_true .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/true/icon_06_on.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_01.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_02.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_03.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_04.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_05.png");}
.main_tab_link_list.tab_law .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_06.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_01_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_02_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_03_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_04_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_05_on.png");}
.main_tab_link_list.tab_law .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/law/icon_06_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_01.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_02.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_03.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_04.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_05.png");}
.main_tab_link_list.tab_hubo .btn_tab_link:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_06.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(1) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_01_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(2) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_02_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(3) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_03_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(4) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_04_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(5) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_05_on.png");}
.main_tab_link_list.tab_hubo .btn_tab_link.on:nth-child(6) > a {background-image:url("/images/n24/rvt/main/tab/hubo/icon_06_on.png");} */

/* 메인하단 컨텐츠 */
.main_bottom_content {
    display: flex;
    margin-top:40px;
}
.main_slide_banner_wrap {
    position: relative;
    width:890px;
    overflow: hidden;
}
.main_bottom_right_wrap {
    display: flex;
    flex-direction: column;
    margin-left:40px;
}
.main_bottom_right_wrap .image_banner {
    width: 400px;
    margin-top:40px;
    border-radius:12px;
    overflow:hidden;
}
.main_bottom_right_wrap .image_banner a {
	display:block;
	width:100%;
}
.main_bottom_right_wrap .image_banner a:focus,
.main_bottom_right_wrap .image_banner a:focus-visible {
	outline:2px solid #000;
	outline-offset:-2px;
}
.main_bottom_right_wrap .image_banner img {
    width: 100%;
}
.main_rolling_banner_wrap {
    position: relative;
    width:400px;
    z-index:0;
}
.main_rolling_banner_wrap .swiper-slide > a {
	border-radius: 12px;
	overflow:hidden;
}
.main_rolling_banner_wrap .swiper-slide > a:focus,
.main_rolling_banner_wrap .swiper-slide > a:focus-visible {
	outline: 2px dashed #000;
    outline-offset: -2px;
}

/************************** 스와이퍼 **************************/
.swiper-slide {
    display: flex;
    justify-content: center;
    align-items: center;
    background: #fff;
}
.swiper-slide>a {display: block;}
.swiper-slide img {width: 100%;}

/* 메인 슬라이더 */
.main_slide_banner_wrap .swiper-slide > a {
    width: 280px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    border-radius: 12px;
    overflow:hidden;
}
.main_slide_banner_wrap .swiper-slide > a:focus,
.main_slide_banner_wrap .swiper-slide > a:focus-visible {
    outline: 2px dashed #000;
    outline-offset: -2px;
}
.main_slide_banner_wrap .banner-slider-nav {
    position: relative;
    z-index: 10;
    width:170px;
    margin: 10px auto 0;
}
.main_slide_banner_wrap .banner-slider-nav .slider-page {
	position:absolute;
	top:7px;
	left:34px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #565656;
    font-size: 16px;
    width:auto;
    margin-left: 20px;
    margin-right: 16px;
}
.main_slide_banner_wrap .banner-slider-nav .slider-page > span {
    position:relative;
    font-size:16px;
    line-height: 150%;
    margin-right:8px;
}
.main_slide_banner_wrap .banner-slider-nav .slider-page .swiper-pagination-current {
    font-weight:700;
}
.main_slide_banner_wrap .banner-slider-nav .slider-page .swiper-pagination-total {
    margin-right:0;
    margin-left:8px;
}
.main_slide_banner_wrap .banner-slider-nav .slider-controller {
	position:relative;
    display: flex;
    align-items: center;
    justify-content: center;
}
.main_slide_banner_wrap .banner-slider-nav .slider-controller button {
    display: block;
    width: 24px;
    height: 24px;
    border-radius: 50%;
    background-color: #fff;
    background-position: center center;
    background-repeat: no-repeat;
    background-size: contain;
    text-align: left;
    text-indent: -9999px;
    overflow: hidden;
    margin-right: 6px;
}
.main_slide_banner_wrap .banner-slider-nav .slider-controller button:last-child {margin-right: 0;}
.main_slide_banner_wrap .banner-slider-nav .slider-controller .btn-prev {margin-right:76px;background-image: url("/images/n24/rvt/main/btn_slide_prev.png");}
.main_slide_banner_wrap .banner-slider-nav .slider-controller .btn-next {background-image: url("/images/n24/rvt/main/btn_slide_next.png");}
.main_slide_banner_wrap .banner-slider-nav .slider-controller .btn-stop {background-image: url("/images/n24/rvt/main/btn_slide_stop.png");}
.main_slide_banner_wrap .banner-slider-nav .slider-controller .btn-stop.active {background-image: url("/images/n24/rvt/main/btn_slide_play.png");}

/* 메인 우측 롤링 스와이퍼 */
.main_rolling_banner {overflow: hidden;}
.main_rolling_banner_wrap .swiper-wrapper {
    z-index: 0;
}
.main_rolling_banner_wrap .banner-slider-nav {
    position: absolute;
    top: 10px;
    left: 10px;
    display: flex;
    z-index: 1;
}
.main_rolling_banner_wrap .banner-slider-nav .swiper-pagination {
    position: relative;
    bottom:0;
    display: flex;
    align-items: center;
}
.main_rolling_banner_wrap .banner-slider-nav .swiper-pagination .swiper-pagination-bullet {
    width:6px;
    height:6px;
    background-color: rgba(34, 34, 34, 0.4);
}
.main_rolling_banner_wrap .banner-slider-nav .swiper-pagination .swiper-pagination-bullet.swiper-pagination-bullet-active {
    width:20px;
    background-color:#222;
    border-radius: 50px;
}
.main_rolling_banner_wrap .banner-slider-nav .slider-controller {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left:9px;
}
.main_rolling_banner_wrap .banner-slider-nav .slider-controller button {
    display: block;
    width: 14px;
    height: 14px;
    border-radius: 50%;
    background-position: center center;
    background-repeat: no-repeat;
    background-size: contain;
    text-align: left;
    text-indent: -9999px;
    overflow: hidden;
    margin-right: 6px;
}
.main_rolling_banner_wrap .banner-slider-nav .slider-controller button:last-child {margin-right: 0;}
.main_rolling_banner_wrap .banner-slider-nav .slider-controller .btn-stop {background-image: url("/images/n24/rvt/main/btn_rolling_banner_stop.png");}
.main_rolling_banner_wrap .banner-slider-nav .slider-controller .btn-stop.active {background-image: url("/images/n24/rvt/main/btn_rolling_banner_play.png");}


@media screen and (max-width:1024px) {
    
}

@media screen and (max-width:769px) {
	#container::before,
	#container::after {
		display:none;
	} 
	#container .main_content_wrap {
        width:100%;
        padding: 24px 16px;
    }
    .main_top_content {
        flex-direction: column;
        width: 100%;
    }
    .main_vote_wrap{
        position: relative;
        width:100%;
        padding: 0 0 20px;
    }
    .main_vote_wrap::before {
        display: none;
    }
    .main_search_wrap {
        width: 100%;
        margin-top: 16px;
    }
    .main_vote_wrap .icon_vote {
        position: absolute;
        top:14px;
    }
    .main_vote_wrap .icon_vote {
        display: inline-block;
        width:52px;
        height:34px;
        background-size: contain;
    }
    .main_vote_wrap .txt_main_vote {
        margin-top:0;
    }
    .count_day_wrap {
        display: inline-flex;
        width:calc(100% - 60px);
        align-items: center;
        justify-content: space-between;
        margin-left:60px;
    }
    .count_day_wrap .count_day {
        margin-top:0;
    }
    .count_day .data.today {
    	font-size: 28px;
    }
    .main_tab_wrap {
        display: block;
        width: 100%;
    }
    .main_tab_wrap + .main_tab_wrap {
        margin-left:0;
        margin-top:20px;
    }
    .main_tab_wrap .tabContent {
        height:auto;
    }
    .main_bottom_content {
        flex-direction: column;
        margin-top:20px;
    }
    .main_slide_banner_wrap {
        width: 100%;
    }
    .main_bottom_right_wrap {
        flex-direction: column;
        margin-top:20px;
        margin-left:0;
    }
    .main_rolling_banner_wrap {
        width:100%;
    }
    .main_bottom_right_wrap .image_banner {
        width:100%;
        margin-left:0;
        margin-top:12px;
    }
    .main_search_wrap #total_search:focus, 
	.main_search_wrap #total_search:focus-within {
		outline:3px solid;
	}
    .main_tab_wrap {
        padding-top: 8px;
    }
    .main_tab_wrap .tabBar {
        height: 48px;
    }
    .main_tab_wrap .tabBar .btn_tab {
        font-size: 16px;
        height: 36px;
    }
    .main_tab_wrap .tabContent {
        padding-top: 40px;
    }
    .main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link {
        height: 42px;
    }
    .main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link > a {
        font-size:14px;
        background-size:18px;
        padding: 0 16px 0 38px;
    }
    .main_tab_wrap .tabBar.col3 > li + li> a::before {
    	margin-top:-8px;
    	height:16px;
    }
    .main_slide_banner_wrap .swiper-slide > a {
        width: auto;
    }
    .main_vote_wrap .txt_main_vote {
        flex-direction: column;
        font-size:24px;
        padding-left:2%;
    }
    .txt_main_vote .txt_main_vote_small {
        font-size: 18px;
    }
    .count_day {
        font-size: 38px;
    }
    .main_vote_wrap .icon_vote {
        top:14px;
    }
    .main_search_keyword .keyword_list .keyword {
        font-size:12px;
    }
    .main_search_wrap #total_search {
        font-size: 13px;
    }
    .top_notice_title {
        font-size:12px;
        line-height:1.6
    }
    .top_notice_swiper .swiper-wrapper, .top_notice_link {
        height:36px;
    }
    .count_day .dday_dash {
        margin: 0 5px;
    }
    .main_tab_wrap .tabPage .main_tab_content {
        padding:12px;
    }
    .main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link {
        width:calc(50% - 4px);
    }
    .main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link:nth-child(2n) {
        margin-left:8px;
    }
}


@media screen and (max-width:426px) {
    .main_bottom_right_wrap {
        flex-direction: column;
    }
    .main_rolling_banner_wrap {
        width: 100%;
    }
    .main_bottom_right_wrap .image_banner {
        width: 100%;
        margin-left:0;
        margin-top:20px;
    }
    .sns_menu_mobile .sns_list .btn_sns {
    	height:60px;
    }
}

@media screen and (max-width:280px){
	.main_vote_wrap .txt_main_vote {
		font-size:18px;
	}
	.txt_main_vote .txt_main_vote_small {
		font-size: 14px;
	}
	.main_search_wrap #total_search {
		height:46px;
	}
	.main_search_wrap .btn_total_search {
		top:5px;
		width:36px;
		height:36px;
	}
	.main_search_keyword .keyword_list > li {
		padding-left:8px;
	}
	.main_tab_wrap .tabBar .btn_tab {
		font-size:15px;
	}
	.main_tab_wrap .tabPage .main_tab_content .main_tab_link_list .btn_tab_link > a {
		font-size:13px;
		background-size:17px;
		background-position-x: 13px;
		padding:0 16px 0 36px;
		word-break:break-all;
	}
}

	    
