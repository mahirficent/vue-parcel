<template>
    <div class="body">
      <div class="header">
        <h1>Parcel Information (Without Login)</h1>
      </div>

      <div class="main-container">
            <div class="container">
                <div class="sub-container">
                    <h2>Product Info:</h2>
                </div>
        
                <listOfData />
            </div>

        </div>
  
    </div>
  </template>
  
  <script>
  import listOfData from "@/components/content.vue";
  
  export default {
    components: {
      listOfData,
    },
  };
  </script>

<style scoped>
.header {
  text-align: center;
}

.header h1 {
  font-size: 32px;
  margin: 0;
  color: #0B395A;
}

.container {
  border: 2px solid #ddd;
  padding: 20px;
  justify-content: center;
}

.sub-container {
  margin-bottom: 20px;
}

.body {
  display: flex;
  flex-direction: column;
  align-items: center; 
  height: 100vh;
}

.main-container {
  width: 100%; 
  display: flex;
  justify-content: center;
  align-items: center;
  height: 75vh;
  margin: 0;
}

h2 {
  font-size: 24px;
  margin: 0;
  color: #0B395A;
  text-align: left;
}

.list-of-data {
  max-width: 90%;
  margin: 0 auto;
  overflow-x: auto;
}
</style>
  