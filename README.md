<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>The domain name lucky00.com might be for sale. | 444.cn</title>
        <link rel="stylesheet" type="text/css" href="./static/css/public.css?112114" />
        <link rel="stylesheet" type="text/css" href="./static/css/index.css?112114" />
        <!-- Code TG:@coredns  -->
    </head>
    <body>
    <div class="container">
        <div class="header"></div>
        <div class="main">
            <div class="domain replace">
                <!-- 这里是要被替换的 -->
                <!-- 这里是要被替换的 -->
            </div>
            <div class="content">
                <!-- <div class="h2">
                    您访问的域名
                    <span class="replace"></span>
                    可能会出售。
                </div> -->
                <div class="info-card">
                    <p>Hello.</p>
                    <p>The domain name <span class="replace"></span> might be for sale.</p>
                    <p>Domain list: <a href="https://444.cn/?domain=lucky00.com" target="_blank">444.cn</a></p>
                    <p style="padding-top: 10px;" id="weixin">
                        <a class="btn btn_blue">Online Service</a>
                        <span class="qr-preview"><a href="https://t.me/www444cn" target="_blank"><img src="./static/images/code.png" title="Telgram QR code" alt="Telgram QR code"></a></span>
                    </p>
                </div>
            </div>
        </div>
        <div class="footer"></div>
        <div style="display:none"><script>!function(p){"use strict";!function(t){var s=window,e=document,i=p,c="".concat("https:"===e.location.protocol?"https://":"http://","sdk.51.la/js-sdk-pro.min.js"),n=e.createElement("script"),r=e.getElementsByTagName("script")[0];n.type="text/javascript",n.setAttribute("charset","UTF-8"),n.async=!0,n.src=c,n.id="LA_COLLECT",i.d=n;var o=function(){s.LA.ids.push(i)};s.LA?s.LA.ids&&o():(s.LA=p,s.LA.ids=[],o()),r.parentNode.insertBefore(n,r)}()}({id:"3O6rlcRp1jC8spBy",ck:"3O6rlcRp1jC8spBy"});</script></div>
    </div>
</body>
<script>
function domainURI(str) {
    if (!str) return "";
    var match = str.match(/^(?:https?:\/\/)?([^\/]+)/i);
    return match ? match[1] : "";
}
window.onload = function() {
    var domain = "";
    if (window.frames.length !== parent.frames.length && document.referrer) {
        domain = domainURI(document.referrer);
    }
    if (!domain) {
        domain = document.domain;
    }
    var replaceBox = document.querySelectorAll(".replace");
    for (var i = 0; i < replaceBox.length; i++) {
        replaceBox[i].innerHTML = domain;
    }
    
    // 移动端二维码显示/隐藏处理（优化性能）
    var weixinEl = document.getElementById('weixin');
    if (weixinEl) {
        var isTouchDevice = 'ontouchstart' in window || navigator.maxTouchPoints > 0;
        var clickHandler = null;
        var docClickHandler = null;
        
        if (isTouchDevice) {
            // 预加载二维码图片
            var qrImg = weixinEl.querySelector('.qr-preview img');
            if (qrImg && qrImg.src) {
                var preloadImg = new Image();
                preloadImg.src = qrImg.src;
            }
            
            // 使用 requestAnimationFrame 优化点击处理
            clickHandler = function(e) {
                e.preventDefault();
                e.stopPropagation();
                var isActive = weixinEl.classList.contains('active');
                
                // 使用 requestAnimationFrame 优化 DOM 操作
                requestAnimationFrame(function() {
                    if (isActive) {
                        weixinEl.classList.remove('active');
                    } else {
                        weixinEl.classList.add('active');
                    }
                });
            };
            
            // 节流处理文档点击事件
            var docClickTimer = null;
            docClickHandler = function(e) {
                if (docClickTimer) return;
                docClickTimer = setTimeout(function() {
                    docClickTimer = null;
                    if (!weixinEl.contains(e.target)) {
                        requestAnimationFrame(function() {
                            weixinEl.classList.remove('active');
                        });
                    }
                }, 10);
            };
            
            weixinEl.addEventListener('click', clickHandler, {passive: false});
            document.addEventListener('click', docClickHandler, {passive: true});
        }
    }
    
    // 修复 iOS Safari问题
    function setViewportHeight() {
        var vh = window.innerHeight * 0.01;
        document.documentElement.style.setProperty('--vh', vh + 'px');
    }
    setViewportHeight();
    window.addEventListener('resize', setViewportHeight);
    window.addEventListener('orientationchange', function() {
        setTimeout(setViewportHeight, 100);
    });
}
</script>
</html>

