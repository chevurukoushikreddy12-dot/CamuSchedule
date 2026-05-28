# Ex08 CAMU Schedule using Bootstrap
## Date:28-05-2026

## AIM:
To design a responsive and visually appealing CAMU Schedule using Bootstrap.

## DESIGN STEPS:
### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Add the Bootstrap CDN link inside the <head> section.

### Step 5:
Insert a table element with Bootstrap table classes.

### Step 6:
Construct the complete table.

### Step 7:
Add a header/footer displaying copyright information.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Modern CAMU Schedule</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <!-- Bootstrap Icons -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family:'Poppins',sans-serif;
      background: linear-gradient(135deg,#0f172a,#1e3a8a,#2563eb);
      min-height:100vh;
      color:white;
    }

    .main-container{
      padding:40px 15px;
    }

    .header{
      background: rgba(255,255,255,0.12);
      backdrop-filter: blur(10px);
      border:1px solid rgba(255,255,255,0.2);
      border-radius:25px;
      padding:35px;
      text-align:center;
      margin-bottom:40px;
      box-shadow:0 8px 25px rgba(0,0,0,0.3);
    }

    .header h1{
      font-size:3rem;
      font-weight:700;
      letter-spacing:2px;
    }

    .header p{
      font-size:1.1rem;
      color:#dbeafe;
      margin-top:10px;
    }

    .student-box{
      margin-top:20px;
      display:inline-block;
      background:rgba(255,255,255,0.15);
      padding:15px 30px;
      border-radius:15px;
      border:1px solid rgba(255,255,255,0.2);
    }

    .student-box h5,
    .student-box h6{
      margin:5px 0;
    }

    .schedule-card{
      background: rgba(255,255,255,0.12);
      backdrop-filter: blur(12px);
      border:1px solid rgba(255,255,255,0.2);
      border-radius:25px;
      padding:25px;
      color:white;
      transition:0.4s;
      height:100%;
      box-shadow:0 8px 20px rgba(0,0,0,0.2);
    }

    .schedule-card:hover{
      transform:translateY(-10px) scale(1.02);
      box-shadow:0 12px 30px rgba(0,0,0,0.4);
    }

    .day-title{
      font-size:1.7rem;
      font-weight:600;
      margin-bottom:20px;
      text-align:center;
    }

    .schedule-item{
      background:rgba(255,255,255,0.1);
      padding:12px;
      border-radius:12px;
      margin-bottom:12px;
      transition:0.3s;
    }

    .schedule-item:hover{
      background:rgba(255,255,255,0.2);
    }

    .time{
      color:#93c5fd;
      font-weight:600;
      display:block;
      margin-bottom:5px;
    }

    .subject{
      font-size:0.95rem;
      font-weight:500;
    }

    .icon{
      margin-right:8px;
      color:#facc15;
    }

    .footer{
      text-align:center;
      margin-top:40px;
      padding:20px;
      background:rgba(255,255,255,0.12);
      border-radius:20px;
      backdrop-filter:blur(10px);
      border:1px solid rgba(255,255,255,0.2);
    }

    @media(max-width:768px){

      .header h1{
        font-size:2.2rem;
      }

      .schedule-card{
        padding:20px;
      }

    }

  </style>
</head>

<body>

<div class="container main-container">

  <!-- Header -->
  <div class="header">
    <h1><i class="bi bi-calendar-week"></i> CAMU Schedule</h1>
    <p>Modern Responsive Timetable Using Bootstrap 5</p>

    <div class="student-box">
      <h5>NAME : CHEVURU KOUSHIK</h5>
      <h6>REFERENCE NO : 25014537</h6>
    </div>
  </div>

  <!-- Schedule Cards -->
  <div class="row g-4">

    <!-- Monday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-primary">Monday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>8:00 - 10:00 AM</span>
          <div class="subject">Fundamentals of Web Development</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>10:00 - 12:00 AM</span>
          <div class="subject">C Programming</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>1:00 - 3:00 PM</span>
          <div class="subject">Computer Networks</div>
        </div>

      </div>
    </div>

    <!-- Tuesday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-success">Tuesday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>8:00 - 10:00 AM</span>
          <div class="subject">Career Development Skills</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>10:00 - 12:00 AM</span>
          <div class="subject">Computer Networks</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>1:00 - 3:00 PM</span>
          <div class="subject">Computer Networks</div>
        </div>

      </div>
    </div>

    <!-- Wednesday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-danger">Wednesday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>8:00 - 10:00 AM</span>
          <div class="subject">Computer Networks</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>1:00 - 3:00 PM</span>
          <div class="subject">Mentor Meet</div>
        </div>

      </div>
    </div>

    <!-- Thursday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-warning">Thursday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>8:00 - 10:00 AM</span>
          <div class="subject">Fundamentals of Web Development</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>10:00 - 12:00 AM</span>
          <div class="subject">Fundamentals of Web Development</div>
        </div>

      </div>
    </div>

    <!-- Friday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-info">Friday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>8:00 - 10:00 AM</span>
          <div class="subject">Fundamentals of Web Development</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>1:00 - 3:00 PM</span>
          <div class="subject">Career Development Skills</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>3:00 - 4:30 PM</span>
          <div class="subject">C Programming</div>
        </div>

      </div>
    </div>

    <!-- Saturday -->
    <div class="col-md-6 col-lg-4">
      <div class="schedule-card">
        <div class="day-title text-secondary">Saturday</div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>10:00 - 12:00 AM</span>
          <div class="subject">C Programming</div>
        </div>

        <div class="schedule-item">
          <span class="time"><i class="bi bi-clock icon"></i>1:00 - 3:00 PM</span>
          <div class="subject">C Programming</div>
        </div>

      </div>
    </div>

  </div>

  <!-- Footer -->
  <div class="footer">
    <h5>Designed Using Bootstrap 5</h5>
    <p>Responsive | Modern UI | Glassmorphism Design</p>
  </div>

</div>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
```


## OUTPUT:
<img width="1284" height="996" alt="{C2000489-B746-4758-9CAC-F48854D3AC29}" src="https://github.com/user-attachments/assets/6835009f-a1d5-4bd0-b2e3-feb48677c201" />


## RESULT:
A responsive and visually appealing CAMU Schedule web page using Bootstrap is designed successfully.
