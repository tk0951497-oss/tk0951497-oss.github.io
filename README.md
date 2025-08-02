<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>25-Day Hardcore Transformation Calendar</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background-color: #f0f0f0;
    }
    h1 {
      text-align: center;
    }
    .calendar {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 10px;
      margin-top: 20px;
    }
    .day {
      background-color: #fff;
      padding: 15px;
      border-radius: 8px;
      cursor: pointer;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      transition: 0.2s;
    }
    .day:hover {
      background-color: #e0ffe0;
    }
    .details {
      margin-top: 10px;
      display: none;
    }
    .active .details {
      display: block;
    }
    .rest-day {
      background-color: #ffe0e0;
    }
  </style>
</head>
<body>
  <h1>25-Day Hardcore Home Transformation</h1>
  <div class="calendar" id="calendar"></div>

  <script>
    const startDate = new Date("2025-08-03");
    const days = 25;
    const calendar = document.getElementById("calendar");

    const upperBodyPlan = `
      <strong>Upper Body + Core:</strong><br>
      1. Pull-Ups – 4 x Max Reps<br>
      2. Diamond Push-Ups – 4 x 15-20<br>
      3. Pike Push-Ups – 3 x 12<br>
      4. Superman Holds – 3 x 30s<br>
      5. Plank-to-Push-Up – 3 x 10<br>
      <em>Core Finisher:</em><br>
      Hanging Leg Raises, Russian Twists, Side Plank
    `;

    const lowerBodyPlan = `
      <strong>Lower Body + Cardio:</strong><br>
      1. Pistol/Bulgarian Split Squats – 4 x 10/leg<br>
      2. Jump Squats – 3 x 20<br>
      3. Glute Bridges – 3 x 15<br>
      4. Burpees – 4 x 15<br>
      5. Mountain Climbers – 3 x 30s<br>
      <em>Core Finisher:</em><br>
      Hanging Leg Raises, Russian Twists, Side Plank
    `;

    for (let i = 0; i < days; i++) {
      const date = new Date(startDate);
      date.setDate(startDate.getDate() + i);
      const dayOfWeek = date.getDay();
      const dateStr = date.toDateString();

      const div = document.createElement("div");
      div.classList.add("day");

      const title = document.createElement("div");
      title.innerHTML = `<strong>${dateStr}</strong>`;

      const details = document.createElement("div");
      details.classList.add("details");

      if ((i + 1) % 7 === 0) {
        // Rest day
        div.classList.add("rest-day");
        details.innerHTML = `<strong>Rest Day:</strong> Recovery and hydration.`;
      } else if ((i % 2) === 0) {
        // Upper Body Days: Day 1, 3, 5 etc.
        details.innerHTML = upperBodyPlan;
      } else {
        // Lower Body Days: Day 2, 4, 6 etc.
        details.innerHTML = lowerBodyPlan;
      }

      div.appendChild(title);
      div.appendChild(details);

      div.addEventListener("click", () => {
        div.classList.toggle("active");
      });
      div.addEventListener("dblclick", () => {
        div.classList.remove("active");
      });

      calendar.appendChild(div);
    }
  </script>
</body>
</html>


Here's your complete HTML code for a

