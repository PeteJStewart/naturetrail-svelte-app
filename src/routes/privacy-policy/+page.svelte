<script lang="ts">
	import PolicyCard from '$lib/components/PolicyCard.svelte';
	import PolicySection from '$lib/components/PolicySection.svelte';

	const year = new Date().getFullYear();

	/**
	 * IMPORTANT:
	 * This MUST match your Google Play developer name (legal entity) exactly as shown on the store listing.
	 * If Google Play shows "Tinkr Ltd" (or similar), change it here to match character-for-character.
	 */
	const developerLegalEntity = 'Tinkr';

	/**
	 * Optional: keep an explicit list of current app names covered.
	 * Add new app names here as you publish them.
	 */
	const coveredApps = ['Nant Gwrtheyrn', 'NatureTrail'];
</script>

<svelte:head>
	<title>Privacy Policy — NatureTrail Apps (by {developerLegalEntity})</title>
	<meta
		name="description"
		content="Privacy Policy for the NatureTrail family of apps (including Nant Gwrtheyrn) published by Tinkr. We don’t collect personal data; limited technical data is used only for error reporting and internal feature testing."
	/>
	<meta name="robots" content="noindex,follow" />
</svelte:head>

<section class="flex min-h-[80vh] items-center justify-center">
	<div class="max-w-6xl px-4 py-16">
		<PolicyCard>
			<header>
				<h1>Privacy Policy — NatureTrail Apps (by {developerLegalEntity})</h1>
				<div class="sub">Effective date: November 2025</div>

				<div class="sub">
					<strong>Developer / legal entity (Google Play listing):</strong> {developerLegalEntity}
				</div>

				<div class="sub">
					<strong>Apps covered by this policy:</strong> This Privacy Policy applies to the NatureTrail family of
					apps published by {developerLegalEntity}, including {coveredApps.join(', ')}, and other
					NatureTrail-branded trail apps we publish from time to time.
				</div>
			</header>

			<div class="summary" role="note" aria-label="Plain-language summary">
				<strong>Summary:</strong> We don’t collect personal data. Settings stay on your device. We use
				Sentry (error reporting) and LaunchDarkly (internal feature testing) which may receive limited
				technical, non-identifiable information (e.g. device/OS and crash logs) to keep the app stable
				and test new features. No advertising. No selling of data.
			</div>

			<PolicySection id="overview" title="1. Overview">
				<p>
					The <em>NatureTrail family of apps</em> (including <strong>Nant Gwrtheyrn</strong>) helps you
					explore local nature trails and learn Welsh. We value your privacy. These apps do
					<strong>not collect or store any personal information</strong>
					about you. Your preferences (such as language choice or completed routes) are stored
					<strong>locally on your device</strong> and are never transmitted to us or third parties.
				</p>
			</PolicySection>

			<PolicySection id="info-we-collect" title="2. Information We Collect">
				<p>
					We do <strong>not</strong> collect personal data (e.g. name, email, contact details,
					location history). The app only sends limited,
					<strong>non-identifiable technical data</strong> to the services below to maintain app quality
					and test features.
				</p>
			</PolicySection>

			<PolicySection id="sentry" title="3. Error Reporting (Sentry)">
				<p>
					We use <strong>Sentry</strong> to monitor errors and crashes so we can fix problems. When an
					error occurs, Sentry may receive:
				</p>
				<ul>
					<li>Device type and operating system version</li>
					<li>App version</li>
					<li>Error messages and stack traces</li>
				</ul>
				<p>
					This is used only to debug and improve stability. Sentry does <strong>not</strong> receive
					personal or identifying information. Data is transmitted securely and retained for a limited
					period solely for troubleshooting.
				</p>
			</PolicySection>

			<PolicySection id="launchdarkly" title="4. Feature Testing (LaunchDarkly)">
				<p>
					We use <strong>LaunchDarkly</strong> to enable/disable experimental features on specific test
					devices. LaunchDarkly may receive:
				</p>
				<ul>
					<li>An anonymous device identifier (e.g. <code>test_device_1</code>)</li>
					<li>Device model and operating system version</li>
				</ul>
				<p>
					This data is <strong>non-identifiable</strong> and used only for internal testing and feature
					control. We do not send personal details or precise location to LaunchDarkly.
				</p>
			</PolicySection>

			<PolicySection id="local-storage" title="5. Local Storage">
				<p>
					Your settings—such as language preferences, visited points of interest, and downloaded
					maps—are stored
					<strong>only on your device</strong>. Removing the app deletes this data.
				</p>
			</PolicySection>

			<PolicySection id="children" title="6. Children’s Privacy">
				<p>
					The app does not collect or store data from users of any age, including children. No
					accounts are required.
				</p>
			</PolicySection>

			<PolicySection id="security" title="7. Data Security">
				<p>
					Communications with our service providers use secure, encrypted connections. Our providers
					follow strong data-protection standards (including GDPR compliance measures).
				</p>
			</PolicySection>

			<PolicySection id="rights" title="8. Your Rights">
				<p>
					As we do not collect personal data, there is no personal data for you to access, correct,
					or delete. If you have any questions, contact {developerLegalEntity} at
					<a href="mailto:support@naturetrail.app">support@naturetrail.app</a>.
				</p>
			</PolicySection>

			<PolicySection id="changes" title="9. Changes to This Policy">
				<p>
					We may update this policy from time to time. The latest version will always be available
					within the app and at
					<a href="https://naturetrail.app/privacy">naturetrail.app/privacy</a>.
				</p>
			</PolicySection>

			<footer>&copy; {year} {developerLegalEntity}. All rights reserved.</footer>
		</PolicyCard>
	</div>
</section>
