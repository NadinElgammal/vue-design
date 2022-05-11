<template>
    <header>
        
        <div class="lhs">
            <div class="logo">
            <img class="logo-img" src="../assets/—Pngtree—pinterest white icon_3570424.png">
            <span style="color:white">Picsart</span>
            </div>
            <div>
            <span class="nav-text"> Explore </span>
            </div>
        </div>
        <div class="rhs">
            <span class="num"> 555 </span>
            <img class="icon" src="https://upload.wikimedia.org/wikipedia/commons/6/60/Contact_vmc2015.png">
            <span class="name"> David Whipps </span>
            <img class="pro-img" src="https://www.opticalexpress.co.uk/media/1064/man-with-glasses-smiling-looking-into-distance.jpg"> 
        </div>
        
    </header>
</template>

<script>

export default{
    name:"Header",
}

</script>
<style scoped>
header{
    position: fixed;
    display: flex;
    justify-content: space-between;
    align-items: center;
    top: 0;
    left: 0;
    width: 100%;
    height: auto;
    z-index: 10;
}
header .lhs{
    display: flex;
    justify-content: start;
    align-items: center;
    gap: 50px;
    padding: 10px 20px;
}
header .lhs .logo{
    display: flex;
    justify-content: start;
    align-items: center;
    gap: 10px;

}
header .rhs{
    display: flex;
    /* justify-content: end; */
    align-items: center;
    gap:20px;
    padding: 10px 20px;
}
.logo-img{
    justify-content: flex-start;
    width:50px;
}
.nav-text{
    top:25px;
    left: 80px;
    color: white;
    text-decoration: underline;
}
.pro-img{
    border-radius: 50%;
    width: 45px;
    height: 50px;
}
.name{
    top:25px;
    color: white;
}
.icon{
    width: 35px;
    top: 12px;
}
.num{
    
    top:25px;
    color: white;
}


</style>