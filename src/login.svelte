
  <script>
  import { navigate } from "svelte-navigator";
    import "./style.css";
    import axios from "axios";
   
   const handleclick = () =>{
    console.log("Inam")
    let data = {
      username: 'Inam',
      password: "123"
    }
    axios
    .post('https://apimocha.com/carbon/login', data)
    .then((res)=>{
      console.log(res);
    
      localStorage.setItem('loggedIn', res.data.loggedIn)
    })

   };
  

  </script>
<div class="page-container">
 
  <div class="left-section">
      <h4 class="text1">Nice to See You Again</h4>
      <h2 class="text2">WELCOME BACK</h2>
      <h5 class="text3">Check out the latest curated collections on all things trending in media, entertainment, and the world at large.</h5>
   
  </div>
  <div class="right-section">
    <div class="right-top">
      <h2 class="login"> Login Account</h2>
      <h5>check out the latest curated collections on all things trending in media, entertainment, and the world at large.</h5>
    </div>
    <div class="textfields">
      <input type="text" id="username" name="username" placeholder="Email ID"><br><br>
      <input type="password" id="password" name="password" placeholder="Password">
    </div>
    <div class="options">
      <input type="checkbox" id="keep-signin" name="keep-signin">
  <label for="keep-signin">Keep me signed in</label>
  <span id="already-member" on:click={() => navigate("/signup")}>Already a member?</span>
    </div>
    <button class="subscribe" on:click={()=> handleclick()}>SUBSCRIBE</button>
  </div>

</div>