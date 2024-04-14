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
.header {
    padding-left: 88px;
    height: 97px;
    background-color: #FFFFFF;
    display: flex;
    align-items: center;

    @include for-phone-only {
        padding-left: 16px;
    }

    @include for-tablet-portrait-up {
        padding-left: 32px;
    }

    @include for-tablet-landscape-up {
        padding-left: 64px;
    }

    @include for-desktop-up {
        padding-left: 88px;
    }
    @include for-telephone  {
        padding-left: 16px;
    }
}

.menu {
    @include for-phone-only {
        display: none;
    }

    @include for-tablet-portrait-up {
        display: flex;
    }
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
    @include for-tablet-landscape-up {
        flex-wrap: wrap;
    }
    @include for-telephone  {
        display: none;
    }

    @include for-desktop-up   {
        flex-wrap: wrap;
    }
    
}
.list-element {
    margin-right: 24px;
}
.element {
    color: #666666;
    font-family: var(--font-title);
}
.telephone {
    padding-right: 8px;
    @include for-tablet-landscape-up {
        display: none;
    }
}
.number {
    font-family: var(--font-text);
    padding-right: 24px;
    width: 158px;
    @include for-tablet-landscape-up {
        display: none;
    }
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
    // float: right;
    display: flex;
    align-items: center;
    margin-left: auto;
    padding-right: 88px;
    @include for-telephone  {
        padding-right: 16px;
    }


}

// @media screen and (max-width: 350){ 
//     .header {
//         padding-left: 16px;
//     }
//     .menu {
//         display: none;
//     }
// }


</style>