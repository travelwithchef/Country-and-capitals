<!DOCTYPE html>
<html>
<head>
  <title>Countries and Capitals</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      margin-top: 50px;
    }
    select, h2 {
      font-size: 20px;
      padding: 10px;
    }
    h1 {
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <h1>Select a Country</h1>
  <select id="countryList" onchange="showCapital()">
    <option value="">--Choose a country--</option>
    <option value="USA">USA</option>
    <option value="Canada">Canada</option>
    <option value="India">India</option>
    <option value="China">China</option>
    <option value="Japan">Japan</option>
    <option value="Germany">Germany</option>
    <option value="UK">United Kingdom</option>
    <option value="France">France</option>
    <option value="Italy">Italy</option>
    <option value="Russia">Russia</option>
    <option value="Brazil">Brazil</option>
    <option value="South Africa">South Africa</option>
    <option value="Mexico">Mexico</option>
    <option value="Australia">Australia</option>
    <option value="Spain">Spain</option>
    <option value="Saudi Arabia">Saudi Arabia</option>
    <option value="Argentina">Argentina</option>
    <option value="South Korea">South Korea</option>
    <option value="Turkey">Turkey</option>
    <option value="Egypt">Egypt</option>
    <option value="Thailand">Thailand</option>
    <option value="Sweden">Sweden</option>
    <option value="Norway">Norway</option>
    <option value="Denmark">Denmark</option>
    <option value="Finland">Finland</option>
    <option value="Poland">Poland</option>
    <option value="Netherlands">Netherlands</option>
    <option value="Belgium">Belgium</option>
    <option value="Austria">Austria</option>
    <option value="Switzerland">Switzerland</option>
    <option value="Chile">Chile</option>
    <option value="Peru">Peru</option>
    <option value="Pakistan">Pakistan</option>
    <option value="Bangladesh">Bangladesh</option>
    <option value="Nigeria">Nigeria</option>
    <option value="Ukraine">Ukraine</option>
    <option value="Iraq">Iraq</option>
    <option value="Malaysia">Malaysia</option>
    <option value="Israel">Israel</option>
    <option value="Vietnam">Vietnam</option>
    <option value="Singapore">Singapore</option>
    <option value="New Zealand">New Zealand</option>
    <option value="Czech Republic">Czech Republic</option>
    <option value="Greece">Greece</option>
    <option value="Romania">Romania</option>
  </select>
  
  <h2 id="capitalResult"></h2>

  <script>
    const capitals = {
      "USA": "Washington D.C.",
      "Canada": "Ottawa",
      "India": "New Delhi",
      "China": "Beijing",
      "Japan": "Tokyo",
      "Germany": "Berlin",
      "UK": "London",
      "France": "Paris",
      "Italy": "Rome",
      "Russia": "Moscow",
      "Brazil": "Brasília",
      "South Africa": "Pretoria",
      "Mexico": "Mexico City",
      "Australia": "Canberra",
      "Spain": "Madrid",
      "Saudi Arabia": "Riyadh",
      "Argentina": "Buenos Aires",
      "South Korea": "Seoul",
      "Turkey": "Ankara",
      "Egypt": "Cairo",
      "Thailand": "Bangkok",
      "Sweden": "Stockholm",
      "Norway": "Oslo",
      "Denmark": "Copenhagen",
      "Finland": "Helsinki",
      "Poland": "Warsaw",
      "Netherlands": "Amsterdam",
      "Belgium": "Brussels",
      "Austria": "Vienna",
      "Switzerland": "Bern",
      "Chile": "Santiago",
      "Peru": "Lima",
      "Pakistan": "Islamabad",
      "Bangladesh": "Dhaka",
      "Nigeria": "Abuja",
      "Ukraine": "Kyiv",
      "Iraq": "Baghdad",
      "Malaysia": "Kuala Lumpur",
      "Israel": "Jerusalem",
      "Vietnam": "Hanoi",
      "Singapore": "Singapore",
      "New Zealand": "Wellington",
      "Czech Republic": "Prague",
      "Greece": "Athens",
      "Romania": "Bucharest"
    };

    function showCapital() {
      const country = document.getElementById("countryList").value;
      const capital = capitals[country];
      if (capital) {
        document.getElementById("capitalResult").innerText = `The capital of ${country} is ${capital}.`;
      } else {
        document.getElementById("capitalResult").innerText = "";
      }
    }
  </script>
</body>
</html>
