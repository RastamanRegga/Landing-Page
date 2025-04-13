<template>
  <div>
    <header>
      <a href="#home" class="logo">Regga</a>
      <nav>
        <a href="#home" class="active">Home</a>
        <a href="#about">About Me</a>
        <a href="#Project">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>
  </div>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 1rem 9%;
  background-color: #dfd9ca;
  backdrop-filter: blur(45px);
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 999;
}

nav a {
  font-size: 1.8rem;
  color: #48A6A7;
  margin-left: 4rem;
  font-weight: 500;
  transition: 0.3s ease;
  border-bottom: 3px solid transparent;
}

nav a:hover,
nav a:active {
  color: #006A71;
  border-bottom: 3px solid #006A71;
}

@media(max-width:995px) {
  nav {
    position: absolute;
    top: 100%;
    right: 0;
    width: 40%;
    border-left: 3px solid #006A71;
    border-bottom: 3px solid #006A71;
    border-bottom-left-radius: 2 rem;
    padding: 1rem solid;
    background-color: #F2EFE7;
    border-top: 0.1rem solid #9ACBD0;
  }

  nav.active {
    display: block;
  }

  nav a {
    display: block;
    font-size: 2rem;
    margin: 3rem 0;
  }

  nav a:hover,
  nav a.active {
    padding: 1rem;
    border-radius: 0.5rem;
    border-bottom: 0.5rem solid #006A71;
  }
}
</style>