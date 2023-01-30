# Bike-service
<!DOCTYPE html>
<html>
  <head>
    <title>Bike Care</title>
  </head>
  <body>
    <h1>Bike Service</h1>
    <form action="">
      <label for="employee_name">customer Name:</label>
      <input type="text" id="employee_name" name="employee_name"><br><br>
      <label for="position">Problem:</label>
      <input type="text" id="position" name="position"><br><br>
      <label for="salary">cost:</label>
      <input type="text" id="salary" name="salary"><br><br>
      <input type="submit" value="Submit">
    </form>
    <br>
    <table border="1">
      <tr>
        <th>Customer Name</th>
        <th>Problem</th>
        <th>cost</th>
      </tr>
      <tr>
        <td id="table_employee_name"></td>
        <td id="table_position"></td>
        <td id="table_salary"></td>
      </tr>
    </table>
    <script>
      document.querySelector('form').addEventListener('submit', function(event) {
        event.preventDefault();
        document.querySelector('#table_employee_name').innerHTML = document.querySelector('#employee_name').value;
        document.querySelector('#table_position').innerHTML = document.querySelector('#position').value;
        document.querySelector('#table_salary').innerHTML = document.querySelector('#salary').value;
      });
    </script>
  </body>
</html>
