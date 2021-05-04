<script context="module">
	export async function load() {
		return { props: { html: '<p>hello weird unrecoverable error in Root</p>' } };
	}
</script>

<script>
	export let html;
</script>

<slot />
<footer>{@html html}</footer>
