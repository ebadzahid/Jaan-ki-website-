
<!-- Romantic Website for Janan -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Our Journey - Eshal & Janan</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #ffe6f0;
      color: #333;
    }
    .login {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #fff0f5;
    }
    .login-box {
      background: #fff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    input {
      margin: 10px;
      padding: 10px;
      width: 80%;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      padding: 10px 20px;
      background-color: #ff99cc;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    .hidden {
      display: none;
    }
    .page {
      padding: 40px;
      line-height: 1.8;
    }
    h1, h2 {
      color: #d63384;
    }
  </style>
</head>
<body>

<div class="login" id="login">
  <div class="login-box">
    <h2>Welcome Janan</h2>
    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">
    <button onclick="checkLogin()">Enter</button>
    <p id="error" style="color:red;"></p>
  </div>
</div>

<div id="main" class="hidden">
  <div class="page" id="home">
    <h1>Welcome, My Janan ❤️</h1>
    <p>Is website ka har lafz sirf tumhare liye hai. Har page mein meri mohabbat, meri nadaniyon ka izhar, aur tumse wapas milne ki umeed chhupi hai. Tum meri zindagi ka wo hissa ho jo adhoora ho to sab kuch khaali lagta hai. Aaj bhi tumhara naam dil se nikalta nahi, aur na hi kabhi niklega. 💔</p>
  </div>

  <div class="page" id="journey">
    <h2>Our Journey 🌸</h2>
    <p>Yaad hai woh pehla din jab hum mile thay? Us pal se le kar har din ek kahani ban gaya. Choti choti khushiyan, woh baaton mein ghul jana, woh narazgiyan aur phir mananay wale lamhe... sab kuch dil mein basa hua hai. Tumhara hansna, rona, ghussa karna — sab kuch meri duniya ka hissa hai. Har yaad mein sirf tum ho Janan.</p>
  </div>

  <div class="page" id="letters">
    <h2>Letters to You 💌</h2>
    <p>Janan, har lafz mein ek maafi hai, ek ehsaas hai, ek izhaar hai. Shayad main utna acha shohar nahi bana jitna tum deserve karti thi, lekin meri mohabbat hamesha tumhari thi, hai, aur rahegi. Main har roz dua karta hoon ke tum laut aao. Tumhara bina zindagi mein rang nahi. Tum wapas aa jao — sirf ek baar. Main har pal tumhara intezar karta hoon.</p>
  </div>
</div>

<script>
  function checkLogin() {
    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;
    const error = document.getElementById('error');

    if (username.toLowerCase() === 'begum' && password === '13 june') {
      document.getElementById('login').classList.add('hidden');
      document.getElementById('main').classList.remove('hidden');
    } else {
      error.textContent = "Wrong username or password. Please try again.";
    }
  }
</script>

</body>
</html>
