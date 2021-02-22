<template>
  <div class="col-12 row topbar bg-dark m-0 p-0">
    <div class="col-2 sidebar-header m-0 p-0">
      <div class="sidebar-header w-100">
        <div class="col-12 row d-flex align-items-center m-0 p-0">
          <div class="col-8 m-0 p-0">
            <h4 class="text-light mt-2">Heros</h4>
          </div>
          <div class="col-4 m-0 p-0 d-flex justify-content-center">
            <img
              style="width: 30px; height: 30px"
              src="../assets/logo.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
    <div class="col-2">
    </div>
    <div class="col-5 search-box float-left">
      <div class="col-12 row">
        <div class="col-12">
          <div class="col-12 m-0 p-1 row">
            <div class="col-8 p-0">
              <input class="form-control w-100" />
            </div>
            <div class="col-4 d-flex align-items-center">
              <button type="button" class="btn btn-secondary w-100">
                <i class="fas fa-search"></i> Search
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopBar'
}
</script>

<style scoped>
.sidebar-header {
  background-color: #7386d5
}
</style>
