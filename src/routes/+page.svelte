<script>
	import Hero from '$lib/components/hero.svelte';

	let name = 'DevEmm';
	let description = 'Lorem ipsum dolor sit amet consectetur adipisicing elit.';
</script>

<Hero />
<h1>Welcome {name}</h1>

<div
	class="w-full max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
>
	<div class="flex justify-end px-4 pt-4">
		<button
			id="dropdownButton"
			data-dropdown-toggle="dropdown"
			class="inline-block text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:ring-4 focus:outline-none focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-1.5"
			type="button"
		>
			<span class="sr-only">Open dropdown</span>
			<svg
				class="w-5 h-5"
				aria-hidden="true"
				xmlns="http://www.w3.org/2000/svg"
				fill="currentColor"
				viewBox="0 0 16 3"
			>
				<path
					d="M2 0a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3Zm6.041 0a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3ZM14 0a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3Z"
				/>
			</svg>
		</button>
		<!-- Dropdown menu -->
		<div
			id="dropdown"
			class="z-10 hidden text-base list-none bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700"
		>
			<ul class="py-2" aria-labelledby="dropdownButton">
				<li>
					<a
						href="#"
						class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"
						>Edit</a
					>
				</li>
				<li>
					<a
						href="#"
						class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"
						>Export Data</a
					>
				</li>
				<li>
					<a
						href="#"
						class="block px-4 py-2 text-sm text-red-600 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white"
						>Delete</a
					>
				</li>
			</ul>
		</div>
	</div>
	<div class="flex flex-col items-center pb-10">
		<img
			class="w-24 h-24 mb-3 rounded-full shadow-lg"
			src="/docs/images/people/profile-picture-3.jpg"
			alt="Bonnie image"
		/>
		<h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">Bonnie Green</h5>
		<span class="text-sm text-gray-500 dark:text-gray-400">Visual Designer</span>
		<div class="flex mt-4 md:mt-6">
			<a
				href="#"
				class="inline-flex items-center px-4 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
				>Add friend</a
			>
			<a
				href="#"
				class="inline-flex items-center px-4 py-2 text-sm font-medium text-center text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-gray-200 dark:bg-gray-800 dark:text-white dark:border-gray-600 dark:hover:bg-gray-700 dark:hover:border-gray-700 dark:focus:ring-gray-700 ms-3"
				>Message</a
			>
		</div>
	</div>
</div>

<div
	class="p-4 mb-4 text-sm text-blue-800 rounded-lg bg-blue-50 dark:bg-gray-800 dark:text-blue-400"
	role="alert"
>
	<span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
</div>
<div
	class="p-4 mb-4 text-sm text-red-800 rounded-lg bg-red-50 dark:bg-gray-800 dark:text-red-400"
	role="alert"
>
	<span class="font-medium">Danger alert!</span> Change a few things up and try submitting again.
</div>
<div
	class="p-4 mb-4 text-sm text-green-800 rounded-lg bg-green-50 dark:bg-gray-800 dark:text-green-400"
	role="alert"
>
	<span class="font-medium">Success alert!</span> Change a few things up and try submitting again.
</div>
<div
	class="p-4 mb-4 text-sm text-yellow-800 rounded-lg bg-yellow-50 dark:bg-gray-800 dark:text-yellow-300"
	role="alert"
>
	<span class="font-medium">Warning alert!</span> Change a few things up and try submitting again.
</div>
<div
	class="p-4 text-sm text-gray-800 rounded-lg bg-gray-50 dark:bg-gray-800 dark:text-gray-300"
	role="alert"
>
	<span class="font-medium">Dark alert!</span> Change a few things up and try submitting again.
</div>

<p>{description}</p>
