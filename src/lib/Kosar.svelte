<script>
  export let termekek
  import cart from './cart.png';
</script>
<h1>
  <p>Kosár<img src={cart} alt="kosár"></p> 
  <table>
    <tr>
      <th>Termék neve</th>
      <th>Ára</th>
      <th>Mennyiség</th>
    </tr>
  {#each termekek as item}
    <tr>
      <td>{item.nev}</td>
      <td>{item.ar} Ft</td>
      <td><input id="db" type="number"> db</td>
    </tr>
      {/each}
    </table>
</h1>
<style>
  th, td{
    border: 1px solid black;
  }
  th{
    background-color: blue;
    color: white;
  }
  td{
    background-color: yellow;
    color: orange;
  }
  img{
    width: 50px;
    height: 50px;
  }
  table{
    border-collapse: collapse;
  }
  p{
    border: 1px solid rgb(130, 2, 2);
    box-shadow: 5px 5px 5px orangered;
    background-color: red;
    width: 200px;
    color: blue;
    border-radius: 10px;
  }
  #db{
    color: orange;
    width: 100px;
    height: 25px;
    margin-bottom: 10px;
  }

</style>