<template>
    <footer class="footer">
        <button class="button-footer">Оставить заявку</button>
        <div class="footer-up">
            <div class="zagdom-footer-left">
                <div class="images">
                    <img src="~/assets/img/logo_white.png" alt="logo-white" class="footer-logo"/>
                    <img src="~/assets/img/zagdom_white.png" alt="zagdom-white" class="zagdom"/>
                </div>
                
            </div>
            <div class="nav-footer">
                <ul class="menu-list-footer">
                    <li class="list-element-footer"><a href="" class="element-footer">Реализованные проекты</a></li>
                    <li class="list-element-footer"><a href="" class="element-footer">Новости</a></li>
                    <li class="list-element-footer"><a href="" class="element-footer">Контакты</a></li>
                </ul>
            </div>
            <div class="nav-footer1">
                <ul class="menu-list-footer">
                    <li class="list-element-footer">
                    <img src="~/assets/img/telephone.png" alt="telephone" class="nav-img"/>
                    <span class="element-footer">+7 (900) 900-90-90</span>
                    </li>
                    <li class="list-element-footer">
                    <img src="~/assets/img/email.png" alt="email" class="nav-img"/>
                    <span class="element-footer">info@gmail.com</span>
                    </li>
                    <li class="list-element-footer">
                    <img src="~/assets/img/placeholder.png" alt="placeholder" class="nav-img"/>
                    <span class="element-footer">г. Владивосток ул. Выселковая 49, стр. 3</span>
                    </li>
                </ul>   
            </div>
        </div>
        <div class="zagdom-footer-links">
            <a class="zag">© Загдом, 2021</a>
            <a class="zag-pol">Политика конфиденциальности</a>
            <a class="zag-user">Пользовательское соглашение</a>
        </div>
    </footer>
</template>

<style lang='scss'>
@mixin for-phone-only {
  @media (max-width: 350px) { @content; }
}
@mixin for-tablet-portrait-up {
  @media (max-width: 600px) { @content; }
}
@mixin for-tablet-landscape-up {
  @media (max-width: 900px) { @content; }
}
@mixin for-telephone {
  @media (max-width: 1070px) { @content; }
}
@mixin for-desktop-up {
  @media (max-width: 1200px) { @content; }
}
@mixin for-big-desktop-up {
  @media (max-width: 1800px) { @content; }
}

.button-footer {
    height: 49px;
    width: 204px;
    border-radius: 10px;
    border-color: #029F59;
    background: #029F59;
    color: #FFFFFF;
    font-family: var(--font-text);
    float: right;
    margin-left: auto;
    margin-right: 87.5px;
    margin-left: auto;

    @include for-telephone {
        margin-left: 0;
    }
}
.nav-img {
    margin-right: 8px;
}
.nav-footer {
    margin-right: 154px;
    @include for-desktop-up {
        margin-right: 90px;
    }
}

.nav-footer1 {
    @include for-desktop-up {
        margin-right: 90px;
    }
}
.footer-contacts {
    padding-left: 122px;
    color: #FFFFFF;
    font-family: var(--font-text);
    padding:0;
    list-style-type: none;
    display: flex;
    flex-direction: column;
}
.footer-up {   
    display: flex;
    flex-direction: row;
    order: -1;
    @include for-telephone {
        display: flex;
        flex-direction: column;
    }
}
.zagdom-footer-left {
    margin-right: 154px;
    display: flex;
    flex-direction: column;
    @include for-desktop-up {
        margin-right: 90px;
    }
}
.zagdom-footer-links {
    color: #FFFFFF;
    font-family: var(--font-title);
    font-weight: 400;
    opacity: 60%;

    @include for-telephone {
        display: flex;
        flex-direction: column;
        gap: 24px;
        margin-bottom: 20px;
    }
}
.zag {
    margin-right: 205px;
    @include for-desktop-up {
        margin-right: 90px;
    }
}
.zag-pol {
    margin-right: 99px;
}
.footer {
    padding-left: 88px;
    padding-top: 37px;
    margin: 0;
    background-color:#254741;
    min-height: 246px;

    @include for-telephone {
        display: flex;
        flex-direction: column;
        gap: 24px;
    }
}

.list-element-footer {
    margin-bottom: 24px;
}
.element-footer {
    color: #FFFFFF;
    font-family: var(--font-title);  
    text-decoration: none;
}
.footer-logo {
    margin-right: 9.67px;
}

.menu-list-footer {
    padding:0;
    list-style-type: none;
    display: flex;
    flex-direction: column;
}
</style>