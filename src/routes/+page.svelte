<!-- <h1>Welcome to your library project</h1>
<p>Create your package using @sveltejs/package and preview/showcase your work with SvelteKit</p>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p> -->

<svelte:head>
	<link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="" />
	<link
		rel="stylesheet"
		href="https://fonts.googleapis.com/css2?display=swap&family=Noto+Sans:wght@400;500;700;900&family=Plus+Jakarta+Sans:wght@400;500;700;800"
	/>
	<title>Slack Emoji Converter</title>
	<link rel="icon" type="image/x-icon" href="data:image/x-icon;base64," />
	<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
</svelte:head>

<div
	class="group/design-root relative flex size-full min-h-screen flex-col gap-6 overflow-x-hidden bg-white"
	style="font-family: Plus Jakarta Sans, Noto Sans, sans-serif;"
>
	<div>
		<div class="flex items-center justify-between bg-white p-4 pb-2">
			<h2
				class="flex-1 pl-12 pr-12 text-center text-lg font-bold leading-tight tracking-[-0.015em] text-[#111518]"
			>
				Emoji Converter
			</h2>
		</div>
	</div>

	<div class="flex justify-center gap-6">
		<div class="flex w-1/3 flex-wrap items-end gap-4 px-4 py-3">
			<label class="flex min-w-40 flex-1 flex-col">
				<p class="pb-2 text-base font-medium leading-normal text-[#111518]">Input</p>
				<textarea
					placeholder="Type your message here"
					class="form-input flex min-h-96 w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl border border-[#dbe1e6] bg-white p-[15px] text-base font-normal leading-normal text-[#111518] placeholder:text-[#60768a] focus:border-[#dbe1e6] focus:outline-0 focus:ring-0"
				></textarea>
			</label>
		</div>

		<div class="flex w-1/3 flex-wrap items-end gap-4 px-4 py-3">
			<label class="flex min-w-40 flex-1 flex-col">
				<p class="pb-2 text-base font-medium leading-normal text-[#111518]">Output</p>
				<textarea
					placeholder="Converted emojis will appear here"
					class="form-input flex min-h-96 w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl border border-[#dbe1e6] bg-white p-[15px] text-base font-normal leading-normal text-[#111518] placeholder:text-[#60768a] focus:border-[#dbe1e6] focus:outline-0 focus:ring-0"
				></textarea>
			</label>
		</div>
	</div>

	<div>
		<div class="flex justify-center">
			<div class="flex max-w-[480px] flex-1 flex-col items-stretch gap-3 px-4 py-3">
				<button
					class="flex h-10 w-full min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl bg-[#2590f4] px-4 text-sm font-bold leading-normal tracking-[0.015em] text-white"
				>
					<span class="truncate">Convert</span>
				</button>
				<button
					class="flex h-10 w-full min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl bg-[#f0f2f5] px-4 text-sm font-bold leading-normal tracking-[0.015em] text-[#111518]"
				>
					<span class="truncate">Clear</span>
				</button>
			</div>
		</div>
		<footer class="flex flex-col gap-6 px-5 py-10 text-center @container">
			<p class="text-base font-normal leading-normal text-[#60768a]">
				<!-- 2023 Emoji Inc -->
			</p>
		</footer>
		<div class="h-5 bg-white"></div>
	</div>
</div>
