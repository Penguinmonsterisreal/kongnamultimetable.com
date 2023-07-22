<!DOCTYPE html>
<html>
<head>
    <title>Time Table</title>
    <style>
         font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      background-image: url("Skyblue_Monster.jpg");
      background-size: cover;
      background-position: center;
        table {
            border-collapse: collapse;
            width: 100%;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        td {
            background-color: #ffffff;
        }
        h1 {
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="table-container">
    <h1>Time Table</h1>
    <table>
        <tr>
            <th>/</th>
            <th>Monday</th>
            <th>Tuesday</th>
            <th>Wednesday</th>
            <th>Thursday</th>
            <th>Friday</th>
        </tr>
        <tr>
            <td>12:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>13:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>13:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>14:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>14:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>15:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>15:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>16:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>16:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>17:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>17:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>18:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>18:30</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
        <tr>
            <td>19:00</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
            <td onclick="editCell(this)">Edit</td>
        </tr>
    </table>
</div>
    <script>
        function editCell(cell) {
            var text = prompt("Enter the text:");
            if (text !== null) {
                cell.innerText = text;
                changeColor(cell);
            }
        }

        function changeColor(cell) {
            var color = prompt("Enter the color (red, orange, yellow, green, blue, indigo, violet):");
            if (color !== null) {
                var validColors = ["red", "orange", "yellow", "green", "blue", "indigo", "violet"];
                if (validColors.includes(color.toLowerCase())) {
                    cell.style.backgroundColor = color.toLowerCase();
                } else {
                    alert("Invalid color! Please choose a color from the rainbow.");
                }
            }
        }
    </script>
</body>
</html>
