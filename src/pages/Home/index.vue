<template>
  <header id="header-home-page" class="header-container content-center">
    <div class="top-advertisement-campaign content-center flex justify-between px-5 relative"> 
      <span class="text-right ml-5"></span>
      <span class="text-center justify-center text-slate-100 title-top-campaign">
        Introductory Offer Get Upto 50% Off.
        <a href="" class="text-indigo-600 underline-offset-1 ml-2 buy-now-text"> Buy Now</a>
      </span>

      <span class="text-right mr-5 close-campain">
        <label for="check-close-campain" class="remove-banner">✕</label>
        <input type="checkbox" name="close-campain" id="check-close-campain">
      </span>
    </div>

    <div class="tab-menu-bar py-4 content-center justify-center flex ">
      <div class="tab-container w-3/5 h-full flex rounded-lg px-5 py-2 justify-between items-center justify-center flex">
        <a href="#" class="h-3/5 flex">
          <img src="/assets/img/logo.png" alt="Logo" class="h-full">
        </a>

        <ul class="tab-menu-container">
          <li><a href="#">Home</a></li>
          <li><a href="#">Home</a></li>
          <li><a href="#">Home</a></li>
          <li><a href="#">Home</a></li>
        </ul>

        <div class="h-4/5 rounded-md w-1/6 btn-login bg-indigo-500 text-white flex-center ">Search</div>
      </div>
    </div>
  </header>

  <!-- Body of Page -->
  <main></main>

  <!-- Footer of Page -->
  <footer></footer>
</template>

<script>
export default {
    name: 'HomePage'
}
</script>

<style scoped>
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}

html , body {
  background-color: var(--white);
  font-family: 'DM Sans'
}

.header-container {
  height: auto;
  /* box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px; */
}

.top-advertisement-campaign:not(.close-campaign) {
  background-image: url(https://raw.githubusercontent.com/tandat1508/ZuneXPhone.io/master/assets/img/banner.png);
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  padding: 8px 0px;
  height: 40px;
  transition: margin-top 0.5s ease-in;
  margin-top: 0px;
}

.top-advertisement-campaign:has(input[name="close-campain"]:checked) {
  margin-top: -40px;
}


.title-top-campaign {
  font-size: 15px;
}

.buy-now-text {
  transition: all 0.2s ease-in;
  -o-transition: all 0.2s ease-in;
  -webkit-transition: all 0.2s ease-in;
}
.buy-now-text:hover {
  color: rgb(220 38 38);
}

.close-campain {
  color: white;
  transform: rotate(90deg);
  transition: 0.3s;
}

.close-campain label {
  cursor: pointer;
}
.close-campain:hover {
  transform: rotate(0deg);
}

#check-close-campain {
  display: none;
}

.tab-menu-bar {
  height : 110px
}

.tab-container {
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

.btn-login {
  max-width: 140px;
  transition: transform .5s cubic-bezier(0.165, 0.84, 0.44, 1);
  font-size: 14px;
  cursor: pointer;
}

.btn-login:hover {
  transform: scale(1.1);
  font-size: 14px;
}

.tab-menu-container {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  display: flex;
  column-gap: 5rem;
}

.tab-menu-container li {
  float: left;
}

.flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>