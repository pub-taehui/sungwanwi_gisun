# sungwanwi_gisun
지선이
<footer>
			<div class="inner">
				<div class="row1">
				<!-- 하단에 자바스크립트로 이동 -->

					<ul class="footer-links">
						<li><a href="/site/nec/07/10702020000002020040802.jsp" title="새창열림" target="_blank">개인정보처리방침</a></li>
                	    <li><a href="/site/nec/07/10702030000002020040802.jsp" title="새창열림" target="_blank">저작권정책</a></li>
                   	 	<li><a href="/site/nec/05/10503070100002020040801.jsp" title="새창열림" target="_blank">연락처</a></li>
                	    <li><a href="/site/nec/05/10505010000002020040801.jsp" title="새창열림" target="_blank">찾아오시는길</a></li>
					</ul>
					
					<!-- 모바일용 -->
					<select onclick="if(this.value!='') window.open(this.value); $(this).val('');" class="mobile_f_select">
						<option selected="" value="">시·도 선거관리위원회 바로가기</option>
						<option value="https://su.nec.go.kr">서울특별시선거관리위원회</option>
						<option value="https://bs.nec.go.kr">부산광역시선거관리위원회</option>
						<option value="https://dg.nec.go.kr">대구광역시선거관리위원회</option>
						<option value="https://ic.nec.go.kr">인천광역시선거관리위원회</option>
						<option value="https://gj.nec.go.kr">광주광역시선거관리위원회</option>
						<option value="https://dj.nec.go.kr">대전광역시선거관리위원회</option>
						<option value="https://us.nec.go.kr">울산광역시선거관리위원회</option>
						<option value="https://sj.nec.go.kr">세종특별자치시선거관리위원회</option>
						<option value="https://gg.nec.go.kr">경기도선거관리위원회</option>
						<option value="https://gw.nec.go.kr">강원특별자치도선거관리위원회</option>
						<option value="https://cb.nec.go.kr">충청북도선거관리위원회</option>
						<option value="https://cn.nec.go.kr">충청남도선거관리위원회</option>
						<option value="https://jb.nec.go.kr">전북특별자치도선거관리위원회</option>
						<option value="https://jn.nec.go.kr">전라남도선거관리위원회</option>
						<option value="https://gb.nec.go.kr">경상북도선거관리위원회</option>
						<option value="https://gn.nec.go.kr">경상남도선거관리위원회</option>
						<option value="https://jj.nec.go.kr">제주특별자치도선거관리위원회</option>
					</select>
					
					<!-- 웹용 -->
					<div class="sido-baro">
						<label for="f_select_baro" class="soundOnly">시·도 선거관리위원회 바로가기</label>
						<select id="f_select_baro">
							<option selected="" value="">시·도 선거관리위원회 바로가기</option>
							<option value="https://su.nec.go.kr">서울특별시선거관리위원회</option>
							<option value="https://bs.nec.go.kr">부산광역시선거관리위원회</option>
							<option value="https://dg.nec.go.kr">대구광역시선거관리위원회</option>
							<option value="https://ic.nec.go.kr">인천광역시선거관리위원회</option>
							<option value="https://gj.nec.go.kr">광주광역시선거관리위원회</option>
							<option value="https://dj.nec.go.kr">대전광역시선거관리위원회</option>
							<option value="https://us.nec.go.kr">울산광역시선거관리위원회</option>
							<option value="https://sj.nec.go.kr">세종특별자치시선거관리위원회</option>
							<option value="https://gg.nec.go.kr">경기도선거관리위원회</option>
							<option value="https://gw.nec.go.kr">강원특별자치도선거관리위원회</option>
							<option value="https://cb.nec.go.kr">충청북도선거관리위원회</option>
							<option value="https://cn.nec.go.kr">충청남도선거관리위원회</option>
							<option value="https://jb.nec.go.kr">전북특별자치도선거관리위원회</option>
							<option value="https://jn.nec.go.kr">전라남도선거관리위원회</option>
							<option value="https://gb.nec.go.kr">경상북도선거관리위원회</option>
							<option value="https://gn.nec.go.kr">경상남도선거관리위원회</option>
							<option value="https://jj.nec.go.kr">제주특별자치도선거관리위원회</option>
						</select>
						<button type="button" id="inputBTN1" name="inputBTN1" class="input_img" title="새창열림">이동</button>
					</div>					
					<script>
                   	   var urlChange = '';
                       $("#f_select_baro").change(function(){
                           urlChange = $("#f_select_baro option:selected").val();
                           var urlTxt = $("#f_select_baro option:selected").text();
                           var selectTxt = urlTxt + " 새창열림 ";
                           $("#inputBTN1").attr("title", selectTxt);
                           //$("#inputBTN1").focus();
                       });

                       $("#inputBTN1").click(function(){
                    	   if(urlChange != "NO" && urlChange != "") {
                    		   window.open(urlChange);
                    	   }
                       });
                   </script>
                   
				</div>
				<div class="row2">
					<address>
						[13809] 경기도 과천시 홍촌말로 44 중앙선거관리위원회<br>
						대표전화 : 02-503-1114  /  선거법질의·신고제보 : 국번없이 <em>1390(유료)</em>
					</address>
					<div class="footer_image">
						<a href="#" onclick="javascript:popupOpen(2);return false;" title="새창열림" class="webwatch">과학기술정보통신부 WEB ACCESSIBILITY 마크(웹 접근성 품질인증 마크)</a>
					</div>
				</div>
			</div>
		</footer>
