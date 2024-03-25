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
                    <li class="list-element-footer"><span href="" class="element-footer">Реализованные проекты</span></li>
                    <li class="list-element-footer"><span href="" class="element-footer">Новости</span></li>
                    <li class="list-element-footer"><span href="" class="element-footer">Контакты</span></li>
                </ul>
                
            
            </div>
            <div class="nav-footer">
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
    margin-right: 176px;
}
.nav-img {
    margin-right: 8px;
}
.nav-footer {
    margin-right: 154px;
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
}
.zagdom-footer-left {
    margin-right: 154px;
    display: flex;
    flex-direction: column;
}
.zagdom-footer-links {
    color: #FFFFFF;
    font-family: var(--font-title);
    font-weight: 400;
    opacity: 60%;
}
.zag {
    margin-right: 205px;
}
.zag-pol {
    margin-right: 99px;
}
.footer {
    padding-left: 88px;
    padding-top: 36.98px;
    margin: 0;
    background-color:#254741;
    position: fixed;
    bottom: 0;
    width: 100%;
    z-index: 1000; 
    height: 246px;
}

.list-element-footer {
    margin-bottom: 24px;
}
.element-footer {
    color: #FFFFFF;
    font-family: var(--font-title);  
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