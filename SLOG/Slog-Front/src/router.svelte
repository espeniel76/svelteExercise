<script>
	import { Route } from "tinro";
	import Aritcles from "./pages/Articles.svelte";
	import Login from "./pages/Login.svelte";
	import Register from "./pages/Register.svelte";
</script>

<Route path="/" redirect="/articles" />
<Route path="/articles/*"><Aritcles /></Route>
<Route path="/login"><Login /></Route>
<Route path="/register"><Register /></Route>
