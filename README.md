<!DOCTYPE html>
<html lang="az">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gartic.io WhoWhere Viewer</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<div id="overlay">
  <header><h2>M2H Gartic Viewer</h2></header>
  <p>Hazırki Otağlar</p>

  <input type="text" id="searchRoom" placeholder="Otaq axtar..." class="input-search">

  <select id="languageSelect" class="input-select">
    <option value="23" selected>Azərbaycanca</option>
    <option value="2">English</option>
    <option value="3">Español</option>
    <option value="4">Français</option>
    <option value="5">Italiano</option>
    <option value="6">Deutsch</option>
    <option value="7">Русский</option>
    <option value="8">Türkçe</option>
    <!-- lazım olan digər dillər əlavə oluna bilər -->
  </select>

  <div id="flex" class="flex"></div>
</div>

<div id="totalCount" class="total-count"></div>

<script src="script.js"></script>
</body>
</html>
