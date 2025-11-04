<script lang="ts">
	import logo from '$lib/assets/naturetrail-app-logo.png';
</script>

<svelte:head>
	<title>Nature Trail App - Discover and Explore Nature Trails</title>
	<meta
		name="description"
		content="Discover beautiful nature trails, track your hikes, and connect with nature. Your ultimate companion for outdoor adventures."
	/>
</svelte:head>

<!-- Hero Section -->
<section class="hero flex min-h-[80vh] items-center justify-center bg-[#F9F3E3]">
	<div
		class="hero-content flex max-w-6xl flex-col items-center justify-center px-4 py-16 text-center"
	>
		<div class="mx-auto max-w-4xl">
			<div class="mb-10 flex justify-center">
				<img src={logo} alt="Nature Trail App" class="h-auto w-72 max-w-full md:w-96" />
			</div>
			<h1 class="mb-6 text-5xl leading-tight font-bold text-gray-800 md:text-7xl">
				Discover Nature's Beauty
			</h1>
			<p class="mx-auto max-w-3xl py-6 text-xl leading-relaxed text-gray-600 md:text-2xl">
				Your ultimate companion for exploring scenic trails, tracking your adventures, and
				connecting with the great outdoors. Find your next journey today.
			</p>
			<div class="mt-8 flex flex-wrap justify-center gap-4">
				<a href="#features" class="btn bg-[#39653A] px-8 text-white shadow-lg btn-soft btn-lg">
					Explore Features
				</a>
				<a
					href="#about"
					class="btn border-2 border-green-600 px-8 text-green-700 btn-outline btn-lg hover:border-green-600 hover:bg-green-600 hover:text-white"
				>
					Learn More
				</a>
			</div>
		</div>
	</div>
</section>

