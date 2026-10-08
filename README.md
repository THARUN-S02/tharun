<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>College Placement Tracker</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background-color: #f3f6fb;
      color: #253047;
    }

    nav {
      background-color: #123c69;
      color: white;
      padding: 15px 7%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    nav h2 {
      margin: 5px 0;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 8px;
    }

    nav a:hover {
      color: #ffd166;
    }

    .banner {
      min-height: 280px;
      padding: 50px 8%;
      color: white;
      background:
        linear-gradient(rgba(10, 35, 70, 0.75), rgba(10, 35, 70, 0.75)),
        url("https://images.unsplash.com/photo-1523050854058-8df90110c9f1?auto=format&fit=crop&w=1400&q=80")
        center/cover;
    }

    .banner h1 {
      margin-bottom: 12px;
      font-size: 38px;
    }

    .announcement {
      background-color: #ffd166;
      padding: 12px;
      color: #222;
      font-weight: bold;
    }

    .container {
      width: 86%;
      margin: 30px auto;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 18px;
      margin: 25px 0;
    }

    .stat-card,
    .company-card,
    .table-box {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 3px 12px #00000012;
    }

    .stat-card h3 {
      color: #123c69;
      margin-bottom: 8px;
    }

    .stat-number {
      color: #e76f51;
      font-size: 28px;
      font-weight: bold;
    }

    .company-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 18px;
      margin: 18px 0 30px;
    }

    .company-card img {
      width: 55px;
      height: 55px;
      object-fit: contain;
      margin-bottom: 10px;
    }

    .company-card h3 {
      color: #123c69;
      margin-bottom: 6px;
    }

    .table-box {
      overflow-x: auto;
      margin: 18px 0 30px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      min-width: 600px;
    }

    th, td {
      text-align: left;
      padding: 12px;
      border-bottom: 1px solid #ddd;
    }

    th {
      background-color: #123c69;
      color: white;
    }

    .status {
      color: #16803c;
      font-weight: bold;
    }

    footer {
      text-align: center;
      padding: 18px;
      background-color: #123c69;
      color: white;
      margin-top: 35px;
    }

    @media (max-width: 600px) {
      nav {
        display: block;
        text-align: center;
      }

      .banner h1 {
        font-size: 30px;
      }
    }
  </style>
</head>

<body>

  <nav>
    <h2>ABC College</h2>
    <div>
      <a href="#home">Home</a>
      <a href="#statistics">Statistics</a>
      <a href="#companies">Companies</a>
      <a href="#students">Students</a>
    </div>
  </nav>

  <div class="announcement">
    <marquee>
      Placement Update: New job opportunities are available for final-year students.
      Check the eligibility criteria and application deadlines!
    </marquee>
  </div>

  <div class="banner" id="home">
    <h1>College Placement Tracker</h1>
    <p>Track placement statistics, recruiting companies, and student selections.</p>
  </div>

  <div class="container" id="statistics">
    <h2>Placement Overview</h2>

    <div class="stats">
      <div class="stat-card">
        <h3>Registered Students</h3>
        <div class="stat-number">420</div>
      </div>

      <div class="stat-card">
        <h3>Students Placed</h3>
        <div class="stat-number">286</div>
      </div>

      <div class="stat-card">
        <h3>Companies Visited</h3>
        <div class="stat-number">38</div>
      </div>

      <div class="stat-card">
        <h3>Highest Package</h3>
        <div class="stat-number">₹18 LPA</div>
      </div>
    </div>

    <h2 id="companies">Top Recruiting Companies</h2>

    <div class="company-list">
      <div class="company-card">
        <img src="https://placehold.co/60x60?text=TCS" alt="TCS logo">
        <h3>Tata Consultancy Services</h3>
        <p>Students selected: 54</p>
        <p>Role: Graduate Trainee</p>
      </div>

      <div class="company-card">
        <img src="https://placehold.co/60x60?text=INFY" alt="Infosys logo">
        <h3>Infosys</h3>
        <p>Students selected: 42</p>
        <p>Role: Systems Engineer</p>
      </div>

      <div class="company-card">
        <img src="https://placehold.co/60x60?text=ACC" alt="Accenture logo">
        <h3>Accenture</h3>
        <p>Students selected: 31</p>
        <p>Role: Associate Developer</p>
      </div>
    </div>

    <h2 id="students">Recent Student Placements</h2>

    <div class="table-box">
      <table>
        <thead>
          <tr>
            <th>Student Name</th>
            <th>Department</th>
            <th>Company</th>
            <th>Package</th>
            <th>Status</th>
          </tr>
        </thead>

        <tbody>
          <tr>
            <td>Ananya Sharma</td>
            <td>Computer Science</td>
            <td>Infosys</td>
            <td>₹6 LPA</td>
            <td class="status">Selected</td>
          </tr>
          <tr>
            <td>Rahul Kumar</td>
            <td>Information Technology</td>
            <td>TCS</td>
            <td>₹5.5 LPA</td>
            <td class="status">Selected</td>
          </tr>
          <tr>
            <td>Meera Patel</td>
            <td>Electronics</td>
            <td>Accenture</td>
            <td>₹4.8 LPA</td>
            <td class="status">Selected</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>

  <footer>
    <p>© 2026 ABC College | Training and Placement Cell</p>
  </footer>

</body>
</html>
