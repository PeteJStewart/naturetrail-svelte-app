<script lang="ts">
	const currentYear = new Date().getFullYear();
</script>

<footer class="border-t-4 border-t-lightgreen bg-white">
	<div class="container mx-auto max-w-7xl px-4 py-12">
		<nav class="mb-8 flex flex-wrap justify-center gap-8">
			<a
				href="/privacy-policy/"
				class="text-base font-medium text-gray-700 transition-colors hover:text-green-600"
			>
				Privacy Policy
			</a>
			<a
				href="/#about"
				class="text-base font-medium text-gray-700 transition-colors hover:text-green-600"
			>
				About
			</a>
			<a
				href="/#features"
				class="text-base font-medium text-gray-700 transition-colors hover:text-green-600"
			>
				Features
			</a>
			<a
				href="mailto:support@naturetrail.app"
				class="text-base font-medium text-gray-700 transition-colors hover:text-green-600"
			>
				Contact
			</a>
		</nav>
		<div class="text-center">
			<p class="text-sm text-gray-600">
				© {currentYear} Nature Trail App. All rights reserved.
			</p>
		</div>
	</div>
</footer>
