<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>MoZai Server</title>

<!-- Favicon -->
<link rel="icon" href="favicon.png" type="image/png">

<style>
  body {
    margin: 0;
    min-height: 100vh;
    background-image: url("bg.jpg"); 
    background-size: cover;
    background-position: center;
    font-family: Arial, sans-serif;
    color: white;
  }

  .container {
    background: black;
    max-width: 900px;
    width: 90%;
    margin: 40px auto;
    padding: 30px;
    border-radius: 15px;
  }

  h1, h2 { text-align: center; }

  form input, form textarea, form select {
    width: 100%;
    padding: 10px;
    margin: 8px 0 15px;
    border-radius: 6px;
    border: none;
    font-size: 15px;
  }

  textarea { resize: vertical; }

  button {
    padding: 12px 20px;
    background: #00ff99;
    border: none;
    border-radius: 8px;
    font-size: 16px;
    cursor: pointer;
  }

  button:hover { background: #00cc77; }

  .section { margin-top: 40px; }

  .store-item {
    background: #111;
    padding: 15px;
    margin: 10px 0;
    border-radius: 8px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .store-item button { width: 120px; }

  label { font-weight: bold; }
</style>
</head>

<body>

<div class="container">
  <h1>MoZai Server</h1>

  <div class="section" id="application">
    <h2>Staff Application</h2>
    <form action="mailto:MoZazm18@gmail.com" method="post" enctype="text/plain">
      <label>Minecraft Username</label>
      <input type="text" name="Minecraft Username" required>

      <label>Email</label>
      <input type="email" name="Email" required>

      <label>Application Password</label>
      <input type="password" name="Application Password" required>

      <label>Age</label>
      <input type="number" name="Age" required>

      <label>Gender</label>
      <select name="Gender" required>
        <option value="">Select</option>
        <option>Male</option>
        <option>Female</option>
      </select>

      <label>Reason for applying</label>
      <textarea name="Reason" rows="4" required></textarea>

      <label>
        <input type="checkbox" required>
        I confirm all information is real
      </label>

      <br><br>
      <button type="submit">Submit Application</button>
    </form>
  </div>

  <div class="section" id="store">
    <h2>Store - Buy Items / Cards</h2>

    <div class="store-item">
      <span>Diamond Sword</span>
      <button onclick="alert('Purchased Diamond Sword!')">Buy</button>
    </div>
    <div class="store-item">
      <span>Gold Armor Set</span>
      <button onclick="alert('Purchased Gold Armor Set!')">Buy</button>
    </div>
    <div class="store-item">
      <span>VIP Card</span>
      <button onclick="alert('Purchased VIP Card!')">Buy</button>
    </div>
  </div>

  <div class="section" id="complaint">
    <h2>Report / Submit Evidence</h2>
    <form>
      <label>Player Name / Issue</label>
      <input type="text" name="issue" required>

      <label>Description</label>
      <textarea name="description" rows="4" required></textarea>

      <label>Attach Image / Evidence</label>
      <input type="file" name="evidence" accept="image/*">

      <br><br>
      <button type="button" onclick="alert('Complaint submitted (demo)!')">Submit Complaint</button>
    </form>
  </div>

</div>

</body>
</html>
