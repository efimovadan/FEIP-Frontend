<template>
    <header class="header">
        <img src="~/assets/img/logo.png" alt="logo" class="header-logo"/>
        <img src="~/assets/img/zagdom.png" alt="zagdom"/>
        <nav class="menu">
            <ul class="menu-list">
            <li class="list-element"><a href="" class="element">Реализованные проекты</a></li>
            <li class="list-element"><a href="" class="element">Новости</a></li>
            <li class="list-element"><a href="" class="element">Контакты</a></li>
            </ul>
        </nav>
        <div class="contacts">
            <img src="~/assets/img/telephone.png" alt="telephone" class="telephone"/>
            <a class="number">+7 (900) 900-90-90</a>
            <button class="button">Оставить заявку</button>
        </div>
    </header>
</template>

<style lang='scss'>

.header {
    padding-left: 88px;
    height: 97px;
    background-color: #FFFFFF;
    display: flex;
    align-items: center;
}
.log-menu {
    gap: 80px;
}
.header-logo {
    margin-right: 9.67px;
}
.menu-list {
    list-style-type: none;
    display: flex;
    align-items: center;  
}
.list-element {
    margin-right: 24px;
}
.element {
    color: #666666;
    font-family: var(--font-title);
}
.telephone {
    padding-left: 254px;
    padding-right: 8px;
}
.number {
    font-family: var(--font-text);
    padding-right: 24px;
}
.button {
    height: 49px;
    width: 204px;
    border-radius: 10px;
    border-color: #029F59;
    background: #029F59;
    color: #FFFFFF;
    font-family: var(--font-text);
}
.contacts {
    /* padding-right: 88px; */
    float: right;
    margin-left: auto;
    padding-right: 88px;
}
</style>