<script>
     import { Router, Route, Link } from "svelte-navigator";
     import home from "./home.svelte";
     import login from  "./login.svelte";
     import signup from "./signup.svelte";

</script>

<Router>
    <Route path="/signup" component={signup} />
    <Route path="/login" component={login} />
    <Route path="/home"  component={home}/>
</Router>