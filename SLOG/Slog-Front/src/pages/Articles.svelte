<script>
	import ArticleHeader from "../components/ArticleHeader.svelte";
	import ArticleList from "../components/ArticleList.svelte";
	import ArticleAddForm from "../components/ArticleAddForm.svelte";
</script>

<div class="svelte-demo mdl-color--grey-100 mdl-layout mdl-js-layout mdl-layout--fixed-header">
	<ArticleHeader />

	<main class="mdl-layout__content">
		<ArticleAddForm />
		<ArticleList />
	</main>
</div>
