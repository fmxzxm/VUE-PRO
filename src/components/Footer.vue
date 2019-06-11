<template>
    <nav class="fixed-nav iphonex_padding iphonex_white" style="display: block;">
        <div class="nav-content row">
            <a href="/" class="col">
                <i class="icon icon-home"></i>
                <p>首页</p>
            </a>
            <a href="/discovery" class="col">
                <i class="icon icon-dicovery"></i>
                <p>发现</p>
            </a>
            <router-link to="Mmine" class="col active">
                <i class="icon icon-my"></i>
                <p>我的</p>
            </router-link>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
.fixed-nav {
  background-color: #fff;
  border-top: 1px solid #f5f5f5;
  text-align: center;
  position: fixed;
  left: 0;
  bottom: 0;
  z-index: 999;
  width: 100%;
}
* {
  -webkit-tap-highlight-color: transparent;
  outline: 0;
  margin: 0;
  padding: 0;
  vertical-align: baseline;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}

.fixed-nav .nav-content {
  display: -webkit-flex;
  display: flex;
  padding: 0.6rem 0 0.5rem;
}
.row {
  display: -webkit-box;
  display: -webkit-flex;
  display: flex;
}

.fixed-nav a {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
  font-size: 1.1rem;
  color: #333;
}
.col {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
}
a {
  color: inherit;
}
a {
  text-decoration: none;
  color: #333;
}

