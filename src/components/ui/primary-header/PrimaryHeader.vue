<template>
    <header class="header wrapper">
        <div class="logo">
          <h1 class="logo__text"><a href="#">Taskoo</a></h1>
        </div>
        <nav class="header-nav">
          <ul class="header-nav__list">
            <li class="header-nav__item">
              <a href="#" class="header-nav__link">Solutions</a>
            </li>
            <li class="header-nav__item">
              <a href="#" class="header-nav__link">Product</a>
            </li>
            <li class="header-nav__item">
              <a href="#" class="header-nav__link">Resources</a>
            </li>
            <li class="header-nav__item">
              <a href="#" class="header-nav__link">Pricing</a>
            </li>
          </ul>
        </nav>
        <div class="auth">
          <a href="#" class="auth__link primary-btn primary-btn--link">Log In</a>
          <a href="#" class="auth__link primary-btn">Sign Up</a>
        </div>
    </header>
</template>

<style>
.header {
  padding: 15px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo__text {
  color: var(--clr-yellow-400);
  font-weight: 600;
  font-size: var(--fs-500);
}

.header-nav__list {
  display: flex;
  gap: 30px;
}

.header-nav__link {
    font-size: var(--fs-300);
}

.auth {
  display: flex;
  align-items: center;
  gap: 30px;
}
</style>