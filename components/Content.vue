<template>
    <div class="content">
        <div class="banner">
            Banner
        </div>
        <h1 class="hello">Hello, world!</h1>
        <p class="look">Look at my website</p>
        <div class="cards">
            <div class="card">Here</div>
            <div class="card">And here</div>
        </div>
    </div>
</template>


<style lang="scss">

@mixin card($color: white, $width: 100%, $height: 100%) {
  background: $color;
  width: $width;
  height: $height;
  padding: 5px 5px 5px 10px;
  font-family: var(--font-title);
}


.look {
    color: black;
    font-size: 25px;
}
.hello {
    font-family: var(--font-title);
    font-weight: bold;
}
.content{
    margin-left: 25%;
    margin-top: 20px;
    margin-bottom: 20px;
}
.banner {
    @include card(rgb(0, 156, 0), 50%, 50%);
    color: white;
    
    font-weight: 50;
    font-size: 1.5rem;
}

.card {
  @include card(rgb(213,253,209), 110px, 25px);
  margin-right:20px;
  font-size: 1.1rem;
}

.cards {
    display: flex;
}
</style>