<script>
    import { Button } from 'webcoreui/svelte'
    import { github } from 'webcoreui/icons'

    import Layout from './components/Layout.svelte'
</script>

<Layout>
	<h1 class="flex center md">
		Welcome to <img src="logo.svg" width="160" alt="logo" />
	</h1>
	<p>
		Edit <code>src/App.svelte</code> to get started.
		For documentation, visit <a href="https://webcoreui.dev" target="_blank">webcoreui.dev</a>
	</p>
	<div class="flex justify-center xs">
		<Button href="https://webcoreui.dev" target="_blank">
			Get Started
		</Button>
		<Button
			href="https://github.com/Frontendland/webcoreui"
			target="_blank"
			theme="secondary"
		>
			{@html github}
			GitHub
		</Button>
	</div>
</Layout>

<style lang="scss">
	@use 'webcoreui/config' as *;

	p {
		@include typography(center);
    }
</style>
