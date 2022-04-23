<script>
	import { setContext } from "svelte";

	import PanelComponent from "./components/panelComponent.svelte";

	let count = 1234567889;

	setContext("count", count);
</script>

<PanelComponent />
