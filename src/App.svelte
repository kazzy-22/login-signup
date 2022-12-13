<script>
     import { Router, Route, Link } from "svelte-navigator";
     import home from "./home.svelte";
     import Login from "./login.svelte";
     import signup from "./signup.svelte";

</script>

<Router>
    <Route path="/signup" component={signup} />
    <Route path="/login" component={Login} />
    <Route path="/home"  component={home}/>
</Router>