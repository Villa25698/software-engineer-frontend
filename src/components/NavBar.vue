<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
      <!-- Logo -->
      <a class="navbar-brand col-lg-2" href="#">
        <img src="@/assets/logo.png" alt="MyWebsite" width="30" height="30" class="d-inline-block align-top">
        MyWebsite
      </a>

      <!-- Icons (without profile) -->
      <ul class="navbar-nav col-lg-6 d-flex justify-content-around">
        <li class="nav-item">
          <a class="nav-link" href="#">
            <img src="@/assets/home.svg" alt="Home" class="icon">
            <span class="d-none d-lg-inline">Home</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <img src="@/assets/about.svg" alt="About" class="icon">
            <span class="d-none d-lg-inline">About</span>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">
            <img src="@/assets/contact.svg" alt="Contact" class="icon">
            <span class="d-none d-lg-inline">Contact</span>
          </a>
        </li>
      </ul>

      <!-- Search Bar -->
      <form class="form-inline col-lg-3">
        <div class="d-flex w-100">
          <input class="form-control mr-2 flex-grow-1" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </div>
      </form>

      <!-- Profile Icon -->
      <div class="col-lg-1 d-flex justify-content-end">
        <div class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" id="accountDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            <img src="@/assets/account.svg" alt="Account" class="icon">
            <span class="d-none d-lg-inline">Profile</span>
          </a>
          <div class="dropdown-menu dropdown-menu-right" aria-labelledby="accountDropdown">
            <a class="dropdown-item" href="#">Profile</a>
            <a class="dropdown-item" href="#">Settings</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Logout</a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<style scoped>
.icon {
  width: 24px;
  height: 24px;
  fill: white;
}

.icon + .d-none.d-lg-inline {
  margin-left: 5px;
}

.form-inline .form-control {
  flex: 1;
}
</style>
