<template>
  <section>
    <ul>
      <li>
        <a href="https://www.facebook.com/search/top?q=skyplusagency">
          <i class="fab fa-facebook-f"></i>
        </a>
      </li>
      <li>
        <a href="https://www.instagram.com/skyplusagency/?hl=fr">
          <i class="fab fa-instagram"></i>
        </a>
      </li>
      <li>
        <a href="mailto:contact@skyplus.fr">
          <i class="far fa-envelope"></i>
        </a>
      </li>
      <li>
        <a href="tel:0695686899">
          <i class="fas fa-mobile"></i>
        </a>
      </li>

    </ul>
  </section>

</template>

<script>
export default {
  name: "ReseauSociaux"
}
</script>

<style scoped>

section {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 5em;
  padding: 0 0 5em 0;
}

ul {
  position: relative;
  display: flex;
  z-index: 2;
}

ul li {
  position: relative;
  list-style: none;
  margin: 10px;
}

ul li a {
  position: relative;
  width: 80px;
  height: 80px;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  color: #fff;
  font-size: 2em;
  border: 1px solid rgba(255, 255, 255, 0.4);
  border-right: 1px solid rgba(255, 255, 255, 0.2);
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
  box-shadow: 0 5px 45px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(2px);
  transition: 0.5s;
  overflow: hidden;
}

ul li a:hover {
  transform: translateY(-20px);
}

ul li a::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 50px;
  height: 100%;
  background: rgba(255, 255, 255, 0.5);
  transform: skewX(45deg) translateX(150px);
  transition: 0.5s;
}

ul li a:hover::before {
  transform: skewX(45deg) translateX(-150px);
}

/* Small devices (landscape phones, 340px and up) */
@media (min-width: 320px) and (max-width: 767px) {
  section{
    padding-bottom: 15em;
    width: 80%;
    margin: 5em auto;
}

  ul li {
      margin: 5px;
  }

  ul li a {
    width: 70px;
    height: 70px;
  }

  
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) and (max-width: 1023px) {

}

/* Large devices (desktops, 992px and up) */
@media (min-width: 1024px) and (max-width: 1279px) {
  section{
    margin-bottom: 19em;
  }
}

/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1280px) and (max-width: 1535px) {
  section{
    margin-bottom: 21em;
  }
}

@media (min-width: 1536px) {
  section{
    margin-bottom: 23em;
}
}
</style>
