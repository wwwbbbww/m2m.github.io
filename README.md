body { margin:0; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background:#000; color:#f0f0f0; }

#overlay { position:fixed; top:0; left:0; width:100%; height:100%; overflow-y:auto; padding:20px; z-index:9999; }
#overlay h2 { color:#ff3c3c; text-shadow: 0 0 8px #ff3c3c, 0 0 16px #ff0000; margin-bottom:10px; }

.flex { display:flex; justify-content:center; flex-wrap:wrap; gap:12px; margin-top:1rem; }

.flex-child { background: #111; padding:12px 18px; min-width:180px; border-radius:12px; box-shadow:0 0 12px rgba(255,0,0,0.5); display:flex; flex-direction:column; align-items:center; transition: transform 0.2s, box-shadow 0.2s; }
.flex-child:hover { transform: translateY(-5px); box-shadow:0 0 20px rgba(255,0,0,0.8); }
.flex-child img { width:32px; height:32px; border-radius:50%; border:1px solid #666; margin-bottom:6px; }

.input-search, .input-select { font-size:16px; padding:6px 12px; border-radius:30px; background-color:#222; color:white; border:1px solid #444; margin-bottom:10px; }

.viewer-btn { display:block; width:80px; margin:6px auto 12px auto; padding:4px 0; border-radius:6px; background-color:#222; color:#fff; text-decoration:none; font-weight:bold; text-align:center; font-size:12px; box-shadow:0 0 6px rgba(255,0,0,0.5); transition: all 0.2s; }
.viewer-btn:hover { background-color:#ff0000; box-shadow:0 0 12px rgba(255,0,0,0.8); }

.total-count { position:fixed; top:50px; left:10px; background-color:darkslateblue; color:white; padding:5px 10px; border-radius:5px; z-index:9999; }

.users .user-info { display:flex; align-items:center; margin-bottom:6px; justify-content:flex-start; }
.users .user-info p { margin-left:6px; font-size:13px; color:#ccc; overflow-wrap:anywhere; }
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
