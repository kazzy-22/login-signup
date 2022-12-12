<script>
  import { navigate } from "svelte-navigator";
   import "./home.css"

</script>

<div class="container">
    <div class="top-section">
        <div class="top-left">
            <img src="src/images.png" alt="logo">
        </div>
        <div class="top-right">
            <ul id="navbar">
                <li on:click={() => navigate("/home")} >Home</li>
                <li  on:click={() => navigate("/login")} >login</li>
            </ul>
        </div>
    </div>
    <div class="bottom-section">
        <div class="bottom-text">
            <h1 id="text1">Think Diffrent</h1>
            <h4 id="text2">Reduce your carbon footprint in style</h4>
        </div>
        <div class="button" on:click={() => navigate("/signup")} >Sign up now</div>
    </div>
</div>