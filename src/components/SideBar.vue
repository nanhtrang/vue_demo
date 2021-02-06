<template>
  <div class="wrapper position-absolute" id="sidebar-div">
    <!-- Sidebar -->
    <nav id="sidebar">
      <div class="sidebar-header">
        <div class="col-12 row d-flex align-items-center">
          <div class="col-4 m-0 p-0">
            <h4 class="text-light mt-2">Heros</h4>
          </div>
          <div class="col-4 m-0 p-0 d-flex justify-content-start">
            <img
              style="width: 30px; height: 30px"
              src="../assets/logo.png"
              alt=""
            />
          </div>
        </div>
      </div>

      <ul class="list-unstyled components pt-0">
        <li>
          <a
            href="#homeSubmenu"
            data-toggle="collapse"
            aria-expanded="false"
            class="dropdown-toggle"
            >Tướng</a
          >
          <ul class="collapse list-unstyled" id="homeSubmenu">
            <li>
              <a href="#">Tất cả</a>
            </li>
            <li>
              <a href="#">Xạ thủ</a>
            </li>
            <li>
              <a href="#">Pháp sư</a>
            </li>
            <li>
              <a href="#">Đấu sĩ</a>
            </li>
            <li>
              <a href="#">Sát thủ</a>
            </li>
            <li>
              <a href="#">Trợ thủ</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">About</a>
        </li>
        <li>
          <a
            href="#pageSubmenu"
            data-toggle="collapse"
            aria-expanded="false"
            class="dropdown-toggle"
            >Pages</a
          >
          <ul class="collapse list-unstyled" id="pageSubmenu">
            <li>
              <a href="#">Page 1</a>
            </li>
            <li>
              <a href="#">Page 2</a>
            </li>
            <li>
              <a href="#">Page 3</a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">Portfolio</a>
        </li>
        <li>
          <a href="#">Contact</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'SideBar'
}
</script>

<style scoped>
#sidebar-div {
  top: 0px;
}
.wrapper {
  display: flex;
  width: 100%;
  align-items: stretch;
}
.wrapper {
  display: flex;
  align-items: stretch;
}

#sidebar {
  min-width: 250px;
  max-width: 250px;
}

#sidebar.active {
  margin-left: -250px;
}
#sidebar {
  min-width: 250px;
  max-width: 250px;
  min-height: 100vh;
}
a[data-toggle='collapse'] {
  position: relative;
}

.dropdown-toggle::after {
  display: block;
  position: absolute;
  top: 50%;
  right: 20px;
  transform: translateY(-50%);
}
@media (max-width: 768px) {
  #sidebar {
    margin-left: -250px;
  }
  #sidebar.active {
    margin-left: 0;
  }
}
@import 'https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700';
body {
  font-family: 'Poppins', sans-serif;
  background: #fafafa;
}

p {
  font-family: 'Poppins', sans-serif;
  font-size: 1.1em;
  font-weight: 300;
  line-height: 1.7em;
  color: #999;
}

a,
a:hover,
a:focus {
  color: inherit;
  text-decoration: none;
  transition: all 0.3s;
}

#sidebar {
  /* don't forget to add all the previously mentioned styles here too */
  background: #7386d5;
  color: #fff;
  transition: all 0.3s;
}

#sidebar .sidebar-header {
  padding: 20px;
  background: #6d7fcc;
}

#sidebar ul.components {
  padding: 20px 0;
  border-bottom: 1px solid #47748b;
}

#sidebar ul p {
  color: #fff;
  padding: 10px;
}

#sidebar ul li a {
  padding: 10px;
  font-size: 1.1em;
  display: block;
}
#sidebar ul li a:hover {
  color: #7386d5;
  background: #fff;
}

#sidebar ul li.active > a,
a[aria-expanded='true'] {
  color: #fff;
  background: #6d7fcc;
}
ul ul a {
  font-size: 0.9em !important;
  padding-left: 30px !important;
  background: #6d7fcc;
}
</style>