.fixed-nav .icon-home {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAAflBMVEUAAAAjGBVmZmZmZmYjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBVmZmYjGBUjGBUjGBVmZmYjGBVmZmZmZmZmZmZmZmZmZmZmZmYjGBUjGBUjGBVmZmaafbqRAAAAKHRSTlMAEMBQ+fEELQjMwrmsfm0m6NWTdWM2HNy0oJmJV0g4Ihzz48uQgD8Xdjtq3wAAANRJREFUOMvt0VcSgjAUBVDAhA6hgyjFHve/QctDEDIpn4zj/ePlzCVFW2/sAONQ0TYlfcYlCrTwKQSlpoSaKaJjHEtorzEw34HygF9+2wItG/iDoNwM8VBnvz6JKyjPHaj1us8khPI4X1I9ARrtv4bdUL6zZzaLmDGUY7Z8OJjLnqbwYCmZWqYdsMmg3J/hROc9afXe4Qxr/GSwrob1P/5N3G4Wafn4fGdy4eIDi49cfGKxwcV9bSxS96u/ZxWMqDR4xJ4c+yO2kLSYaJP2hBxVRFtRHoAOUBJdIzQPAAAAAElFTkSuQmCC);
}
.fixed-nav .icon {
  display: block;
  width: 2.1rem;
  height: 2.1rem;
  margin: 0 auto;
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
em,
i {
  font-style: normal;
}

.fixed-nav p {
  line-height: 1.7rem;
  height: 1.7rem;
}
blockquote,
body,
button,
dd,
dl,
dt,
fieldset,
form,
h1,
h2,
h3,
h4,
h5,
h6,
hr,
input,
legend,
li,
ol,
p,
pre,
td,
textarea,
th,
ul {
  margin: 0;
  padding: 0;
  vertical-align: baseline;
}

.fixed-nav a {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
  font-size: 1.1rem;
  color: #333;
}
.col {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
}
a {
  color: inherit;
}
a {
  text-decoration: none;
  color: #333;
}

.fixed-nav .icon-dicovery {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAAq1BMVEUAAABiYWEjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBUjGBVmZmZmZmYjGBVmZmYjGBUjGBVmZmZmZmYjGBVmZmZmZmZmZmZmZmZmZmZmZmZmZmZmZmYjGBUjGBUjGBVmZmZmZmZmZmYjGBVmZmYjGBUjGBUjGBUjGBVmZmYjGBVmZmZmZmZmZmZmZmZmZmZmZmYjGBVmZmZ0USAkAAAAN3RSTlMABvTppH7SQic5k4gr3B2MEw/XxbOGa2U1Fc6X8ubgzql+d3FcUk9GKyAPCbevmYxO9rKfa18lFATzsAAAAeBJREFUOMu9VdeygkAMBRUV7CCKvffe/f8vu8m2wILOqDM3L2SSw+7ZnGzW+MVM26qXUo9HqlS3bPMttFxIP0KWLpRfQmvOI2ZONRmbo1XDqx+TsAWRzVamdj5vTytZESjED5ZhiZSTp1jRSbFgRj8ox27L2oF3HB2NWizYjJNrsoQVDtmMQi7x2IxKKLUpUSCOxlxpEyXR0FHLkef6JmdCRGq40zaKDA7uE+0Cfh051kRigr+uCGguOr2ntLVhrDA/EUms/l4h58PuM2QtiO1RK57O449Si/XgGbE+U4cQDfDacmFfolw/OMPnoPZuSPFI/z5DeuM7EDqBt2DRipKxDd5Mlguh1xbz5+B2eVvM1ObYmUUBHgNgIPwO+EN0OOk085C9bHEPACPhY/lu3K0iRoFFyVvIIhCyyMKhbASmlW+Q74mFR3hQI7SyznkIgI4AYMHHhs6ZqmGidnNO6IoslgJM1aA6LyB/gmLdxx7JR3WWCmZVsc6B70oVfYiRgtQbRSUf2WANMeoN+s/hhSPrDudcPdl1Wj+vFbLXWSik7Gf9plx4vx0Cg4xuinYHTd/1RsvEaWB9dLs/mRvfTSSadbsXs+6bKUroytv5rNvxg8kPLZ78pvz+WsXfQePf7A/vX4tSGacr3AAAAABJRU5ErkJggg==);
}
.fixed-nav .icon {
  display: block;
  width: 2.1rem;
  height: 2.1rem;
  margin: 0 auto;
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
em,
i {
  font-style: normal;
}

.fixed-nav p {
  line-height: 1.7rem;
  height: 1.7rem;
}

.fixed-nav a {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
  font-size: 1.1rem;
  color: #333;
}
.col {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
}
a {
  color: inherit;
}
a {
  text-decoration: none;
  color: #333;
}

.fixed-nav a.active .icon-my {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAABEVBMVEUAAAChlveckfeVifSWivWWivWajvWVifSVifSdkfennPiWifSglfeVifS1rPuWivSWivWWivSZjfWek/a1rPuVifSVifShlveVifSbkPakmfi2rfuupPq2rfunnPiVifS2rPuekvakmviyqfu1rPu2rfuwpvqbkPWil/erofm2rfuxp/qVifSjmPeVifSzqvu0q/uqn/iglPaXjPWWi/S2rfuvpfqonviajvWsovmVifSckfaVifSbkPWckfawpvq2rfuzqvqVifS1rPukmfeflPaxp/qckPazqvqmnPivpPmhlvepnviso/n///+qoPn08/7d2f3DvPvAuPrt6/7V0Pz6+v/l4v3KxPvn5P3Uz/zn6584AAAAQnRSTlMACQL0WlEw7NBAOCQS/Oyyk2Aa7eHc1dC9urmkoZt/fHVkKSIU+vn5+PDVs5ePjHxvaVJKRfb04+DXxrGngHNaUUGAqQ4hAAAB40lEQVQ4y8XQZ1/qMBSA8SQdtIAMkS0y5Lq33r0tloq0guC49/t/EJMm2HqS6s9XPq9O6f+0JSi59U5zJ/fBcZyVVi9ZkWwfo37TifqYVkL8p7UTPi3nxGupaEcYWEe2f1c8tW1iyR55Uc/sEZI6dF2XS7B0KNvf7iKwtEvkU/00EhAs5fpIane0CCxtrEs27dO4hUurEl714zHqzVy+s5EFlmxfh938m3rcO5NgLl51DL+CW+8uCO7Z4LuTIAh8HvyO7jjshooJw6M5nf7TJdZXgNdimA0PdJhei7YB3r8Me8IzOsxHbGIaPpnjGcNsGN/S6X4sAvh4QKOG/q1bvjelekx/oX0G2B7w/IcZXeL6jq2xGgDjrYHcpWgNgRpXrIEyE+KTK5G8VEUwUr1gMQmXTpCUfbEIbDWQon3BwFJpWYVJfUiDeCuNlOHvwyhhSzZKiPzcHD6v2kPJmfU4Lf0iEABe+MLlZr2L0est24Z+2iPoXcuaZ0axqBvpDH75Y/XCt9R5VDnfPlNvZNrWuSItr0NPjFoMQL+XiVujEru3lKpYllXW4v5HxAvRO9unGYJ42NQL1tMTugu8FF6n9mwin02xxu9qSFSmF5UiTjqjA409ConMfE0nLx39gZYy0Ft7BF0l8pv1XL4PAAAAAElFTkSuQmCC);
}
// .fixed-nav .icon-my {
//   background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAAnFBMV…wdd7hdstkt23tEvF9fdlMWuWKxUFW33s8/Nb5Nwxy+qzcQeWeeTnn7fQAAAABJRU5ErkJggg==);
// }
.fixed-nav .icon {
  display: block;
  width: 2.1rem;
  height: 2.1rem;
  margin: 0 auto;
  background-repeat: no-repeat;
  background-size: 100% 100%;
}

em,
i {
  font-style: normal;
}

.fixed-nav p {
  line-height: 1.7rem;
  height: 1.7rem;
}
blockquote,
body,
button,
dd,
dl,
dt,
fieldset,
form,
h1,
h2,
h3,
h4,
h5,
h6,
hr,
input,
legend,
li,
ol,
p,
pre,
td,
textarea,
th,
ul {
  margin: 0;
  padding: 0;
  vertical-align: baseline;
}
</style>
