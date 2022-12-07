
  <script>
  import { navigate } from "svelte-navigator";
    import "./style.css"
  </script>
<div class="page-container">
 
  <div class="left-section">
      <h4 class="text1">Nice to See You Again</h4>
      <h2 class="text2">WELCOME BACK</h2>
      <h5 class="text3">Check out the latest curated collections on all things trending in media, entertainment, and the world at large.</h5>
   
  </div>
  <div class="right-section">
    <div class="right-top">
      <h2 class="signup"> Signup Account</h2>
      <h5>check out the latest curated collections on all things trending in media, entertainment, and the world at large.</h5>
    </div>
    <div class="textfields">
      <input type="text" id="name" name="name" placeholder="Full Name">
      <input type="number" id="number" name="number" placeholder="Phone number">
      <input type="text" id="username" name="username" placeholder="Email ID">
      <input type="password" id="password" name="password" placeholder="Password">
      <input type="password" id="password" name="password" placeholder="Confirm Password">
    
    </div>
    <div class="options">
      <input type="checkbox" id="keep-signin" name="keep-signin">
  <label for="keep-signin">Keep me signed in</label>
  <span id="already-member"on:click={() => navigate("/login")}>login to account?</span>
    </div>
    <div class="subscribe">SUBSCRIBE</div>
  </div>

</div>