<!-- Features Section -->
<section id="features" class="bg-white py-24">
	<div class="container mx-auto max-w-7xl px-4">
		<div class="mb-16 text-center">
			<h2 class="mb-4 text-4xl font-bold text-gray-800 md:text-5xl">
				Everything You Need for Your Adventure
			</h2>
			<p class="mx-auto max-w-2xl text-lg text-gray-600 md:text-xl">
				Powerful features designed to enhance your outdoor experience
			</p>
		</div>

		<div class="grid gap-8 md:grid-cols-2 lg:grid-cols-3">
			<!-- Feature 1 -->
			<div
				class="card border border-green-100 bg-linear-to-br from-green-50 to-emerald-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
			>
				<div class="card-body p-8">
					<div
						class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-green-600 shadow-md"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8 text-white"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0021 18.382V7.618a1 1 0 00-.553-.894L15 4m0 13V4m0 0L9 7"
							/>
						</svg>
					</div>
					<h3 class="mb-3 card-title text-2xl text-gray-800">Discover Trails</h3>
					<p class="leading-relaxed text-gray-600">
						Browse curated nature trails with detailed information, difficulty levels, and audio
						descriptions at points of interest.
					</p>
				</div>
			</div>

			<!-- Feature 2 - Welsh Language Learning -->
			<div
				class="card border border-blue-100 bg-linear-to-br from-blue-50 to-indigo-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
			>
				<div class="card-body p-8">
					<div
						class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-600 shadow-md"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8 text-white"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129"
							/>
						</svg>
					</div>
					<h3 class="mb-3 card-title text-2xl text-gray-800">Welsh Language Learning</h3>
					<p class="leading-relaxed text-gray-600">
						Immerse yourself in Welsh culture with fully bi-lingual trail descriptions, audio guides
						in Welsh and English, and learn place names in their native language.
					</p>
				</div>
			</div>

			<!-- Feature 2 - Track Progress (COMMENTED OUT) -->
			<!-- <div
					class="card border border-teal-100 bg-gradient-to-br from-teal-50 to-cyan-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
				>
					<div class="card-body p-8">
						<div
							class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-teal-600 shadow-md"
						>
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-8 w-8 text-white"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
								/>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
								/>
							</svg>
						</div>
						<h3 class="card-title mb-3 text-2xl text-gray-800">Track Progress</h3>
						<p class="leading-relaxed text-gray-600">
							Monitor your hiking adventures with GPS tracking, distance metrics, elevation
							profiles, and detailed activity logs.
						</p>
					</div>
				</div> -->

			<!-- Feature 3 - Share Memories (COMMENTED OUT) -->
			<!-- <div
					class="card border border-blue-100 bg-gradient-to-br from-blue-50 to-indigo-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
				>
					<div class="card-body p-8">
						<div
							class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-600 shadow-md"
						>
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-8 w-8 text-white"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M3 9a2 2 0 012-2h.93a2 2 0 001.664-.89l.812-1.22A2 2 0 0110.07 4h3.86a2 2 0 011.664.89l.812 1.22A2 2 0 0018.07 7H19a2 2 0 012 2v9a2 2 0 01-2 2H5a2 2 0 01-2-2V9z"
								/>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M15 13a3 3 0 11-6 0 3 3 0 016 0z"
								/>
							</svg>
						</div>
						<h3 class="card-title mb-3 text-2xl text-gray-800">Share Memories</h3>
						<p class="leading-relaxed text-gray-600">
							Capture and share your favorite moments with the community through stunning photos and
							detailed trail reports.
						</p>
					</div>
				</div> -->

			<!-- Feature 4 - Weather Updates (COMMENTED OUT) -->
			<!-- <div
					class="card border border-amber-100 bg-gradient-to-br from-amber-50 to-yellow-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
				>
					<div class="card-body p-8">
						<div
							class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-amber-600 shadow-md"
						>
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-8 w-8 text-white"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"
								/>
							</svg>
						</div>
						<h3 class="card-title mb-3 text-2xl text-gray-800">Weather Updates</h3>
						<p class="leading-relaxed text-gray-600">
							Get real-time weather forecasts and current trail conditions to plan your perfect
							outdoor adventure safely.
						</p>
					</div>
				</div> -->

			<!-- Feature 5 - Join Community (COMMENTED OUT) -->
			<!-- <div
					class="card border border-purple-100 bg-gradient-to-br from-purple-50 to-pink-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
				>
					<div class="card-body p-8">
						<div
							class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-purple-600 shadow-md"
						>
							<svg
								xmlns="http://www.w3.org/2000/svg"
								class="h-8 w-8 text-white"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"
								/>
							</svg>
						</div>
						<h3 class="card-title mb-3 text-2xl text-gray-800">Join Community</h3>
						<p class="leading-relaxed text-gray-600">
							Connect with a vibrant community of nature enthusiasts, share tips, and discover
							hidden gems together.
						</p>
					</div>
				</div> -->

			<!-- Feature 6 -->
			<div
				class="card border border-slate-100 bg-gradient-to-br from-slate-50 to-gray-50 shadow-lg transition-all duration-300 hover:-translate-y-1 hover:shadow-2xl"
			>
				<div class="card-body p-8">
					<div
						class="mb-6 flex h-16 w-16 items-center justify-center rounded-2xl bg-slate-700 shadow-md"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8 text-white"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"
							/>
						</svg>
					</div>
					<h3 class="mb-3 card-title text-2xl text-gray-800">Offline Access</h3>
					<p class="leading-relaxed text-gray-600">
						Download trail maps and information for offline use, so you stay on track even without
						cell signal in remote areas.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- About Section -->
<section id="about" class="bg-gradient-to-br from-lightgreen via-darkgreen to-lightgreen py-24">
	<div class="container mx-auto max-w-5xl px-4">
		<div class="text-center">
			<h2 class="mb-8 text-4xl font-bold text-gray-100 md:text-5xl">About Nature Trail App</h2>
			<div class="space-y-6 text-lg leading-relaxed text-gray-100">
				<p class="text-xl">
					Nature Trail App was born from a passion for the outdoors and a desire to make nature more
					accessible to everyone. We believe that connecting with nature shouldn't be complicated—it
					should be an adventure.
				</p>
				<p class="text-xl">
					Our mission is to help outdoor enthusiasts discover, explore, and share the beauty of
					natural trails around the world. Whether you're a seasoned hiker or just starting your
					journey into nature, we're here to guide you every step of the way.
				</p>
				<p class="text-xl font-medium text-gray-100">
					Join thousands of nature lovers who have already discovered their next adventure with
					Nature Trail App. The great outdoors is waiting for you.
				</p>
			</div>
			<div class="mt-12">
				<a
					href="mailto:support@naturetrail.app"
					class="btn border-none bg-green-600 px-10 text-white shadow-lg btn-lg hover:bg-green-700"
				>
					Get in Touch
				</a>
			</div>
		</div>
	</div>
</section>
