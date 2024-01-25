<template>
  <main>
    <h1 class="center-container"> Database</h1>
    <div class="center-container">
    <h1>
      <RouterLink to ='employees' class='item'>List Employees </RouterLink>
      <RouterLink to ='departments' class='item'>List Departments </RouterLink>
    </h1>
    </div>
  </main>
</template>



<style scoped>
.center-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.item {
  margin: 100px; /* Adjust margin as needed */
}
</style>