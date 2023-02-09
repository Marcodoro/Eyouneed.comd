<template>
<div class="wrappeer">
    <div class="line"></div>
    <div class="line2"></div>
    <div class="line3"></div>
    <div class="line4"></div>
</div>

</template>

<script>

export default {
    name: 'Hamburger',
}
</script>

<style scoped>
.line {
    width: 40px;
    height: 5px;
    background-color: #ffffff;
    border-radius: 55px;
}
.line2 {
    content: '';
    width: 33px;
    height: 5px;
    background-color: #ffffff;
    border-radius: 55px;
}
.line3{
    content: '';
    width: 25px;
    height: 5px;
    background-color: #ffffff;
    border-radius: 55px;
}
.line4{
    content: '';
    width: 17px;
    height: 5px;
    background-color: #ffffff;
    border-radius: 55px;
}
.wrappeer {
    display: flex;
    flex-direction: column;
    gap: 4px;
    margin: 3px 7px;
    justify-content: left;
}
@media only screen and (min-width: 1024px) {
    .wrappeer {
        margin: 6px -65%;
    }
}
@media only screen and (min-width: 1440px) {
    .wrappeer {
       margin: 6px -70%;
    }
}
@media only screen and (min-width: 720px) {
    .wrappeer {
        margin: 6px -30%;
    }
}
</style>