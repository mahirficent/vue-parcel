<template>
    <div class="content-container">
      <table>
        <tbody>
          <tr>
            <th v-for="item in items" :key="item.id">{{ item.name }}</th>
          </tr>
          <tr>
            <td v-for="item in items" :key="item.id">{{ item.value }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          { id: 1, name: 'Product ID', value: '123456' },
          { id: 2, name: 'Product Name', value: 'Example Product' },
          { id: 3, name: 'Product Quantity', value: '10' },
          { id: 4, name: 'Product Picture', value: 'product-image.jpg' },
          { id: 5, name: 'Dispatch Date', value: '01/01/2024' },
          { id: 6, name: 'Estimated Delivery Date', value: '01/01/2024' },
          { id: 7, name: 'Price', value: '100' },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .content-container {
    margin: 0 auto;
    overflow-x: auto;
    justify-content: center;
  }
  
  table {
    width: 100%;
    border-collapse: collapse;
  }
  
  th, td {
    font-size: 16px;
    border: 1px solid #ddd;
    padding: 8px;
    text-align: center;
    color: #35495e;
  }
  
  th {
    background-color: #f2f2f2;
  }
  </style>
  