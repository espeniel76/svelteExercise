<script>
	import { getContext } from "svelte";
	let count = getContext("count");
</script>

<button>
	increment count [{count}]
</button>
