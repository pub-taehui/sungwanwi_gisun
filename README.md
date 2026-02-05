# sungwanwi_gisun
지선이
/* select 초기화 */
select {
    -webkit-appearance: none;
    -moz-appearance: none;    
    appearance: none;
}
/* footer */
footer {
    display: flex;
    background-color: #3A3B44;
}
footer>.inner {
    position: relative;
    width:1330px;
    margin:0 auto;
    padding: 28px 0 32px;
}
footer .row1 {
    padding-bottom: 20px;
    position: relative;
}
footer .row2 {
    display: flex;
    justify-content: flex-start;
}
footer .row2 .footer_image {
    padding-left: 32px;
}
.footer-links:after {
    display: block;
    clear: both;
    content: '';
}
.footer-links li {
    position: relative;
    float: left;
    padding: 0 18px;
}
.footer-links li:first-child {
    padding-left: 0;
}
.footer-links li:after {
    display: block;
    content: '';
    position: absolute;
    top: 50%;
    left: 0;
    margin-top: -7px;
    width: 1px;
    height: 13px;
    background: #ccc;
}
.footer-links li:first-child:after {
    background: none;
}
.footer-links li a {
    display: block;
    color: #fff;
    font-size: 15px;
}
.footer-links li a b {
    color: #333;
    font-weight: nomal;
}
.mobile_f_select {
    display: none;
    border-radius: 50px;
    color: #fff;
    font-size: 14px;
    height: 40px;
    background: #171620 url("/images/n24/rvt/footer/bg_selectbox_arrow_w.png") no-repeat;
    background-position-x: 93%;
    background-position-y: center;
    background-size: 15px;
    padding: 0 38px 0px 16px;
    border: 1px solid rgba(255, 255, 255, 0.2);
}
.sido-baro {
    position: absolute;
    right: 3px;
    top: 0;
    width: 256px;
}
.sido-baro select {
    width: 100%;
    padding: 0px 16px;
    border-radius: 10px;
    color: #fff;
    font-size: 14px;
    height: 40px;
    background-color: #171620;
    border-radius: 50px;
    border: 1px solid rgba(255, 255, 255, 0.2);
}
.sido-baro .input_img {
    position: absolute;
    right: 1px;
    top: 1px;
    text-indent: -9999px;
    width: 38px;
    height: 38px;
    background: transparent url("/images/n24/rvt/footer/bg_selectbox_arrow_right.png") center center no-repeat;
    background-size: 17px;
    border-radius: 0px 50px 50px 0px;
}
footer address {
    color: #fff;
    font-size: 14px;
    line-height: 1.3;
    letter-spacing: -0.01em;
}
footer .goodcon {
    display: inline-block;
    vertical-align: middle;
    width: 106px;
    height: 50px;
    margin: 0 20px 0 0px;
    background: url("/images/n24/rvt/footer/btn_goodcontent.png") 50% 50% no-repeat;
    text-indent: -9999px;
}
footer .webwatch {
    display: inline-block;
    vertical-align: middle;
    width: 63px;
    height: 50px;
    margin: 0 20px 0 0px;
    background: url("/images/n24/rvt/footer/img_footer_WA_rvt.png") no-repeat;
    background-size:63px 50px;
    text-indent: -9999px;
}
footer .accessibility {
    display: inline-block;
    vertical-align: middle;
    width: 63px;
    height: 50px;
    background: url("/images/n24/rvt/btn_web_accessibility.png") 50% 50% no-repeat;
    text-indent: -9999px;
}
@media screen and (max-width: 1024px) {
    footer>.inner {
        width:100% !important;
        padding:24px 20px;
    }
    .footer-links li a {
        font-size:12px;
    }
    .sido-baro {
        display: none;
    }
    .mobile_f_select {
        display: block;
        margin-top: 12px;
        font-size: 12px;
        width: fit-content;
    }
    footer .row1 {
        padding-bottom: 12px;
    }
    footer address {
        font-size:12px;
    }
    .footer-links li {
        padding: 0 9px;
    }
    .footer-links li:after {
        height: 8px;
        margin-top: -4px;
    }
    footer .row2 {
        flex-direction: column;
        align-items:flex-start;
    }
    footer .row2 .footer_image {
        padding-left:0;
        padding-top: 12px;
    }
}
@media screen and (max-width: 768px) {
	footer>.inner {
        width:100% !important;
    }
    footer .row1 {
        display: flex;
        flex-direction: column;
    }
}
@media screen and (max-width: 321px) {
    .footer-links li {
        padding:0 7px;
    }
}
